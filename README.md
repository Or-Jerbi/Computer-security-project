# Computer Security Project

## Overview

This project focuses on developing a browser-based application with robust security measures against common web vulnerabilities, specifically Cross-Site Scripting (XSS) and SQL Injection (SQLi) attacks. It includes both server-side and client-side protections to provide a full-stack security approach.

## Features

- **XSS Protection**: Input sanitization and output encoding to block malicious scripts.
- **SQL Injection Defense**: Use of parameterized queries to prevent unauthorized database access.
- **User Authentication**: Secure login system with proper session handling.
- **MVC Architecture**: Clean and organized code structure for scalability and maintainability.

## Technologies Used

- **Backend**: Node.js, Express.js  
- **Frontend**: HTML, CSS, JavaScript, EJS  
- **Database**: MySQL  
- **Security Tools**: [Helmet](https://www.npmjs.com/package/helmet), [express-validator](https://www.npmjs.com/package/express-validator)

## Installation

- Clone the repository:
  ```bash
  git clone https://github.com/Or-Jerbi/Computer-security-project.git
  cd Computer-security-project
  npm install

- Create a .env file in the root directory with the following variables:
  ```bash
  DB_HOST=your_database_host
  DB_USER=your_database_user
  DB_PASSWORD=your_database_password
  DB_NAME=your_database_name
  SESSION_SECRET=your_session_secret


 - Set up your MySQL database and import the schema/data from the db directory if provided.
 - Start the server:
   ```bash
   npm start
   
 - Access the application at http://localhost:3000.


## Usage

- Open your browser and go to `http://localhost:3000`.
- Register a new user or log in with existing credentials.
- Try inputting potentially malicious scripts (e.g., `<script>alert("XSS")</script>`) or SQL injection attempts (`' OR 1=1--`) to see how the application handles them.
- Observe how the backend and frontend work together to sanitize inputs and prevent attacks.
- Use this environment to test, learn, or demonstrate basic web security practices.

## Project Structure
   ```bash
    Computer-security-project/
    ├── public/             # Static assets
    ├── routes/             # Route definitions
    ├── views/              # EJS templates
    ├── .env                # Environment config
    ├── auth.js             # Auth middleware
    ├── db-config.js        # DB connection setup
    ├── server.js           # App entry point
    ├── package.json
