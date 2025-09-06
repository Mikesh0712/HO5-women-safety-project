# README for Women Safety Platform Backend

## Overview
This backend service is designed to support the Women Safety Platform, providing functionalities such as user authentication, emergency contact management, and SOS alert services. It integrates with Firebase for real-time data storage and messaging services.

## Features
- User authentication using Firebase Authentication
- Management of emergency contacts
- SOS alert system that sends notifications to emergency contacts
- Integration with Firebase Firestore for data storage
- SMS service for sending alerts

## Getting Started

### Prerequisites
- Node.js (version 14 or higher)
- Firebase account and project setup
- A valid Twilio account (if using SMS service)

### Installation
1. Clone the repository:
   ```
   git clone <repository-url>
   ```
2. Navigate to the backend directory:
   ```
   cd backend
   ```
3. Install the dependencies:
   ```
   npm install
   ```

### Configuration
1. Create a `.env` file in the root directory and add the following environment variables:
   ```
   FIREBASE_API_KEY=<your-firebase-api-key>
   FIREBASE_AUTH_DOMAIN=<your-firebase-auth-domain>
   FIREBASE_PROJECT_ID=<your-firebase-project-id>
   FIREBASE_STORAGE_BUCKET=<your-firebase-storage-bucket>
   FIREBASE_MESSAGING_SENDER_ID=<your-firebase-messaging-sender-id>
   FIREBASE_APP_ID=<your-firebase-app-id>
   TWILIO_ACCOUNT_SID=<your-twilio-account-sid>
   TWILIO_AUTH_TOKEN=<your-twilio-auth-token>
   TWILIO_PHONE_NUMBER=<your-twilio-phone-number>
   ```

### Running the Application
To start the server, run:
```
node src/app.js
```
The server will start on the specified port (default is 5000).

### API Endpoints
- **POST /send-sos**: Sends an SOS alert to the user's emergency contacts.
- **GET /contacts**: Retrieves the user's emergency contacts.
- **POST /contacts**: Adds a new emergency contact.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License
This project is licensed under the MIT License. See the LICENSE file for details.