# Real-Time Location Tracking System

A comprehensive real-time location tracking system with user and admin interfaces.

## Features

- **User Registration and Login**: Secure authentication using JWT.
- **Real-time GPS Location Tracking**: Tracks user location every 4 seconds.
- **Admin Dashboard**: Monitors all registered users in real-time.
- **Location History**: Detailed records of user locations.
- **WebSocket Integration**: Enables live updates for seamless tracking.

## Tech Stack

- **Backend**: Node.js, Express, MongoDB
- **Frontend**: React, Material-UI, Socket.io-client
- **Database**: MongoDB Atlas
- **Real-time Communication**: Socket.io
- **Authentication**: JWT

## Setup

### Backend

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file and add the following environment variables:
   ```env
   MONGODB_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   PORT=3002
   ```

4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file and add the following environment variable:
   ```env
   REACT_APP_API_URL=http://localhost:3002 # or production URL
   ```

4. Start the frontend server:
   ```bash
   npm start
   ```

## API Endpoints

### Authentication
- `POST /auth/register`: User registration
- `POST /auth/login`: User login

### Location
- `POST /location/update`: Update user location
- `GET /location/history/:userId`: Get location history for a specific user

### Admin
- `GET /admin/users`: Fetch all users for admin monitoring

## Production URLs

- **Backend**: [https://ashu-az-live-location-tracking-system.onrender.com](https://ashu-az-live-location-tracking-system.onrender.com)
- **Frontend**: [Your Frontend URL]

## Directory Structure

```plaintext
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   └── app.js
└── frontend/
    ├── src/
    │   ├── components/
    │   └── App.js
```

## Testing

1. Use the `test-client.html` file to simulate location updates.
2. The admin dashboard displays real-time locations of all users.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to enhance this README with additional details as needed!
