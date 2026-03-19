



# Scheme Seva - Government Scheme Management Portal

A centralized web platform designed to help citizens discover, understand, and access government welfare schemes efficiently.



## Table of Contents

* Overview
* Problem Statement
* Solution
* Features
* System Architecture
* Tech Stack
* Installation and Setup
* Environment Variables
* API Endpoints
* Folder Structure
* Future Enhancements
* Contributing
* License



## Overview

Scheme Seva provides a single platform where users can explore various government schemes, check eligibility, and receive personalized recommendations. The system aims to improve awareness and accessibility of welfare programs.



## Problem Statement

Many citizens are unable to benefit from government schemes due to:

* Lack of awareness
* Scattered information across multiple platforms
* Difficulty understanding eligibility criteria
* Complex application procedures



## Solution

Scheme Seva addresses these issues by offering:

* A centralized database of schemes
* Intelligent filtering and search options
* AI-based chatbot assistance
* Personalized recommendations



## Features

### 1. Scheme Discovery

* Access central and state government schemes
* Advanced filtering options:

  * Income group
  * Gender
  * Age group
  * State
  * Category



### 2. AI Chatbot

* Interactive chatbot for user queries
* Provides information on:

  * Eligibility
  * Required documents
  * Benefits
  * Application process
* Supports multiple languages



### 3. User Management

* Secure user authentication using JWT
* Profile management
* Save and manage favorite schemes
* Track user interactions



### 4. Recommendation System

* Personalized scheme suggestions based on:

  * User demographics
  * Location
  * Interests
  * Previous activity



## System Architecture

The application follows a client-server architecture:

* Frontend communicates with backend via REST APIs
* Backend handles business logic and authentication
* MongoDB is used for data storage
* AI chatbot is integrated using external API



## Tech Stack

### Frontend

* React.js
* Tailwind CSS
* Material UI
* Axios
* React Router

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication

### AI Integration

* Google Gemini API



## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/9582anupam/scheme-seva




### 2. Install Dependencies

```bash
cd Frontend
npm install

cd ../Backend
npm install




## Environment Variables

Create a `.env` file in the Backend directory and add:


PORT=5000
MONGODB_URI=your_mongodb_uri
ACCESS_TOKEN_SECRET=your_access_token_secret
REFRESH_TOKEN_SECRET=your_refresh_token_secret
GEMINI_API_KEY=your_gemini_api_key
```



### 3. Run the Application

Start Backend:

```bash
npm start
```

Start Frontend:

```bash
npm start
```



## API Endpoints

### User Routes

* POST `/api/v1/users/signup`
* POST `/api/v1/users/login`
* POST `/api/v1/users/logout`
* GET `/api/v1/users/getme`
* GET `/api/v1/users/refresh-access-token`



### Scheme Routes

* GET `/api/v2/schemes/get-all-schemes`
* GET `/api/v2/schemes/get-scheme-by-id/:id`
* GET `/api/v2/schemes/get-filtered-schemes`
* POST `/api/v2/schemes/save-favorite-schemes`
* DELETE `/api/v2/schemes/remove-favorite-schemes/:id`



### Chatbot Route

* POST `/api/v1/chatbot`



### Recommendation Route

* GET `/api/v1/users/personalized`



## Folder Structure


scheme-seva/
│
├── Frontend/
│   ├── src/
│   ├── components/
│   ├── pages/
│
├── Backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│
└── README.md



## Future Enhancements

* Add more regional languages
* Mobile application support
* Notification system for new schemes
* Direct application submission
* Admin dashboard for scheme management


## Contributing

Contributions are welcome. Please follow standard GitHub practices:

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Submit a pull request



## License

This project is licensed under the MIT License.



If you want next level improvement, I can add:

* badges (build, license, tech stack)
* screenshots section
* deployment link section

That will make your GitHub look like a professional project.
