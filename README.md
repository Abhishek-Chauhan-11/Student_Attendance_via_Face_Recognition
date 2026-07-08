ABOUT

The Student Attendance Via Face Recognition is a python based project application, which automates student attendance tracking and monitoring. Built on Tkinter GUI and Pandas, the system successfully captures student face and records attendance into a .csv file. This application automates the traditional student attendance process using Computer Vision. By leveraging facial recognition, the system identifies students in real-time and logs their attendance automatically, reducing manual overhead and eliminating proxy attendance.

TECHNICAL ASPECTS

->Language: Python

->Computer Vision: OpenCV

->Algorithms: Haar Cascade Classifier (Face Detection), Local Binary Patterns Histograms / LBPH (Face Recognition)

->Data Storage: CSV / Pandas

IMPLEMENTATION

Face Detection: Utilizes the "haarcascade_frontalface_default.xml" model for fast, lightweight, and highly accurate real-time face detection in standard environmental conditions.

Face Recognition (LBPH): The LBPH algorithm was specifically chosen for its robustness to varying lighting conditions and its computational efficiency. LBPH extracts local features by comparing pixel intensities with their neighbors, making it highly effective for real-time edge processing on standard computer hardware.

Data Handling: Attendance records are dynamically written to "StudentDetails.csv", capturing accurate timestamps and student IDs.

SCALABILITY & FUTURE

While currently optimized for local processing and flat-file storage, the architecture is designed with scalability in mind. If required, then in the future iterations can also be focused on distributed deployment,

1). Database Migration: Transitioning the data storage layer from local .csv files to a high-performance, distributed NoSQL database to handle concurrent attendance logging across hundreds of classrooms simultaneously with low latency.

2). Cloud Integration: Containerizing the application to synchronize local edge-device data with a centralized cloud server for university-wide real-time analytics.

3). Liveness Detection: Implementing anti-spoofing techniques to ensure physical presence.
