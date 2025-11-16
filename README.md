# Blood-Bank

**Project Description**

The Blood Bank is a full-stack web application designed to streamline the process of managing blood donations and requests. It allows users to register as donors or recipients, manage donation records, and search for available blood types. The application provides complete CRUD (Create, Read, Update, Delete) functionality. Built using the MERN stack, the system ensures real-time updates, responsive design, and secure data handling.

**Technical Decisions and Overview**
**Frontend**
* Framework: React.js for building a responsive, component-based user interface.
* Responsive Design: CSS media queries ensure compatibility across desktop, tablet, and mobile devices.
* User Interface: Intuitive UI that allows users to register, log in, and manage donation or request records.
* State Management: Utilizes React Hooks like useState and useEffect for dynamic state handling.
* Error Handling: Client-side form validations for correct input (e.g., valid blood types, phone numbers).

**Backend**
* Framework: Node.js with Express.js for building RESTful APIs and managing server-side logic.
* Database: MongoDB for storing donor and recipient data, including blood types, availability, and contact info.
* API Endpoints: Exposes RESTful routes for handling donor registration, blood search, and request management.
* Validation: Backend validation using middleware to ensure accurate and complete submissions.
* Error Handling: Structured error responses for client and server issues, ensuring a robust experience.

**Data Management**
* Database: MongoDB is used to store and manage blood donation and request records with flexible schemas.
* CRUD Operations: Allows creating, reading, updating, and deleting donor and request entries.
* Blood Search: Users can search available blood types and donors based on their city or blood group.

**Setup Instructions**
**Prerequisites**
* Node.js
* MongoDB


**Installation**
* Clone the Repository
  ```bash
  git clone https://github.com/Mehaksinghal2/blood-bank.git
  cd blood-bank
  ```
* Install Server Dependencies
  ```bash
  npm install
  ```
* Install Client Dependencies
  ```bash
  cd ../client
  npm install
  ```
* Configure Environment Variables
  * Create a .env file in the backend folder:
    ```bash
    PORT=PORT = 8080
    MONGODB_URI = mongodb://localhost:27017/blood-bank
    JWT_SECRET = your_jwt_secret_key
    ```
* Start MongoDB
Ensure MongoDB is running locally or configure your MONGODB_URI appropriately.
* Run the Backend Server
  ```bash
  cd ..
  npm start
  ```
  * Server runs at http://localhost:8080
 
* Run the Frontend
  ```bash
  cd client
  npm start
  ```
  * Frontend runs at http://localhost:3000

**Project Structure**
**Backend**
* Routes: /donors, /requests, /auth, etc.
* Controllers: Contains logic for creating, updating, deleting donor/request records.
* Database Models: Mongoose schemas for donors and requests.
* Middleware: Authentication, input validation, and error handling.

**Frontend**
* Components:
  * RegisterForm: For new donor/recipient sign-up
  * SearchBlood: For users to search available blood.
  * Dashboard: For viewing and managing blood records.
* Routing: React Router for navigation between components.
* State Management: Hooks used for managing UI and API responses.
* Validation: Form validation for critical fields like name, blood type, and contact info.

**Running Tests**
* Use tools like Postman or Thunder Client to test API endpoints.
* For frontend, use React Testing Library or Jest (optional setup).

**Features** 
* User Registration: Donors and recipients can register with their details.
* Blood Search: Find donors based on city and blood group.
* CRUD Operations: Add, update, and delete donor/request entries.
* Responsive Design: Works on all screen sizes.
* Authentication (planned): For secure donor/recipient management.
* Real-Time Updates: Immediate reflection of added or updated records.
* Error Feedback: Friendly error messages for users and developer logs in console.

**Future Enhancements**
* Authentication & Authorization: Secure login and dashboard access.
* Email & SMS Notifications: Notify users when a matching donor/request is found.
* Geo-Search: Filter donors based on location proximity.
* Admin Panel: Manage system users and records.
* Mobile App: Native app for Android and iOS for wider access.
* Donation History Tracking: Let donors and recipients view past activity.

**Screen Shots**
<img width="1440" height="813" alt="Image" src="https://github.com/user-attachments/assets/9539e7e0-9221-425e-b53a-6d79335d7421" />

<img width="1440" height="813" alt="Image" src="https://github.com/user-attachments/assets/89ee08d8-aced-42af-9684-633b21c2f556" />

<img width="1440" height="813" alt="Image" src="https://github.com/user-attachments/assets/dded5bdc-bb4e-4f35-a383-c8b998a0223c" />

<img width="1440" height="813" alt="Image" src="https://github.com/user-attachments/assets/fbc66070-bac4-4e49-850e-19634bfc5b17" />

<img width="1440" height="813" alt="Image" src="https://github.com/user-attachments/assets/c74d451a-dcf7-4151-b6a1-73bf4d5e3b67" />
