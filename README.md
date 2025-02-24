# Online Application for Psychological Counselling

## Overview
This project is an online platform for psychological counselling, allowing users to book appointments with counsellors, communicate securely, and manage their mental health support.

## Features
- **User Authentication**: Secure signup and login using JWT.
- **User Profiles**: Clients and counsellors can manage their profiles.
- **Appointment Booking**: Clients can schedule sessions with available counsellors.
- **Messaging System**: Secure chat functionality between clients and counsellors.
- **Admin Dashboard**: Manage users, appointments, and track activity.

## Tech Stack
### Frontend:
- React.js (with Tailwind CSS for styling)
- React Router for navigation

### Backend:
- Node.js with Express.js
- JWT Authentication

### Database:
- MongoDB (via Mongoose) or PostgreSQL (via Sequelize)

### Deployment:
- Frontend: Vercel or Netlify
- Backend: Heroku or DigitalOcean
- Database: MongoDB Atlas or Railway (for PostgreSQL)

## Installation & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/psych-counselling-app.git
   cd psych-counselling-app
   ```
2. **Install dependencies:**
   ```bash
   # Frontend
   cd frontend
   npm install
   ```
   ```bash
   # Backend
   cd backend
   npm install
   ```
3. **Set up environment variables:**
   - Create a `.env` file in the backend folder and add:
     ```env
     PORT=5000
     MONGO_URI=your-mongodb-uri
     JWT_SECRET=your-secret-key
     ```
4. **Run the development servers:**
   ```bash
   # Backend
   cd backend
   npm start
   ```
   ```bash
   # Frontend
   cd frontend
   npm start
   ```

## API Routes
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | /api/auth/register | Register a new user |
| POST   | /api/auth/login | Login user and get token |
| GET    | /api/users/:id | Get user profile |
| POST   | /api/appointments/book | Book an appointment |
| GET    | /api/appointments | Get all appointments |
| POST   | /api/messages/send | Send a message |

## Folder Structure
```
psych-counselling-app/
│── frontend/       # React frontend
│── backend/        # Express.js backend
│── README.md       # Project documentation
│── .gitignore      # Ignore unnecessary files
```

## Future Enhancements
- Video/audio call integration
- AI-based mental health assessment
- Multi-language support

## Contributing
Pull requests are welcome! Please create an issue before making significant changes.

## License
This project is licensed under the MIT License.