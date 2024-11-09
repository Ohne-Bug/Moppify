# Moppify

Mopify is a smart IoT solution designed to streamline the process of tracking and managing mopping activities, utilizing a user-friendly frontend, a robust backend, and an IoT component with an NFC reader. The project includes:

- A Vite-powered frontend for fast, interactive user experiences. 
- A Python Flask backend that handles API requests and data management.
- TinyDB, a lightweight, document-oriented database, for quick data storage and retrieval.
- An IoT integration with an NFC reader for capturing and managing data from mop usage in real-time.

## Table of Contents

- Features
- Technologies Used
- Project Structure
- Installation
- Usage
- License

## Features

Real-Time Data Collection: Use an NFC reader to capture data from mops or cleaning stations.
Responsive Frontend: Built with Vite for seamless, fast user interactions.
Lightweight Data Storage: TinyDB for easy-to-manage data storage and retrieval.
API Management: Flask API for connecting frontend, backend, and IoT devices.

## Technologies Used

Frontend: Vite
Backend: Python Flask
Database: TinyDB
IoT: NFC reader integration ()
CV: ESP32 cam with Motion Recognition

Project Structure

```
Mopify/
├── frontend/
│   ├── src/
│   ├── public/
│   └── vite.config.js
├── backend/
│   ├── app.py
│   ├── database.json
│   └── requirements.txt
├── iot/
│   └── MoppifyIOT.ino 
├── cv/
│   └── ESPMotionDetection.ino
└── README.md
```

## Installation
### Prerequisites

- Node.js and npm for the frontend
- Python 3.8+ and pip for the backend

### Frontend Setup (Vite)

Navigate to the frontend folder:

```cd frontend```

Install dependencies:

```npm install```

Start the frontend development server:

```npm run dev```

### Backend Setup (Flask & TinyDB)

Navigate to the backend folder:

```cd backend```

Create and activate a virtual environment:

```
python3 -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate
```

Install dependencies:

```pip install -r requirements.txt```

Run the Flask server:

 ```python app.py```

Usage

Start the Frontend and Backend Servers:
    Run `npm run dev` from the frontend folder to start the Vite frontend server.
    Run `python app.py` from the backend folder to start the Flask API.
Use the NFC Reader:
    When a user NFC tag is scanned by a reader on a cart, such cart will be assigned to the corresponding user. Any subsequent 
Access Mopify:
    Open your browser and navigate to the frontend URL provided by Vite (usually `http://localhost:5173`).
    Use the application interface to view, manage, and analyze mop data.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
