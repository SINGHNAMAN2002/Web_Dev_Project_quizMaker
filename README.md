# QuizMaker Project

## Overview
QuizMaker is a dynamic platform that allows users to create, participate in, and manage quizzes. This project leverages modern web technologies to provide a seamless and interactive experience for both quiz creators and participants.

## Features
- **Quiz Creation:** Users can create quizzes with multiple-choice questions and specify the correct answers.
- **Quiz Participation:** Participants can attempt quizzes and receive immediate feedback on their scores.
- **User Authentication:** Secure login and registration for quiz creators and participants.
- **Responsive Design:** Optimized for both desktop and mobile devices.

## Tech Stack
- **Frontend:**
  - Next.js
  - React.js
  - CSS Modules / Tailwind CSS (if applicable)
- **Backend:**
  - Node.js
  - Express.js
- **Database:**
  - MongoDB
- **Authentication:**
  - JSON Web Tokens (JWT)
- **State Management:**
  - Context API / Redux (if applicable)

## File Structure
### Frontend
- `pages/`: Contains all Next.js page components.
- `components/`: Reusable React components (e.g., quiz forms, result modals).
- `styles/`: Contains CSS/SCSS modules for styling.

### Backend
- `routes/`: API routes for handling quiz and user-related operations.
- `models/`: Mongoose schemas for MongoDB collections.
- `middleware/`: Authentication middleware.
- `server.js`: Main server entry point.

## Setup Instructions
### Prerequisites
- Node.js installed
- MongoDB instance (local or cloud, e.g., MongoDB Atlas)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/SINGHNAMAN2002/Web_Dev_Project_quizMaker.git/
   ```

2. Navigate to the project directory:
   ```bash
   cd quizmaker
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Configure environment variables:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     NEXT_PUBLIC_API_BASE_URL=http://localhost:5000
     ```

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Start the backend server:
   Navigate to the `backend/` folder and run:
   ```bash
   node server.js
   ```

7. Open the application in your browser:
   ```
   http://localhost:3000
   ```

## API Endpoints
### Authentication
- **POST** `/api/auth/register`: Register a new user.
- **POST** `/api/auth/login`: Authenticate a user and return a JWT.

### Quizzes
- **POST** `/api/quizzes`: Create a new quiz.
- **GET** `/api/quizzes`: Fetch all quizzes.
- **GET** `/api/quizzes/:id`: Fetch details of a specific quiz.
- **POST** `/api/quizzes/:id/submit`: Submit answers and calculate the score.

## Deployment
To deploy the project:
1. Use a service like Vercel for the frontend.
2. Deploy the backend on platforms like Heroku or AWS.
3. Ensure the environment variables are configured appropriately in production.

## Future Enhancements
- Add a leaderboard for quiz participants.
- Allow quiz creators to add multimedia (images/videos) to questions.
- Implement real-time updates for quiz submissions using WebSockets.

## Contributing
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For any queries or suggestions, feel free to reach out:
- **Name:** Naman Kumar Singh 
- **Email:** namankumarsingh77@gmail.com
- **GitHub:** SINGHNAMAN2002

