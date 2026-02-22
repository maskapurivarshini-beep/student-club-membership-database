📌 Student Club Membership & Activity Management System
🔍 Project Overview

This project is a relational database system developed using Microsoft Access to manage student clubs, memberships, activities, and participation records. The system supports normalized schema design (up to 3NF), SQL-based analytical queries, structured reporting, and automated query execution using macros.

🛠 Technologies Used

Microsoft Access

SQL (Access SQL)

Relational Database Design

ER Modeling

Database Normalization (1NF, 2NF, 3NF)

Macros (Automation)

🏗 Database Design

The database consists of the following tables:

Student

Club

Activity

Membership (junction table)

Participation (junction table)

Key concepts implemented:

Primary & Foreign Keys

One-to-Many Relationships

Many-to-Many Resolution

Referential Integrity

📊 Sample SQL Queries

Active Memberships

SELECT MembershipID, StudentID, ClubID, JoinDate
FROM [Membership Table]
WHERE MembershipStatus = 'Active';


Count Members Per Club

SELECT [Club Table].ClubName,
COUNT([Membership Table].StudentID) AS NumberOfMembers
FROM [Membership Table]
INNER JOIN [Club Table]
ON [Membership Table].ClubID = [Club Table].ClubID
GROUP BY [Club Table].ClubName;

📈 Reports Generated

Membership Details Report

Participation Summary Report

Activity Attendance Report

Club Popularity Analysis

⚙ Automation

Macros were implemented to automate query execution and reporting workflows using the OpenQuery action.

🎯 Key Skills Demonstrated

Relational Database Modeling

SQL Query Development

Data Normalization

Business Reporting

Front-End Form Design

Workflow Automation
