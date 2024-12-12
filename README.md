# Chat_Application_Java

This is a Java-based chat application that allows users to communicate with each other in real-time, with a focus on group chats, one-on-one messaging, and user authentication. The application features a clean, modern UI with a WhatsApp-like experience, including a contact list, chat history, and real-time messaging.

Features
User Authentication: Login page with username and password validation, stored in a MySQL database.
One-on-One Messaging: Users can select contacts and chat with them, with message bubbles and timestamps.
Group Chat Functionality: Create groups, view group members, and manage group chats.
Chat History: Previous conversations are displayed in the chat window, both for one-on-one and group chats.
Unread Messages: Unread messages are indicated by a red dot next to the contact/group.
User Interface: The UI closely resembles WhatsApp with:
Light green buttons with black text
Purple and white message bubbles with fixed spacing and rounded edges
Clear chat history and timestamps
Database Integration:
Contacts, groups, and users are stored in a MySQL database.
Group creation, joining, and deletion are reflected across all users' contact lists.

Prerequisites
Java 8 or later
MySQL
JavaFX for the UI
MySQL JDBC Driver for database connection

Installation
1. Clone the repository:
bash
Copy code
git clone <repository-url>
cd chat-application
2. Set up the MySQL database:
Create a new database:
sql
Copy code
CREATE DATABASE chat_app;
Import the necessary tables:
sql
Copy code
-- users table with hashed passwords
-- contacts, groups, and group_members tables
3. Configure the database connection:
Update the database connection details in the DatabaseConnection.java file with your MySQL username and password.
4. Run the Application:
Open the project in your preferred Java IDE (e.g., IntelliJ IDEA, VS Code).
Build and run the ChatApplication.java class to start the app.

Usage
1. Login:
Enter your username and password to log in. If you don't have an account, create one via the registration form (if applicable).
2. Chat with Contacts:
From the contact list, select a contact to begin chatting. Messages will appear in bubbles with timestamps.
3. Group Chat:
Create a new group by selecting contacts and naming the group. You can view group members and manage group settings after entering the group chat.
4. Leaving Groups:
Users can leave groups at any time from the group chat window.
5. View Group Members:
Inside a group chat, a button allows you to view the members of the group.
6. Delete Group:
The group member can delete the group, which will remove it from their contact list.
