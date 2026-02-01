🚌 Ebus Management Based Current Location System

Domain: Transportation / Intelligent Transportation Systems
Technologies: HTML, CSS, JavaScript, Firebase (Authentication & Firestore)
Project Type: Web Application (Client-side with Firebase backend)

📌 Project Overview

The Ebus Management Based Current Location System is a web application that provides real-time bus location and arrival information to travelers. It uses Firebase for authentication and data storage and supports role-based access for Admin (Staff), Driver, and User (Traveler).

🎯 Objectives

Provide real-time bus location and arrival updates

Reduce passenger waiting uncertainty

Enable role-based access and secure data handling

Support efficient public transport management

👥 User Roles
👑 Admin / Staff

Login using email & password

Create and manage driver accounts

Add and manage buses and routes

View system data (admin privileges)

🧑‍✈️ Driver

Login with assigned credentials

Update bus current location

Update arrival and linger time

🧍 User (Traveler)

Register and login

Search buses by source and destination

View bus location and arrival time (read-only)

🏗️ System Architecture

Frontend: HTML, CSS, JavaScript

Authentication: Firebase Email/Password Auth

Database: Firebase Firestore

Security: Firestore Rules with role-based access

🧪 Test Cases

🔐 Authentication

| Test Case ID | Description                        | Expected Result  |
| ------------ | ---------------------------------- | ---------------- |
| TC-AUTH-01   | Admin login with valid credentials | Login successful |
| TC-AUTH-02   | Login with invalid password        | Error message    |
| TC-AUTH-03   | Unregistered email login           | Access denied    |

👑 Admin / Staff

| Test Case ID | Description                    | Expected Result |
| ------------ | ------------------------------ | --------------- |
| TC-ADM-01    | Admin dashboard access         | Dashboard loads |
| TC-ADM-02    | Non-admin accessing admin page | Access denied   |
| TC-ADM-03    | Create driver account          | Driver created  |

🧑‍✈️ Driver
| Test Case ID | Description                 | Expected Result  |
| ------------ | --------------------------- | ---------------- |
| TC-DRV-01    | Driver login                | Login successful |
| TC-DRV-02    | Update bus location         | Location updated |
| TC-DRV-03    | Driver accessing admin page | Access denied    |

🧍 User

| Test Case ID | Description         | Expected Result   |
| ------------ | ------------------- | ----------------- |
| TC-USER-01   | User registration   | Account created   |
| TC-USER-02   | User login          | Login successful  |
| TC-USER-03   | Search bus route    | Results displayed |
| TC-USER-04   | User modifying data | Access denied     |

🔒 Security

Firebase Authentication ensures secure access

Firestore rules enforce role-based permissions

Unauthorized reads/writes are blocked

📊 Conclusion

This project demonstrates an effective real-time bus tracking system using Firebase services. It ensures secure role-based access, improves public transport usability, and can be extended with GPS integration and mobile support.
