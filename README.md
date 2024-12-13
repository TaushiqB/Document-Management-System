# Document-Management-System
 
To execute: Run dms.py and copy paste the address in browser

## Technologies Used
- **Flask**: Backend web framework.
- **SQLAlchemy**: ORM for database interaction.
- **Redis & RQ**: Background job processing.
- **Elasticsearch**: Full-text search capabilities.
- **Flask-Mail**: For sending email notifications and attachments.
- **Flask-Babel**: Localization and translation support.
- **JWT**: For secure user sessions.
- **Microsoft Cognitive Services**: Text translation via the Translator API.

## Description

This is a full-featured Flask web application designed to manage a variety of tasks, users, posts, and approvals within a dynamic environment. The application allows user authentication, role-based access, content management, real-time messaging, task tracking, and integration with external services. Built with Flask and powered by a combination of technologies such as SQLAlchemy, Redis, Elasticsearch, Flask-Mail, and Microsoft Cognitive Services, this app offers a seamless experience for both users and administrators.

# Primitive Process:

-All the Institutes/ Departments under the Ministry are using some common file/document movement and approval procedures. The physical movement of such files/ documents has many disadvantages.
-When a document file is under process of approval, the location of the file document where it has been delayed on the way while moving from table to table, is very difficult to trace. The status of a document/ file which has been initiated is not traceable until it returns back to the parent section/ Office.


# Object Model: 

-Web server based on Flask
-Template engine based on Jinja
-Database integration based on SQL Alchemy


# Process: 

-Created a server using python
-Created a User-friendly environment(webpage) for forwarding, rejection/ approval of documents/ files in e-format
-Updation of document approval status to the end user which promotes the right to information and transparency
-Creating a messages section for direct messaging the end user/ government officers for the more info about rejection.


# Hierarchy of approval:

Tahsildar
Head Quarter's Deputy Tahsildar(HQDT)
Regional Inspector (RI)
Village Administrative Officer(VAO)

## Features

### User Management
- **Authentication**: Users can register, log in, and manage their account information.
- **Role-based Access**: Different roles are available, allowing for restricted access based on user responsibilities.
- **Password Security**: Uses hashed passwords for secure authentication.

### Post Management and Approval Workflow
- **Post Submission**: Users can submit posts for approval.
- **Approval Workflow**: Posts go through various stages of approval (by VAO, Tahsildar, HQDT).
- **Dynamic Post Approvals**: Administrators or authorized users can approve/reject posts based on various criteria.

### Task Management
- **Task Creation**: Users can create tasks with descriptions.
- **Background Processing**: Tasks are processed in the background using Redis and RQ (Real-Time Queue).
- **Progress Tracking**: Real-time updates of task progress are provided to users.
- **Task Notifications**: Users are notified when tasks are completed or updated.

### Messaging and Notifications
- **Messaging System**: Send and receive messages between users.
- **Notifications**: Real-time notifications are sent to users for important events like task updates or new messages.

### Search Functionality
- **Full-text Search**: Users can search for posts using Elasticsearch, allowing quick and relevant results from large datasets.
- **Customizable Search**: Developers can easily extend search capabilities to other models.

### Email Integration
- **Email Notifications**: Users receive email notifications for different events, such as post export or account activities.
- **Post Export**: Users can export their posts as JSON files via email.
- **Custom Email Templates**: The application supports customizable email content.

### Localization and Translation
- **Multi-language Support**: Integrated with Flask-Babel for easy localization.
- **Text Translation**: Microsoft Cognitive Services API is used to translate content between languages.

### Asynchronous Operations
- **RQ for Background Jobs**: Tasks like post export or heavy processing are handled asynchronously without blocking the main application.
- **Task Progress**: Real-time task progress updates via the RQ background job queue.


# End User/ Government Officer Experience:
 
-Register in the webpage
-Log in to the webpage
-Customized profile is created
-Files displayed in “documents” section
-File Options:
-Download and View
-Rejection/Approval
-Reason for rejection
-Send and receive private message to/from the end user/government officers
-Log out


# E-file:

-There is no chance of missing files, even if they are missed, they can be re-transmitted
-Individual cannot access files since they are securely stored in server’s database
-Secured protocols ensure prevention of tampering of documents
-There is abundance of storage space, since cloud storage is used
-This procedure does not require attendants/ peons/ MTS personnel for the movement of files

## Installation

### Prerequisites
- Python 3.8+
- pip
- Redis Server
- Elasticsearch
