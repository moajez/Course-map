# Mini Course Planner

A full-stack course planning application built with React (TypeScript) and Express.js that helps educators plan their courses, manage syllabi, and organize teaching schedules.

## Features

- 🔐 User Authentication (JWT-based)
- 📚 Course Planning and Management
- 📅 Interactive Date Selection
- 📋 Syllabus Management
- 🗓️ Teaching Schedule Organization
- 🔄 Flexible Date Filtering

## Tech Stack

### Frontend
- React 18 with TypeScript
- Material UI (MUI) for components
- Vite for build tooling
- React Router for navigation
- Date-fns for date manipulation

### Backend
- Express.js with TypeScript
- MongoDB with Mongoose ODM
- JWT for authentication
- bcrypt for password hashing

## Prerequisites

- Node.js (v16 or higher)
- MongoDB (v6 or higher)
- npm or yarn

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd course-map
   ```

2. **Set up the backend**
   ```bash
   cd backend
   npm install
   
   # Create .env file with:
   # MONGO_URI=mongodb://localhost:27017/course-map
   # JWT_SECRET=your_jwt_secret
   # PORT=5001
   
   npm run dev
   ```

3. **Set up the frontend**
   ```bash
   cd frontend
   npm install
   
   # Create .env file with:
   # VITE_API_BASE_URL=http://localhost:5001
   
   npm run dev
   ```

4. **Access the application**
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:5001

## Project Structure

```
├── frontend/               # React frontend
│   ├── src/
│   ├── public/
│   └── package.json
├── backend/                # Express backend
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   └── server.ts
│   └── package.json
└── README.md
```

## API Endpoints

### Authentication
- POST `/api/users/register` - Register new user
- POST `/api/users/login` - User login

### Syllabus Management
- POST `/api/syllabus` - Create/update syllabus
- GET `/api/syllabus/courses` - List all courses
- GET `/api/syllabus/:courseName` - Get course details

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.
