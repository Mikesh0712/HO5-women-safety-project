🚀 SheSafe – Women Safety Web App

📌 Overview

SheSafe is a web-based women safety platform designed to ensure security, awareness, and community support.
It provides real-time SOS alerts, emergency contact management, resource access, and a forum for sharing experiences.
The project integrates Firebase (Auth, Firestore, Storage) and a Node.js backend (Express.js) for scalability.

✨ Features

🔐 Authentication
Secure Signup & Login using Firebase Authentication.
Session management with auto-redirect for logged-in users.

👩‍💻 Profile Management
Upload & update profile picture (avatar).
View email & username.
Manage emergency contacts: add, view, delete.

🚨 SOS Button
Global floating SOS button (red alert).
Sends emergency alerts (future:sms/whatsapp).
Automatically notifies top 3 emergency contacts + 112 helpline(currently 112 is not being notified as this is for demo and we don't want to make fake notifications).

📚 Resources
Preloaded safety resources (laws, helplines, guides).
Multi-language support via Google Translate widget.

💬 Forum
Community-driven discussion forum.
Users can post experiences, tips, and safety alerts.
Section for own posts and top posts.

🌍 Multi-language Support
Built-in Google Translate integration.
Users can select language for accessibility.

🛠 Tech Stack

🎨 Frontend

HTML, CSS, JavaScript

Responsive UI with modular CSS per page

Global common.css & common.js

⚙ Backend

Node.js + Express.js

Firebase Admin SDK for DB & Auth

APIs for users, forum, emergency contacts

☁ Database

Firebase Firestore → user profiles, emergency contacts, forum posts

Firebase Storage → profile pictures

🔮 Future Scope
>AI-powered danger zone detection (using maps + ML).

>Mobile app version (React Native).

>Live location sharing with emergency contacts(now only mock).

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

▶️ How to Run Locally

Clone this repository

Run Frontend

Open the folder in VS Code (or any editor).

Right click on index.html → Open with Live Server (or just open in browser).

Run Backend

cd backend
node src/app.js


The backend server will start on http://localhost:5000
 (or configured port).

⚠️ Note: This project is not yet deployed fully (backend not hosted). To view the clone, follow the steps above. 

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🔒 Security Note

This project uses Firebase (for authentication & database) and Twilio (for SOS emergency messaging).
For security reasons, API keys and credentials are not included in this repository.
Judges can refer to the demo video for a working showcase of the full project, and the backend can be run with valid keys provided securely if needed.
