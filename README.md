# AI Chatbot using Spring Boot, React & Mistral AI

A full-stack Generative AI chatbot application built using Spring Boot, React.js, and Mistral AI.  
The application allows users to interact with an AI assistant in real time while storing chat history in MySQL.

---

## Features

- AI-powered chatbot using Mistral AI
- Spring Boot REST API backend
- React.js frontend
- MySQL database integration
- Persistent chat history storage
- Clean and responsive UI
- Cross-origin support for frontend-backend communication

---

## Tech Stack

### Backend
- Java
- Spring Boot
- Spring AI
- Mistral AI API
- Spring Data JPA
- MySQL

### Frontend
- React.js
- Axios
- HTML/CSS

---

## Project Architecture

```text
React Frontend
       ↓
Spring Boot REST API
       ↓
Mistral AI API
       ↓
MySQL Database
```

---

## API Endpoints

### Generate AI Response

```http
GET /api/mistral-ai/{message}
```

Example:

```http
/api/mistral-ai/Hello
```

---

### Get Chat History

```http
GET /api/mistral-ai/history
```

---

## Database Schema

### Table: `mistralai`

| Column        | Type |
|---------------|------|
| id            | BIGINT |
| user_message  | TEXT |
| bot_response  | TEXT |
| timestamp     | DATETIME |

---

## Installation & Setup

### Clone Repository

```bash
git clone https://github.com/your-username/AI-Chatbot-SpringBoot-React.git
```

---

## Backend Setup

### Configure MySQL

Create a database:

```sql
CREATE DATABASE mistralai;
```

---

### Configure `application.properties`

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/mistralai
spring.datasource.username=your_username
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

spring.ai.mistralai.api-key=YOUR_API_KEY
```

---

### Run Spring Boot Application

```bash
mvn spring-boot:run
```

Backend runs on:

```text
http://localhost:8080
```

---

## Frontend Setup

Navigate to frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Run React application:

```bash
npm start
```

Frontend runs on:

```text
http://localhost:3000
```

---

## Future Improvements

- JWT Authentication
- Streaming AI responses
- PDF upload & RAG integration
- User-specific chat sessions
- Docker deployment
- Markdown/code rendering
- Chat export functionality

---

## Screenshots
<img width="1918" height="970" alt="image" src="https://github.com/user-attachments/assets/06efbd2e-6a0c-4d2d-b4ab-634332a9ac68" />
<img width="763" height="213" alt="image" src="https://github.com/user-attachments/assets/6a225723-da6a-4db6-9027-299d75294bd6" />




