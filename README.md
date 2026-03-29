# 🚀 ApplyGenius

ApplyGenius is a full-stack Ruby on Rails web application designed to help users efficiently track and manage their job applications.  
It also includes a RESTful API and an AI-powered resume analyzer that evaluates how well a resume matches a job description.

---

## ✨ Features

- 🔐 User authentication (Devise)
- 🏢 Company management
- 📄 Job application tracking
- 🎤 Interview management with notes
- 🧠 AI Resume Analyzer (OpenAI integration)
- 🔗 RESTful API with token-based authentication
- ☁️ Deployed on Heroku

---

## 🧱 Tech Stack

- Backend: Ruby on Rails  
- Database: PostgreSQL  
- Authentication: Devise  
- API: REST (JSON)  
- AI Integration: OpenAI API  
- Deployment: Heroku  
- Testing Tool: Postman  

---

## 🧠 AI Resume Analyzer

This feature allows users to:
- Upload a resume (PDF)
- Provide a job description
- Receive AI-generated feedback:
  - Strengths
  - Gaps
  - Suggestions

---

## 🔗 API Overview

Base URL:
```
/api/v1/
```

### Authentication

All protected endpoints require:
```
Authentication-Token: YOUR_TOKEN
```

---

### Example Endpoints

#### 🔑 Login
```
POST /api/v1/login
```

#### 🏢 Get Companies
```
GET /api/v1/companies
```

#### 📄 Get Job Applications
```
GET /api/v1/job_applications
```

#### 🎤 Get Interviews
```
GET /api/v1/interviews
```

---

## 🧪 API Testing

The API was tested using Postman, including:
- User login and token retrieval  
- Authenticated requests  
- Data retrieval endpoints  

---

## 📊 Database Design

The application uses a relational database with:

- One-to-One: User → Profile  
- One-to-Many:
  - User → Companies  
  - User → JobApplications  
- Many-to-Many: JobApplication ↔ Skills  

---

## ⚙️ Installation

### 1. Clone the repository
```
git clone https://github.com/YOUR_USERNAME/applygenius.git
cd applygenius
```

### 2. Install dependencies
```
bundle install
```

### 3. Setup database
```
rails db:create
rails db:migrate
rails db:seed
```

### 4. Add environment variables

Create a `.env` file:
```
OPENAI_API_KEY=your_api_key_here
```

### 5. Run the server
```
rails server
```

Open:
```
http://localhost:3000
```

---

## 🌍 Deployment

The application is deployed on Heroku.

> Note: AI feature may require proper environment configuration in production.

---


## 🧩 Challenges

- Managing authentication for both web and API  
- Handling differences between local and production environments  
- Integrating external AI services  

---

## 🚀 Future Improvements

- Improve AI reliability in production  
- Store AI analysis results  
- Enhance UI/UX  
- Add advanced filtering and analytics  

---

## 👤 Author

Shada Arabi
---

## 📌 Link to the project:
https://powerful-plateau-99155-42a1fdc3e4bc.herokuapp.com/

