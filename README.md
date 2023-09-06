# login_app
Complete MERN App (OTP Verification, JWT Token, Authentication, Reset Password)
# Complete MERN Login (OTP Verification, JWT Token, Authentication, Reset Password)

This repository contains a complete MERN (MongoDB, Express.js, React.js, Node.js) authentication system with OTP (One-Time Password) verification, JWT (JSON Web Token) token-based authentication, and password reset functionality. This README file will guide you through setting up and using this authentication system.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Features
- User registration with email and password.
- User login with email and password, with JWT token-based authentication.
- OTP verification during user registration.
- Password reset functionality with OTP verification.
- Secure password hashing with bcrypt.
- Customizable JWT token expiration time.
- Express.js API backend with MongoDB for data storage.
- React.js frontend for user interaction.

## Prerequisites
Before you begin, ensure you have met the following requirements:

- [Node.js](https://nodejs.org/) installed on your development machine.
- [MongoDB](https://www.mongodb.com/) installed and running locally or accessible via a remote URL.
- A valid SMTP email server configuration for sending OTP emails during registration and password reset (e.g., [SendGrid](https://sendgrid.com/), [Mailgun](https://www.mailgun.com/), or a custom SMTP server).

## Installation
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/mern-login-otp.git
   ```

2. Navigate to the project directory:
   ```bash
   cd mern-login-otp
   ```

3. Install the backend dependencies:
   ```bash
   cd backend
   npm install
   ```

4. Install the frontend dependencies:
   ```bash
   cd ../frontend
   npm install
   ```

## Usage
Follow these steps to run the MERN authentication system:

1. Configure the application (see [Configuration](#configuration) section).
   
2. Start the backend backend:
   ```bash
   cd backend
   npm start
   ```

3. Start the frontend development backend:
   ```bash
   cd ../frontend
   npm start
   ```

4. Open your web browser and visit `http://localhost:3000` to access the application.

## Project Structure
The project structure is organized as follows:

- `backend`: Contains the Express.js API backend.
- `frontend`: Contains the React.js frontend.
- `config`: Configuration files for the backend and frontend.
- `controllers`: Controllers for handling user registration, login, OTP verification, and password reset.
- `models`: MongoDB schema models.
- `routes`: API routes for user authentication.
- `utils`: Utility functions for sending emails, generating OTPs, and JWT token handling.

## Configuration
To configure the application, you need to update the configuration files in the `config` directory:

- `config/default.json`: Contains default configuration settings.
- `config/development.json`: Contains development-specific configuration settings.
- `config/production.json`: Contains production-specific configuration settings.

You should provide the following configuration parameters:

- `mongoURI`: MongoDB connection URI.
- `jwtSecret`: Secret key for JWT token generation.
- `jwtExpiration`: JWT token expiration time (e.g., "1h" for 1 hour).
- `email`: Email server configuration (SMTP or other email services).
- `frontendURL`: URL where the frontend is hosted (e.g., "http://localhost:3000" during development).

## Contributing
Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please create an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.