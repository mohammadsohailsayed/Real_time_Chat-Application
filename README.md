# Real_time_Chat-Application

Overview

This project is a minimal chat application built for daily use, leveraging Google Cloud technologies. Users can log in using their Gmail credentials, search for other users, add them to their friend list, and start chatting immediately.

Features

Google Authentication: Users authenticate using their Gmail accounts.
Real-Time Messaging: Send and receive messages in real-time.
Notifications: Cloud messaging ensures users receive notifications even when the app is not open.
Cloud Storage/Firestore: Persistent data storage for future retrieval.
AppEngine Deployment: Host the application on Google Cloud’s AppEngine for public access.
Components

AppEngine
Google Authentication Provider
Cloud Functions
Cloud Storage/Firestore
Cloud Messaging
Architecture

This chat application follows the Model-View-Controller (MVC) architecture:

Model: Manages data, logic, and application rules.
View: The user interface, reflecting data managed by the model.
Controller: Handles user interactions and updates both the view and model.
Message Flow
A user sends a message.
A Cloud Function is triggered, processing the message and storing it in Cloud Storage or Firestore.
Cloud Messaging notifies the receiving user, even if the app is closed.
Technology Stack

Frontend: Built with React.js and styled using TailwindCSS.
Backend: Node.js and Express.js for creating RESTful APIs and Cloud Functions.
Google Authentication Provider: Secures the app using OAuth 2.0.
Cloud Functions: Processes messages and triggers services without requiring a server.
Cloud Storage/Firestore: Stores messages and other data securely.
Cloud Messaging: Sends notifications to users about new messages.
Implementation Plan

Frontend: Develop the user interface using React.js and TailwindCSS.
Authentication: Integrate Google Authentication for secure user login.
Backend Logic: Implement Cloud Functions to handle messaging and data storage.
Data Persistence: Choose between Cloud Storage and Firestore for message storage.
Notifications: Set up Cloud Messaging to notify users of new messages.
Tools
Slack: Communication and collaboration for team members.
Trello: Task management, tracking deadlines, and project progress.
Test Plan

We'll host the application on AppEngine to enable user testing via a shared URL.

Future Enhancements

End-to-End Encryption: Ensure secure communication between users.
Media Support: Allow users to share images and other media.
