# Chalkboard

Chalkboard is a full-stack web application which serves as a peer-to-peer course-based learning and instruction platform, in which users can enroll in courses as students or create courses as instructors.

This project was developed as part of CSC 33600 - Introduction to Database Systems at The City College of New York.

## Screenshot

![Chalkboard Homepage](./images/landing-page.png)

## Features

- User authentication (login/register)
- Course creation and management for instructors
- Course enrollment and participation for students
- Lesson + content viewing and management
- Student dashboard
- Instructor center
- Course explorer (guest)
- Platform revenue metrics

## Technologies Used

- Frontend: React + Vite
- Backend: Express.js
- Database: MySQL
- Styling: shadcn/ui components, Tailwind CSS

## Project Structure

```
chalkboard
├── client (Frontend)
│   ├── src
│   │   ├── components
│   │   ├── lib
│   │   └── ...
│   ├── package.json
│   └── ...
└── server (Backend)
    ├── db
    │   ├── config
    │   └── models
    ├── middlewares
    ├── routes
    ├── server.js
    └── package.json
```

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/kareemv/chalkboard.git
   cd chalkboard
   ```

2. Install dependencies for both client and server:

   ```
   cd client && npm install
   cd ../server && npm install
   ```

3. Set up the MySQL database:

   - Create a new MySQL database schema for the project

4. Configure environment variables:
   - In the `server` directory, create a `.env` file with the following contents:
     ```
     DB_HOST=your_database_host
     DB_USER=your_database_user
     DB_PASSWORD=your_database_password
     DB_NAME=your_database_name
     PORT=your_database_port
     SECRET_KEY=your_secret_key_for_password_hashing
     ADMIN_KEY=your_admin_access_password
     ```

## Usage

1. Start the backend server:

   ```
   cd server
   npm start
   ```

2. Start the frontend development server:

   ```
   cd client
   npm run dev
   ```

3. Access the application in your web browser at `http://localhost:5173`

## License

This project is open source and available under the [MIT License](LICENSE).
