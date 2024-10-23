# Hospital Management System - High-Level Design
This document outlines the high-level design and system architecture of the Hospital Management System using Java, JSP, and MySQL. The system is designed to manage hospital operations including patient records, staff management, and appointment scheduling.
## System Architecture Overview
The system consists of three primary layers:
1. User Interface (UI)**2. **Application Layer (Business Logic)
3. Data Layer (Database)
### 1. User Interface (UI)- Role: This is the front-end part of the system where users interact. Users include hospital staff, doctors, and administrators.
- Technologies: Java Server Pages (JSP), HTML, CSS, and JavaScript.- Components:
  - Web Forms: Used for patient registration, appointment scheduling, and staff management.  - Dashboards: Displays key performance indicators (KPIs) like patient status and appointment schedules.
  - Reports: Allows users to generate reports (e.g., patient history, hospital statistics).
### 2. Application Layer (Business Logic)- Role: The core processing layer where the business rules and system logic are executed.
- Technologies: Java (JDK), Servlet technology.- Components:
  - Patient Management: Manages patient records, admission/discharge processes.  - Appointment Scheduling: Manages doctor appointments, availability, and scheduling rules.
  - Hospital Operations: Manages staff, rooms, and resources.  - Shortest Path Algorithm: Uses Dijkstra's Algorithm for calculating the shortest path in hospital logistics (e.g., moving patients between departments).
### 3. Data Layer (Database)
- Role: Responsible for persistent data storage, retrieval, and manipulation.- Technologies: MySQL Database.
- Components:  - Patient Records: Stores patient information including medical history, treatments, and appointments.
  - Staff Information: Stores staff details like doctor schedules, duties, and availability.  - Appointments: Tracks patient appointments, doctor assignments, and hospital room occupancy.
## System Flow and Interaction
1. User Interactions: Users interact with the system through the web interface (UI). They can input data, schedule appointments, or generate reports.
2. Business Logic Execution: The input is processed by the application layer which checks the business rules, such as appointment availability or patient admission status.3. Database Interaction: The application communicates with the MySQL database to fetch or update records, such as patient details or scheduling information.
4. Results Display: The output is presented back to the user through the UI, providing confirmation of successful actions or displaying requested reports.
### Interaction Diagram
```plaintext[ User Interface (UI) ] <--> [ Application Layer (Business Logic) ] <--> [ Data Layer (Database) ]
                                |                                |
                       [ Shortest Path Calculation (Dijkstra's Algorithm) ]
