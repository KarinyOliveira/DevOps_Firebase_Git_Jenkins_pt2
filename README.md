# DevOps_Firebase_Git_Jenkins_pt2

This repository contains the final exam project for the **DevOps1** course, developed by **KarinyCCTB**. The project demonstrates key DevOps practices such as **Continuous Integration (CI)**, **Continuous Delivery (CD)**, **Automated Testing**, and **Containerization** using Docker, focusing on deployment automation and code quality in a real-world scenario.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Setup and Installation](#setup-and-installation)
- [Running the Application](#running-the-application)
- [Technologies Used](#technologies-used)
- [Testing](#testing)

## Project Overview

The project was designed to showcase the application of DevOps practices, including CI/CD pipelines, containerization, and automated testing. This project could be part of a larger infrastructure setup or service deployment pipeline.

### Key Features of the Project:

- **CI/CD pipeline** to automate the build, test, and deployment process.
- **Docker** for containerizing the application.
- **Automated Testing** for ensuring the quality and reliability of the code.
- **Deployment Automation** to facilitate automatic deployments to local or cloud environments.

## Features

- **CI Pipeline**: Automates building, testing, and deployment.
- **Dockerization**: Builds and runs the application in Docker containers for easier and more consistent deployment.
- **Automated Testing**: Ensures that new changes don’t break the system by running automated tests.
- **Deployment Automation**: Allows for deploying the application on any server, container, or cloud platform.
- **Scalability**: The project is designed to scale with minimal configuration changes.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Git**: For cloning the repository and managing version control.
- **Docker**: For containerization and running the application in a consistent environment.
- **Node.js** (if applicable): For running the application (if it’s a Node.js application).
- **npm or yarn**: For installing dependencies in Node.js-based applications.
- **Jenkins** (optional): For CI/CD automation.

## Setup and Installation

Follow these steps to set up and install the project:

1. **Clone the Repository**

   First, clone the repository to your local machine:

   ```bash
   git clone https://github.com/KarinyCCTB/FinalExam_DevOps1_Kariny.git
   cd FinalExam_DevOps1_Kariny
   ```

2. **Install Dependencies**

   If the application uses Node.js (or any other environment), you will need to install dependencies. For Node.js applications, run:

   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure Environment Variables**

   If the application requires any environment variables, create a `.env` file in the root of the repository or use the environment-specific configuration files.

   Example `.env` file:

   ```bash
   DATABASE_URL=mongodb://localhost:27017/devops1
   PORT=3000
   ```

4. **Run the Application in Docker (Optional)**

   If you're using Docker, you can build and run the Docker container for the application.

   ```bash
   docker build -t finalexam_devops1 .
   docker run -p 3000:3000 finalexam_devops1
   ```

   This will run the application on `http://localhost:3000`.

5. **Run the Application Locally**

   If you are not using Docker, you can run the application locally using:

   ```bash
   npm start
   ```

   The app should now be accessible at `http://localhost:3000` (or whichever port you've configured).

## Running Tests

The project includes automated tests to ensure that the code is functioning as expected. To run the tests, use:

```bash
npm test
# or
yarn test
```

This will run the test suite, ensuring that all tests pass before any deployment or integration.

## Technologies Used

- **Node.js**: JavaScript runtime for backend services (if applicable).
- **Docker**: For containerizing the application and ensuring portability.
- **Jenkins**: For automating the CI/CD pipeline (if applicable).
- **MongoDB** or other databases: Used for storing data (if applicable).
- **Jest/Mocha**: JavaScript testing frameworks for unit and integration tests.
- **GitHub Actions**: For automating the CI/CD workflows directly in GitHub (if applicable).
