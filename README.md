# AI-Powered Job & Skill Intelligence Platform

An intelligent career development platform designed to help job seekers discover relevant opportunities, identify skill gaps, analyze job requirements, and make data-driven career decisions.

## Project Overview

The AI-Powered Job & Skill Intelligence Platform aims to bridge the gap between job seekers' existing skills and industry requirements.

The platform will analyze job descriptions, identify required technical skills, compare them with user profiles, and provide personalized recommendations to improve employability.

This project is being developed as a full-stack application with a Java Spring Boot backend, PostgreSQL database, and a modern frontend.

## Problem Statement

Job seekers often struggle to identify which skills are required for their target roles, understand how their current skills compare with industry expectations, and find suitable job opportunities.

This platform aims to simplify that process through job analysis, skill-gap identification, and AI-powered career recommendations.

## Key Features

### Planned Features

- User registration and secure authentication.
- Profile and resume management.
- Job search and job description analysis.
- Automatic extraction of technical skills from job descriptions.
- Skill-gap analysis based on user profiles.
- Job matching and recommendation system.
- Personalized learning recommendations.
- Career insights and analytics dashboard.
- AI-powered career assistance.

## Technology Stack

| Component | Technology |
|---|---|
| Backend | Java, Spring Boot |
| Frontend | React, TypeScript |
| Database | PostgreSQL |
| ORM | Spring Data JPA, Hibernate |
| API | REST APIs |
| Security | Spring Security, JWT (planned) |
| Build Tool | Maven |
| Version Control | Git, GitHub |
| AI Integration | Planned |

## Project Architecture

The application will follow a layered architecture.

```text
Frontend (React + TypeScript)
             |
             v
       REST APIs
             |
             v
    Spring Boot Backend
             |
      ----------------
      |      |       |
   Controller Service Repository
                     |
                     v
                PostgreSQL
```

## Current Development Status

**Phase 1 – Backend Foundation**

- [x] Spring Boot project initialization.
- [x] Maven configuration.
- [x] PostgreSQL installation and database connection.
- [x] JPA/Hibernate initialization.
- [x] Initial health-check endpoint.
- [x] Git repository setup.
- [x] GitHub repository integration.
- [ ] User registration and authentication.
- [ ] User profile management.

## Getting Started

### Prerequisites

Install the following:

- Java Development Kit (JDK).
- PostgreSQL.
- IntelliJ IDEA or another Java IDE.
- Git.

### 1. Clone the Repository

```bash
git clone https://github.com/HariKrishnaM-1118/AI-Job-Skill-Intelligence-Platform.git
```

### 2. Navigate to the Project

```bash
cd AI-Job-Skill-Intelligence-Platform
```

### 3. Create the PostgreSQL Database

Open PostgreSQL and execute:

```sql
CREATE DATABASE job_intelligence;
```

### 4. Configure Environment Variables

Set your PostgreSQL password as an environment variable.

**Windows PowerShell:**

```powershell
$env:DB_PASSWORD="your-postgresql-password"
```

Make sure your `application.properties` contains:

```properties
spring.application.name=jobintelligence

spring.datasource.url=jdbc:postgresql://localhost:5432/job_intelligence
spring.datasource.username=postgres
spring.datasource.password=${DB_PASSWORD}

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true

server.port=8080
```

Do not commit actual database credentials to GitHub.

### 5. Run the Application

Using the Maven wrapper on Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

### 6. Test the Health Endpoint

Open:

```text
http://localhost:8080/api/health
```

A successful response indicates that the backend application is running.

## Future Development Roadmap

1. Backend foundation and database integration.
2. User registration, login, and JWT authentication.
3. User profile and resume management.
4. Job management and job description processing.
5. Skill extraction and skill-gap analysis.
6. Job matching and recommendation engine.
7. AI-powered career guidance.
8. React frontend development.
9. Testing, Docker, and deployment.

## Project Goals

- Build a complete full-stack application.
- Apply real-world backend development practices.
- Understand database design and REST API development.
- Integrate AI into practical career-related workflows.
- Develop a portfolio project demonstrating software engineering skills.

## Author

**Hari Krishna M**

GitHub: [HariKrishnaM-1118](https://github.com/HariKrishnaM-1118)

LinkedIn: [LinkedIn Profile](https://linkedin.com/in/harikrishnam96)

---

*This project is actively under development. Features and documentation will be updated as development progresses.*