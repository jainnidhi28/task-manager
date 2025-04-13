# Task Manager Application

A full-stack task management application built with React and FastAPI.

## Features

- User Authentication
- Create, Read, Update, and Delete tasks
- Mark tasks as complete/incomplete
- Responsive design
- Real-time updates
- Clean and intuitive UI

## Tech Stack

### Frontend
- React (Hooks)
- React Router
- Axios for API calls
- React Icons
- CSS-in-JS for styling

### Backend
- FastAPI
- Python
- JSON file storage
- CORS middleware

## Setup Instructions

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:
   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

5. Start the backend server:
   ```bash
   uvicorn main:app --reload
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd task-manager-frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

## API Documentation

### Authentication
- `POST /login` - Login with username
- `POST /register` - Register new user

### Tasks
- `GET /tasks/{username}` - Get all tasks for a user
- `POST /tasks` - Create a new task
- `PUT /tasks/{task_id}` - Update a task
- `PUT /tasks/complete/{task_id}` - Toggle task completion
- `DELETE /tasks/{task_id}` - Delete a task

## Deployment

### Backend Deployment
1. Install required packages:
   ```bash
   pip install fastapi uvicorn
   ```

2. Start the production server:
   ```bash
   uvicorn main:app --host 0.0.0.0 --port 8000
   ```

### Frontend Deployment
1. Build the production version:
   ```bash
   npm run build
   ```

2. Deploy the build folder to your hosting service

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License
This project is licensed under the MIT License.

