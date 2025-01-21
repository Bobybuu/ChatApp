# Chat App

## Overview
The Chat App is a real-time messaging platform designed to facilitate seamless communication between users. It comprises a **frontend** built with modern web technologies for a responsive user interface and a **backend** that handles data persistence, authentication, and socket-based real-time messaging.

## Features
- **Real-time Chat:** Instant messaging with live updates using Socket.IO.
- **Authentication:** Secure user authentication using JWT.
- **File Uploads:** Image uploads using Cloudinary.
- **Responsive UI:** Optimized for desktop and mobile devices using Tailwind CSS.

---

## Project Architecture

### Frontend
- **Framework:** React
- **State Management:** Zustand
- **Styling:** Tailwind CSS and DaisyUI
- **Utilities:** Axios for API calls, React Router DOM for navigation, and React Hot Toast for notifications.

### Backend
- **Framework:** Express.js
- **Database:** MongoDB
- **Authentication:** JWT and bcryptjs
- **File Storage:** Cloudinary
- **Real-time Communication:** Socket.IO
- **Environment Variables:** Managed with dotenv

---

## Prerequisites
Ensure you have the following installed:
- Node.js (v16 or higher)
- npm (Node Package Manager)
- MongoDB

---

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Install Dependencies
#### Frontend
Navigate to the `frontend` directory and install dependencies:
```bash
cd frontend
npm install
```

#### Backend
Navigate to the `backend` directory and install dependencies:
```bash
cd backend
npm install
```

### 3. Configure Environment Variables
#### Backend
Create a `.env` file in the `backend` directory with the following variables:
```env
PORT=5000
MONGO_URI=<your-mongodb-connection-string>
JWT_SECRET=<your-jwt-secret>
CLOUDINARY_CLOUD_NAME=<your-cloudinary-cloud-name>
CLOUDINARY_API_KEY=<your-cloudinary-api-key>
CLOUDINARY_API_SECRET=<your-cloudinary-api-secret>
```

---

## Usage

### 1. Start the Backend Server
Navigate to the `backend` directory and run:
```bash
npm run dev
```
The backend server will start on `http://localhost:5000`.

### 2. Start the Frontend Server
Navigate to the `frontend` directory and run:
```bash
npm run dev
```
The frontend server will start, typically on `http://localhost:5173`.

### 3. Access the Application
Open your browser and navigate to `http://localhost:5173` to use the Chat App.

---

## File Structure

### Frontend
```
frontend/
|-- src/
    |-- components/   # React components
        |-- pages/        # Page components
            |-- hooks/        # Custom hooks
                |-- store/        # Zustand state management
                    |-- App.jsx       # Main app component
                        |-- index.jsx     # Entry point
                        ```

                        ### Backend
                        ```
                        backend/
                        |-- src/
                            |-- controllers/  # Business logic
                                |-- models/       # Mongoose schemas
                                    |-- routes/       # API routes
                                        |-- utils/        # Utility functions
                                            |-- index.js      # Entry point
                                            ```

                                            ---

                                            ## Additional Scripts

                                            ### Frontend
                                            - **Development Mode:** `npm run dev`
                                            - **Build for Production:** `npm run build`
                                            - **Preview Build:** `npm run preview`
                                            - **Linting:** `npm run lint`

                                            ### Backend
                                            - **Development Mode:** `npm run dev`
                                            - **Start Server:** `npm run start`

                                            ---

                                            ## Contributing
                                            Contributions are welcome! Please fork the repository and submit a pull request with your changes.

                                            ---

                                            ## License
                                            This project is licensed under the MIT License. See the LICENSE file for details.


