The Student Attendance Via Face Recognition is a python based project application, which automates student attendance tracking and monitoring. Built on Tkinter GUI and Pandas, the system successfully captures student face and records attendance into a .csv file.
This desktop application automates the traditional student attendance process using Computer Vision. By leveraging facial recognition, the system identifies students in real-time and logs their attendance automatically, reducing manual overhead and eliminating proxy attendance.


->Language: Python

->Computer Vision: OpenCV

->Algorithms: Haar Cascade Classifier (Face Detection), Local Binary Patterns Histograms / LBPH (Face Recognition)

->Data Storage: CSV / Pandas


Face Detection: Utilizes the haarcascade_frontalface_default.xml model for fast, lightweight, and highly accurate real-time face detection within standard environmental conditions.

Face Recognition (LBPH): The LBPH algorithm was specifically chosen for its robustness to varying lighting conditions and its computational efficiency. Unlike heavy deep learning models that require immense GPU power, LBPH extracts local features by comparing pixel intensities with their neighbors, making it highly effective for real-time edge processing on standard desktop hardware.

Data Handling: Attendance records are dynamically written to StudentDetails.csv, capturing precise timestamps and student IDs.

While currently optimized for local processing and flat-file storage, the architecture is designed with scalability in mind. Future iterations will focus on distributed deployment:

Database Migration: Transitioning the data storage layer from local .csv files to a high-performance, distributed NoSQL database (such as Couchbase) to handle concurrent attendance logging across hundreds of classrooms simultaneously with sub-millisecond latency.

Cloud Integration: Containerizing the application to synchronize local edge-device data with a centralized cloud server for university-wide real-time analytics.

Liveness Detection: Implementing anti-spoofing techniques to ensure physical presence.
