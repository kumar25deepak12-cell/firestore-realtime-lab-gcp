**Firestore Real-Time Database Lab on GCP**
**Project Overview**

This project demonstrates the implementation of a real-time NoSQL database using Google Cloud Firestore in Native Mode. The lab covers database creation, collection 
and document management, and Firestore's document-based data model. The project simulates a user management application storing user profiles in a scalable and serverless database.

**Architecture Diagram**
Architecture Flow:
Mobile App / Web App
          │
          ▼
      Firestore
          │
          ▼
   users Collection
      │       │
      ▼       ▼
   user1    user2

**** Services Used********

Google Cloud Firestore
Native Mode Database
NoSQL Document Database
Real-time synchronization
Automatic scaling
Serverless architecture

**Objectives**
Understand Firestore architecture
Create a Firestore database
Create collections and documents
Learn Firestore data hierarchy
Explore real-time NoSQL database concepts
Understand Firestore use cases

**Firestore Data Model**
Firestore organizes data in the following hierarchy:

Database
   ↓
Collection
   ↓
Document
   ↓
Fields
**Example:**

firestore-realtime-db
       ↓
      users
       ↓
   ┌─────────┐
   │ user1   │
   │ user2   │
   └─────────┘



   Step-by-Step Implementation**
   
Step 1: Create GCP Project

firestore-realtime-lab

Step 2: Open Firestore
Google Cloud Console
   ↓
Firestore

Step 3: Configure Firestore
Edition: Standard
Mode: Native Mode
Region: asia-south1
Security Rules: Open

Step 4: Create Collection
Collection ID: users

Step 5: Create Document user1
{
  "name": "Deepak",
  "role": "Architect",
  "experience": 5
}
Step 6: Create Document user2
{
  "name": "Rahul",
  "role": "Developer",
  "experience": 3
}
Step 7: Verify Documents
users
 ├── user1
 └── user2

 **Collections and Documents**
 
**Collection: users**

Document: user1
Field	Value
name	Deepak
role	Architect
experience	5

Document: user2
Field	Value
name	Rahul
role	Developer
experience	3

**Key Learnings**

Firestore is a NoSQL document database
Data is organized into collections and documents
Firestore supports real-time synchronization
Firestore automatically scales based on demand
Firestore is serverless and highly available
Firestore integrates well with mobile and web applications

**Firestore vs Cloud SQL**

| Feature        | Firestore      | Cloud SQL             |
| -------------- | -------------- | --------------------- |
| Database Type  | NoSQL          | Relational            |
| Schema         | Flexible       | Fixed                 |
| Scaling        | Automatic      | Vertical/Managed      |
| Real-time Sync | Yes            | No                    |
| Mobile Apps    | Excellent      | Moderate              |
| SQL Queries    | No             | Yes                   |
| Best Use Case  | Real-time apps | Transactional systems |

**What is the Firestore hierarchy?**
Database
   ↓
Collection
   ↓
Document
   ↓
Fields

**Firestore vs Cloud SQL?**
Firestore is a NoSQL document database for real-time applications, while Cloud SQL is a relational database for transactional workloads.

**What are common Firestore use cases?**

Chat Applications
Social Media Platforms
Mobile Applications
User Profile Management
Real-time Collaboration Tools
Production Improvements

**For production environments:**

Enable restrictive security rules
Implement Firebase Authentication
Use IAM least-privilege access
Enable audit logging
Configure backup and recovery
Use multi-region deployment for critical workloads
Monitor usage and performance

**Final Outcome**
Successfully deployed a Firestore Native Mode database on Google Cloud Platform and created a real-time NoSQL data model using collections, documents, and fields. 
The project demonstrates Firestore architecture, document hierarchy, and scalable application design principles suitable for modern web and mobile applications.**
