# [App Name] Integration Documentation

## Overview

[Description]

## Folder Structure

```
|--- src
|    |--- controllers
|    |--- database
|    |--- interfaces
|    |--- middlewares
|    |--- routes
|    |--- services
|    |--- utils
|    |--- server.ts
|--- .env
|--- app.ts
|--- .gitignore
|--- package.json
|--- tsconfig.json
```

## Dependencies (Dev)

- Node.js
- TypeScript
- Express
- ts-node-dev
- [Other dependencies]

## Getting Started

Before you begin, ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) (Node Package Manager, included with Node.js)
- [Git](https://git-scm.com/)

## Contribution Guide

## Getting Started

#### If you don't have git on your machine, [install it](https://docs.github.com/en/get-started/quickstart/set-up-git).

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the repository

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone this repository" />

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.

Open a terminal and run the following git command:

```bash
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/copy-to-clipboard.png" alt="copy URL to clipboard" />

For example:

```bash
git clone git@github.com:this-is-you/first-contributions.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.

## Create a branch

Change to the repository directory on your computer (if you are not already there):

```bash
cd first-contributions
```

Now create a branch using the `git switch` command:

```bash
git switch -c your-new-branch-name
```

For example:

```bash
git switch -c add-alonzo-church
```

### Make Changes

Make your changes to the codebase. Ensure your code follows the project's coding standards and guidelines.

### Run Tests

Run the existing tests to ensure your changes do not break anything. If you added new functionality, write corresponding tests.

```sh
npm run test
```

## commit those changes

Now open `Contributors.md` file in a text editor, add your name to it. Don't add it at the beginning or end of the file. Put it anywhere in between. Now, save the file.

<img align="right" width="450" src="https://firstcontributions.github.io/assets/Readme/git-status.png" alt="git status" />

If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add` command:

## Push changes to GitHub

Push your changes using the command `git push`:

```bash
git push -u origin your-branch-name
```

replacing `your-branch-name` with the name of the branch you created earlier.

<details>
<summary> <strong>If you get any errors while pushing, click here:</strong> </summary>

- ### Authentication Error
     <pre>remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
  remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
  fatal: Authentication failed for 'https://github.com/<your-username>/first-contributions.git/'</pre>
  Go to [GitHub's tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) on generating and configuring an SSH key to your account.

</details>

## Submit your changes for review into Staging

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/compare-and-pull.png" alt="create a pull request" />

Now submit the pull request.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/submit-pull-request.png" alt="submit pull request" />

Soon your changes will be merged into the staging branch of this project. You will get a notification email once the changes have been merged.

## Setup Instructions

### 1. Clone the Repository

First, clone the repository to your local machine using Git.

```sh
git clone https://github.com/your-username/[app-name].git
cd [app-name]
```

### 2. Install Dependencies

Navigate to the project directory and install the required dependencies.

```sh
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory of the project and add your environment-specific variables. You can use the provided `.env.example` file as a reference.

```sh
cp .env.example .env
```

Edit the `.env` file to match your environment configuration.

### 4. Compile TypeScript

Compile the TypeScript code to JavaScript.

```sh
npm run build
```

### 5. Run the Development Server

Start the development server with the following command. This will also watch for any changes in your code and automatically restart the server.

```sh
npm run start:dev
```

### 6. Run the Production Server

To run the application in a production environment, use the following command:

```sh
npm run start
```

### 7. Verify the Setup

Open your browser and navigate to `http://localhost:3000/api/v1/` to verify that the application is running correctly.

## Folder Structure

Here's an overview of the project's folder structure:

```
|--- src
|    |--- controllers
          |--- v1
|    |--- database
|    |--- interfaces
|    |--- middlewares
|    |--- routes
|         |--- v1
|    |--- services
|    |--- utils
|    |--- server.ts
|--- .env
|--- app.ts
|--- .gitignore
|--- package.json
|--- tsconfig.json
```

## Scripts

Here are some useful npm scripts that you can use during development and production:

- `npm run build`: Compiles the TypeScript code to JavaScript.
- `npm run start:dev`: Starts the development server with live reloading.
- `npm run start`: Starts the production server.
- `npm run test`: Runs the test suite (if available).
- `npm run lint`: Runs the linter to check for code style issues.

## Additional Resources

- [Node.js Documentation](https://nodejs.org/en/docs/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Express Documentation](https://expressjs.com/)

By following these steps, you should have your Node.js and TypeScript application up and running. If you encounter any issues, please refer to the documentation of the respective tools or seek help from the community.

## API Endpoints

All API endpoints can be referenced in the [API Reference](API_REFERENCE.md) document.

## Versioning

This project is versioned to ensure backward compatibility and easy maintenance. The current version is [version].






# Team Spark Contribution - NodeJs Boilerplate

## Introduction

Welcome to Team Spark contribution to the NodeJS Boilerplate. This document outlines our API and database designs and provides instructions for setting up and contributing to this repository.

## API Design

Our API design is crafted using OpenAPI (formerly known as Swagger). The design ensures a robust and comprehensive structure for all endpoints. Below are the details of our API design:

### Endpoints

# API Endpoints Documentation

## /auth/login
**POST**
- **Description:** Login a user
- **Request Body:**
  - `email` (string, example: 'john.doe@example.com')
  - `password` (string, example: 'password258')
- **Responses:**
  - `201`: User logged in successfully
  - `401`: Invalid credentials

## /auth/change-password
**POST**
- **Description:** Change user password
- **Request Body:**
  - `oldPassword` (string, example: 'oldpassword123')
  - `newPassword` (string, example: 'newpassword123')
- **Responses:**
  - `200`: Password changed successfully
  - `400`: Invalid input
  - `401`: Unauthorized

## /auth/social-login
**POST**
- **Description:** Social login for users
- **Request Body:**
  - `provider` (string, example: 'google')
  - `token` (string, example: 'socialauth_token')
- **Responses:**
  - `200`: User logged in successfully
  - `400`: Invalid input

## /auth/forgot-password
**POST**
- **Description:** Forgot password
- **Request Body:**
  - `email` (string, format: email)
- **Responses:**
  - `200`: Password reset link sent to your registered email successfully
  - `400`: Bad request

## /auth/reset-password
**POST**
- **Description:** Reset password
- **Request Body:**
  - `token` (string)
  - `newPassword` (string, format: password)
- **Responses:**
  - `200`: Password reset successfully
  - `400`: Wrong credentials
  - `401`: Unauthorized

## /users/{userId}
**GET**
- **Description:** Get user profile
- **Parameters:**
  - `userId` (string, example: '5f8d0d55b54764421b7156c7')
- **Responses:**
  - `200`: User profile retrieved successfully
  - `404`: User not found

## /users
**GET**
- **Description:** Get list of users
- **Parameters:**
  - `page` (integer, example: 1)
  - `limit` (integer, example: 10)
- **Responses:**
  - `200`: List of users retrieved successfully

## /admin/users
**GET**
- **Description:** Admin - Get all users
- **Parameters:**
  - `page` (integer, example: 1)
  - `limit` (integer, example: 10)
- **Responses:**
  - `200`: List of users retrieved successfully


### OpenAPI Specification

The complete OpenAPI specification can be found [here]([https://app.swaggerhub.com/apis/Backend_Node_Express/Boilerplate/1.0.0](https://drive.google.com/file/d/1K-7tN1S6JOqorYkfJvbkBGVAZbr4I3ua/view?usp=sharing)).

## Database Design

Our database design is structured to be scalable and efficient. We use a relational database model to manage user data and related entities.

### Entities

## Users
- **Primary Key:**
  - `user_id` int NOT NULL
- **Columns:**
  - `first_name` char(50) NOT NULL
  - `email` char(50) NOT NULL
  - `password` char(50) NOT NULL
  - `phone_number` char(50) NOT NULL
  - `referral_id` char(50) NULLABLE
  - `role` char(50) NOT NULL

## Notification
- **Primary Key:**
  - `notification_id` int NOT NULL
- **Columns:**
  - `title` char(50) NOT NULL
  - `message` char(255) NOT NULL
  - `user_id` char(50) NULL
- **Foreign Key:**
  - `user_id` references `Users(user_id)`

## Address
- **Primary Key:**
  - `address_id` int NOT NULL
- **Columns:**
  - `street` char(50) NOT NULL
  - `city` char(50) NOT NULL
  - `postal_code` char(50) NOT NULL
  - `state` char(50) NOT NULL
  - `country` char(50) NOT NULL
  - `region` char(50) NULL
  - `user_id` int NOT NULL
- **Foreign Key:**
  - `user_id` references `Users(user_id)`

## User_Organisations
- **Primary Key:**
  - `id` int NOT NULL
- **Columns:**
  - `organisation_id` int NOT NULL
  - `user_id` int NOT NULL
  - `is_owner` boolean
- **Foreign Keys:**
  - `organisation_id` references `Organisations(organisation_id)`
  - `user_id` references `Users(user_id)`

## Blog
- **Primary Key:**
  - `blog_id` int NOT NULL
- **Columns:**
  - `user_id` int NOT NULL
  - `title` char(50) NOT NULL
  - `post` char(50) NOT NULL
  - `created_at_time` NOT NULL
  - `updated_at_time` NOT NULL
- **Foreign Key:**
  - `user_id` references `Users(user_id)`

## Payments
- **Primary Key:**
  - `payment_id` int NOT NULL
- **Columns:**
  - `user_id` char(50) NOT NULL
  - `timestamp` NOT NULL
  - `amount` char(50) NOT NULL
  - `status` char(50) NOT NULL
- **Foreign Key:**
  - `user_id` references `Users(user_id)`

## Feedback
- **Primary Key:**
  - `feedback_id` int NOT NULL
- **Columns:**
  - `name` char(50) NOT NULL
  - `email` char(50) NOT NULL
  - `subject` char(50) NOT NULL
  - `message` char(255) NOT NULL
  - `phone_number` char(50) NULL

## Waitlist
- **Primary Key:**
  - `id` int NOT NULL
- **Columns:**
  - `email` char(50) NOT NULL
  - `created_at` char(50) NOT NULL

## Organisations
- **Primary Key:**
  - `organisation_id` int NOT NULL
- **Columns:**
  - `organisation_name` char(50) NOT NULL
  - `address` char(50) NOT NULL
  - `business_no` int NOT NULL

## Email Templates
- **Primary Key:**
  - `template_id` int NOT NULL
- **Columns:**
  - `title` char(50) NOT NULL
  - `subject` char(50) NOT NULL
  - `content` char(50) NOT NULL
  - `created_at` date NOT NULL
  - `updated_at` date NOT NULL

### Database Schema

The complete database schema can be found [here]([https://link-to-database-schema](https://drive.google.com/file/d/1BCwhD5hF5ZG3IwH7HhUEGsBRrFcYaAkS/view?usp=sharing)).
