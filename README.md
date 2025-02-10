# Plant Photo App 🌱

## Overview
The **Plant Photo App** is a mobile application built using **React Native (Expo)** with a **Node.js backend** and **MongoDB** for storage. It allows users to capture and save photos of plants, providing names and optional notes. The app features a clean and modern UI with intuitive navigation.

## Features

### 🌿 List View (Mandatory)
- Displays a list of added plants.
- Shows the plant's name and the date it was added.
- A button to add a new plant, navigating to the Scan View.

### 📷 Scan View (Mandatory)
- Allows users to take a photo of a plant.
- Users can provide a name and optional notes.
- Once saved, the plant appears in the List View.

### 🔍 Detail View (Optional)
- Users can view and edit the plant's details (name, photo, and notes).

### 🧭 Navigation
- **List Tab**: Displays all plants and allows adding new ones.
- **Settings Tab**: Placeholder for settings (empty view).
- **Profile Tab**: Placeholder for user profile (empty view).

## Tech Stack
- **Frontend:** React Native (Expo)
- **Backend:** Node.js with Express
- **Database:** MongoDB (Mongoose for schema management)
- **State Management:** React Context API
- **Navigation:** React Navigation (Bottom Tabs)
- **Storage:** MongoDB for persistent data storage

## Installation & Setup

### Prerequisites
Ensure you have the following installed:
- **Node.js** (>= 14.x)
- **Expo CLI** (`npm install -g expo-cli`)
- **MongoDB** (Locally or via a cloud provider like MongoDB Atlas)

### Backend Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/muiux/plant_photo.git
   cd plant_photo/backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Open a `.env` file and configure it with your IP address:
   ```sh
   APP_ORIGIN = <Your IP Address>
   ```
4. Start the backend server:
   ```sh
   npm run dev
   ```
### Frontend Setup
1. Clone the repository:
   ```sh
   cd ../frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the backend server:
   ```sh
   npm run start
   ```
4. Scan the QR code with your device (Expo Go app) or run on an emulator.

## ScreenShots



## API Endpoints

| Method  | Endpoint         | Description           |
|---------|------------------|-----------------------|
| GET     | plant/getlist    | Get all plants        |
| POST    | plant/add        | Add a new plant       |
| PATCH   | plant/update     | Update plant details  |
| DELETE  | plant/plants/:id | Delete a plant        |

# Technical Decisions

## 1. React Native with Expo
- **Reason for Choosing**: 
  React Native with Expo was chosen to enable fast development and ease of testing. Expo provides a comprehensive set of tools that simplify the development process and minimize configuration time. It also makes it easy to deploy applications to both iOS and Android devices simultaneously.

## 2. MongoDB
- **Reason for Choosing**: 
  MongoDB was selected for its flexibility and scalability. It is a NoSQL database that handles large volumes of unstructured or semi-structured data efficiently, allowing the project to scale as needed. MongoDB’s flexible schema design also supports rapid iteration and change, which is beneficial for the evolving nature of app development.

## 3. React Context API
- **Reason for Choosing**: 
  React Context API was used for lightweight state management across the application. It is particularly useful in smaller to medium-sized projects where complex state management libraries like Redux may be overkill. The Context API provides a simple and clean way to pass data between components without prop drilling.

## 4. React Navigation
- **Reason for Choosing**: 
  React Navigation was chosen for simplifying multi-screen navigation in the application. It is easy to integrate, flexible, and well-suited for creating navigation between different screens with minimal setup. React Navigation offers a simple API and allows customization to fit the project’s requirements.

