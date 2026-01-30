# Information Gathering

## 1.Problem Statement
Campus Network Complaint System is a database-based system that allows students and staff to register network-related complaints (Wi-Fi, LAN, slow internet, outages), track their status, and enables network administrators to manage, assign, and resolve these complaints efficiently using CRUD operations implemented in user friendly way.

## 2.Stakeholders

### a) Students / Staff

Register network complaints
View complaint status
Provide location and issue details

### b) Network Administrator 

View all complaints
Assign complaints to technicians
Update complaint status
Maintain network records

## 3.Data to Collect 

### A.User Information (Students / Staff)
#### Attributes to collect:

User ID (Primary Key)
Name
Role (Student / Faculty / Staff)
Roll No / Employee ID
Department
Phone Number
Email
Hostel / Block / Building

### B. Network Location Details
Location ID (Primary Key)
Building Name (Hostel, Academic Block, Library)
Floor Number
Room / Lab Number

### C. Complaint Details
Complaint ID (Primary Key)
User ID (Foreign Key)
Location ID (Foreign Key)
Complaint Type (No Internet / Slow Speed / Disconnection)
Description
Complaint Date
Priority (Low / Medium / High)
Status (Pending / In Progress / Resolved)

### D. Technician / Admin Details
Technician ID (Primary Key)
Name
Phone Number
Email
Assigned Area
Availability Status

### E. Complaint Assignment Details
Tracks who is handling what:
Assignment ID (Primary Key)
Complaint ID (Foreign Key)
Technician ID (Foreign Key)
Assigned Date
Resolution Date
Remarks

## 4️.Functional Requirements 

Allow users to register network complaints
Store complaint details in database
Display complaint status to users
Assign complaints to technicians
Update complaint status after resolution
Maintain user and technician records
Generate complaint reports

## 5️.Non-Functional Requirements 

System should ensure data integrity
Only admins can assign complaints
Duplicate complaints should be avoided
Database should be normalized
System should support fast retrieval

## 6️.Constraints

Each complaint must belong to a valid user
Each complaint must have one current status
A technician can handle multiple complaints
A complaint can be assigned to only one technician at a time
Status must follow sequence: Pending → In Progress → Resolved



