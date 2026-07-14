# BDA-practicals

## Practical 1: Write an R-Program to demonstrate working with Arithmetic operators.

## Code: 
```R
vect1 <- c(4,5,6)
vect2 <- c(7,8,9)
cat("addition of vector is", vect1+vect2)
cat("substraction of vector is", vect1-vect2)
cat("multiplication of vector is", vect1*vect2)
cat ("division of vector is", vect1/vect2)
cat ("modulus of vector is", vect1%%vect2)
```

## Practical 2: Write an R Program to Find the Factorial of a Number.

## Code:
```R
num <- -1
if(num < 0){
  cat("Factorial is not defined for negative numbers.\n")
} else if(num == 0 || num == 1){
  cat("Factorial is 1\n")
} else {
  res <- 1
  for(i in 2:num){
    res <- res * i
  }
  cat("Factorial is", res, "\n")
}
```

## Practical 4: Write an R Program to create a Matrix and access rows and columns using functions colnames() and rownames() .

## Code:
```R
a = matrix(c(11,12,13,14,15,16,17,18,19),3,3,byrow=TRUE)
rownames(a)<-letters[1:3]
print(a)

b = matrix(c(21,22,23,24,25,26,27,28,29),3,3,byrow=TRUE)
colnames(b)<-letters[1:3]
print(b)
```

## Practical 5: Write an R Program to create a List and modify its components. 

## Code: 
```R
lt = list( 
 a=10, 
 char_vector=letters[1:4], 
 mat1=matrix(c(1,2,3,4,5,6), nrow = 2), 
 mat2=matrix(1:6, nrow = 3) 
) 
print("list before modificaiton:\n") 
print(lt) 
lt$a=20 
print("list after modification:\n") 
print(lt)
```

## Practical 6: Write an R Program to create a Matrix from a Vector using dim() function. 

## Code:
```R
mat <- c(32,12,53,41,64,23,74,28) 
dim(mat) <- c(4,2) 
print(mat)
```

## Practical 7: Write an R Program to create a List and modify its components. 

## Code: 
```R
lt = list( 
 a=10, 
 char_vector=letters[1:4], 
 mat1=matrix(c(1,2,3,4,5,6), nrow = 2), 
 mat2=matrix(1:6, nrow = 3) 
) 
print("list before modificaiton:\n") 
print(lt) 
lt$a=20 
print("list after modification:\n") 
print(lt)
```

## Practical 8: Write an R Program to create a Data Frame. 

## Code: 
```R
fm = data.frame(index=c(1:6), char=letters[1:6]) 
print(fm)
```

## Practical 9: Write an R Program to access a Data Frame like a List.

## Code: 
```R
dfm = data.frame(index=c(1:6), char=letters[1:6]) 
cat("Before Accessing:\n") 
print(dfm) 
dfm$index=c(100,106) 
cat("After Accessing:\n") 
print(dfm)
```

## Practical 10: Write an R Program to access a Data Frame like a Matrix.

## Code: 
```R
dfm = data.frame(index=c(1:6), char=letters[1:6]) 
cat(“Before Accessing:\n”) 
print(dfm) 
dfm[[1]]=c(10,16) 
cat(“After Accessing:\n”) 
print(dfm) 
```

## Promot :

```
You are an experienced Senior Java Backend Engineer and Spring Boot Architect with over 10 years of experience building scalable, secure, and production-grade enterprise applications.

Build a production-ready AI Resume Builder web application using a Monolithic Multi-Layered Spring Boot Architecture for the backend and React.js for the frontend.
The application should allow users to create, edit, manage, and download professional ATS-friendly resumes using AI assistance.
The project should follow clean code principles, SOLID principles, proper package structure, DTO pattern, exception handling, validation, and REST API best practices.AI Resume Builder Backend – Spring Boot Development Prompt

While generating code, strictly follow these principles:

- Follow SOLID Principles
- Follow Clean Architecture
- Follow Monolithic Multi-Layered Architecture
- Follow Feature-Based Package Structure
- Follow Object-Oriented Programming (OOP) Principles
- Follow REST API Best Practices
- Follow Java Coding Standards
- Follow Spring Boot Best Practices
- Follow PostgreSQL Best Practices
- Write clean, readable, maintainable, and reusable code.
- Keep controllers thin.
- Keep business logic inside the service layer only.
- Never place business logic inside controllers.
- Write modular code that is easy to extend.
- Avoid duplicate code.
- Use meaningful class, method, and variable names.
- Use constructor injection only.
- Never use field injection.
- Keep methods small and focused on a single responsibility.
- Use proper transaction management.
- Use appropriate fetch strategies to avoid N+1 query problems.
- Write code that is production-ready and scalable.

Mandatory Design Patterns

Use:

- DTO Pattern
- Repository Pattern
- Service Layer Pattern
- Mapper Pattern
- Builder Pattern where appropriate
- Factory Pattern where appropriate

DTOs

Never expose JPA entities directly through APIs.

Create:

- Request DTOs
- Response DTOs

Every API should communicate only through DTOs.

Mapping

Use MapStruct for all Entity ↔ DTO mappings.

Do not perform manual mapping unless absolutely necessary.

Logging

Use SLF4J logging throughout the application.

Log important events including:

- Authentication
- User Registration
- Resume Creation
- Resume Updates
- AI Requests
- AI Responses
- PDF Generation
- Cloudinary Uploads
- Cloudinary Deletions
- Validation Failures
- Database Errors
- Unexpected Exceptions

Use appropriate log levels:

- INFO
- DEBUG
- WARN
- ERROR

Do not use "System.out.println()" anywhere in the project.

Validation

Use Jakarta Validation.

Validate every request DTO.

Return meaningful validation messages.

Exception Handling

Implement centralized exception handling using "@RestControllerAdvice".

Create custom exceptions for all business scenarios.

Return consistent API responses for both success and failure.

API Responses

Create a common API response model.

Every response should contain:

- success
- message
- data
- timestamp

Create a separate standardized error response model.

Documentation

Document every REST API using Swagger/OpenAPI annotations.

Security

Implement secure JWT Authentication using Spring Security.

Passwords must always be encrypted using BCrypt.

Secure every protected endpoint.

Ensure users can access only their own resources.

Configuration

Store sensitive configuration values in environment variables.

Never hardcode:

- Database credentials
- JWT Secret
- OpenAI API Key
- Cloudinary API Key
- Cloudinary Secret

Final Goal

Generate a production-ready backend that follows enterprise-level coding standards and can be deployed without major architectural changes.

The generated code should look like it was written by an experienced Senior Spring Boot developer working on a large-scale enterprise application.

AI Resume Builder Backend – Spring Boot Development Prompt

Project Overview

Build a production-ready backend for an AI Resume Builder application using Spring Boot 3.x, Java 21, and PostgreSQL.

The backend should expose REST APIs that allow users to create, manage, enhance, version, and export resumes using AI assistance.

The application must follow:

- Monolithic Multi-Layered Architecture
- Feature-Based Package Structure
- SOLID Principles
- Clean Architecture
- DTO Pattern
- Repository Pattern
- Service Layer Pattern
- Global Exception Handling
- Validation
- REST API Best Practices
- Clean Code Principles

The code should be modular, maintainable, scalable, secure, and production-ready.

---

Technology Stack

Core

- Java 21
- Spring Boot 3.x
- Maven

Spring Modules

- Spring Web
- Spring Data JPA
- Spring Security
- Spring Validation

Database

- PostgreSQL

Authentication

- JWT Authentication
- BCrypt Password Encoder

AI

- Spring AI
- OpenAI

PDF Generation

- Flying Saucer
- OpenPDF

File Storage

- Cloudinary Java SDK

Documentation

- Swagger/OpenAPI

Utilities

- Lombok
- MapStruct

---

Architecture

Use a Feature-Based Monolithic Multi-Layered Architecture.

Each feature should contain:

- controller
- service
- repository
- entity
- dto
- mapper

---

Package Structure

com.resumebuilder

├── config
│
├── common
│   ├── exception
│   ├── response
│   ├── constants
│   ├── util
│   └── mapper
│
├── security
│   ├── jwt
│   ├── filter
│   ├── service
│   └── config
│
├── auth
│
├── user
│
├── resume
│
├── education
│
├── experience
│
├── project
│
├── skill
│
├── certification
│
├── language
│
├── template
│
├── ai
│
├── pdf
│
├── cloudinary
│
└── version

---

Database

Use PostgreSQL.

Use UUID as primary keys for all entities.

Every table must contain:

- created_at
- updated_at

Use proper indexes and foreign key relationships.

---

Database Tables

users

- id
- first_name
- last_name
- email
- password_hash
- profile_image
- created_at
- updated_at

---

resumes

- id
- user_id
- template_id
- title
- summary
- ats_score
- pdf_url
- pdf_public_id
- status
- created_at
- updated_at

---

personal_details

- id
- resume_id
- first_name
- last_name
- email
- phone
- address
- city
- state
- country
- postal_code
- linkedin_url
- github_url
- portfolio_url
- created_at
- updated_at

---

education

- id
- resume_id
- institution_name
- degree
- field_of_study
- grade
- start_date
- end_date
- description
- created_at
- updated_at

---

experience

- id
- resume_id
- company_name
- job_title
- employment_type
- location
- start_date
- end_date
- currently_working
- description
- created_at
- updated_at

---

projects

- id
- resume_id
- project_name
- description
- technologies
- github_url
- project_url
- created_at
- updated_at

---

skills

- id
- resume_id
- skill_name
- skill_level
- category
- created_at
- updated_at

---

certifications

- id
- resume_id
- certification_name
- issuing_organization
- issue_date
- expiry_date
- credential_id
- credential_url
- created_at
- updated_at

---

languages

- id
- resume_id
- language_name
- proficiency
- created_at
- updated_at

---

templates

- id
- template_name
- preview_image
- theme_color
- is_premium
- created_at
- updated_at

---

ai_suggestions

- id
- resume_id
- section_name
- original_text
- suggested_text
- prompt_used
- created_at
- updated_at

---

resume_versions

- id
- resume_id
- version_number
- snapshot (JSONB)
- created_at
- updated_at

---

Authentication

Implement JWT Authentication.

Features:

- Register User
- Login User
- Logout User
- Forgot Password
- Reset Password (optional)
- Email Verification (optional)

Requirements:

- BCrypt password encryption
- JWT access token generation
- JWT validation filter
- Secure all APIs except authentication endpoints
- Users should access only their own resumes

Do not implement:

- Admin
- Roles
- RBAC
- Permission Management

Only a single user type exists.

---

Resume Management Features

Users should be able to:

- Create Resume
- Update Resume
- Delete Resume
- Duplicate Resume
- View Resume
- List Resumes
- Maintain Resume Versions
- Restore Previous Version
- Generate Resume PDF
- Download Resume PDF

---

Resume Sections

Support APIs for:

- Personal Details
- Professional Summary
- Education
- Experience
- Projects
- Skills
- Certifications
- Languages
- Achievements
- Interests
- Custom Sections

Each section should support:

- Create
- Update
- Delete
- Get

---

AI Features

Integrate Spring AI with OpenAI.

Provide APIs for:

Professional Summary

Generate a professional summary from resume data.

---

Experience Enhancement

Improve work experience bullet points.

---

Project Enhancement

Rewrite project descriptions professionally.

---

Skill Suggestions

Suggest missing skills based on experience and projects.

---

ATS Optimization

Provide ATS recommendations.

---

Resume Scoring

Calculate and generate an ATS-style resume score.

---

Grammar Correction

Improve grammar and readability.

---

Cover Letter Generation

Generate a professional cover letter.

---

Interview Preparation

Generate interview questions and preparation tips.

---

Store all generated content in the ai_suggestions table.

---

PDF Generation

Use:

- Flying Saucer
- OpenPDF

Requirements:

- Generate ATS-friendly PDFs.
- Generate text-based PDFs.
- Text must remain selectable and searchable.
- Use HTML templates.
- Support multiple templates:
  - Modern
  - Classic
  - Minimal
  - Executive
  - ATS Friendly
- Handle page breaks correctly.
- Generate PDF using ByteArrayOutputStream.
- Do not write temporary files to disk.

Create a dedicated PdfService.

Responsibilities:

- Build HTML
- Apply Template
- Generate PDF
- Return PDF as byte[]

---

Cloudinary Integration

Use Cloudinary to store:

- Resume PDFs
- Profile Images

Requirements:

- Upload PDFs using resource_type="raw"
- Store pdf_url
- Store pdf_public_id
- Replace PDFs when regenerated
- Delete PDFs when resume is deleted
- Delete old profile images when replaced

Create a dedicated CloudinaryService.

Responsibilities:

- Upload File
- Delete File
- Replace Existing File

---

REST APIs

Authentication

POST /api/auth/register

POST /api/auth/login

POST /api/auth/logout

POST /api/auth/forgot-password

---

Resume

GET /api/resumes

GET /api/resumes/{id}

POST /api/resumes

PUT /api/resumes/{id}

DELETE /api/resumes/{id}

POST /api/resumes/{id}/duplicate

---

Education

POST /api/resumes/{id}/education

PUT /api/resumes/{id}/education/{educationId}

DELETE /api/resumes/{id}/education/{educationId}

---

Experience

POST /api/resumes/{id}/experience

PUT /api/resumes/{id}/experience/{experienceId}

DELETE /api/resumes/{id}/experience/{experienceId}

---

Projects

POST /api/resumes/{id}/projects

PUT /api/resumes/{id}/projects/{projectId}

DELETE /api/resumes/{id}/projects/{projectId}

---

Skills

POST /api/resumes/{id}/skills

PUT /api/resumes/{id}/skills/{skillId}

DELETE /api/resumes/{id}/skills/{skillId}

---

AI

POST /api/resumes/{id}/generate-summary

POST /api/resumes/{id}/improve-experience

POST /api/resumes/{id}/rewrite-project

POST /api/resumes/{id}/suggest-skills

POST /api/resumes/{id}/ats-score

POST /api/resumes/{id}/generate-cover-letter

POST /api/resumes/{id}/interview-preparation

---

PDF

POST /api/resumes/{id}/generate-pdf

GET /api/resumes/{id}/download

GET /api/resumes/{id}/preview

---

Validation

Use Jakarta Validation.

Validate:

- Email
- Phone Number
- URLs
- Required Fields
- Date Ranges
- Duplicate Skills
- Maximum Lengths

Return meaningful validation messages.

---

Exception Handling

Implement Global Exception Handling.

Create custom exceptions:

- ResourceNotFoundException
- DuplicateResourceException
- AuthenticationException
- ValidationException
- PdfGenerationException
- CloudinaryException
- AiServiceException

Return consistent API responses.

---

Logging

Use SLF4J.

Log:

- Authentication Events
- AI Requests
- PDF Generation
- Cloudinary Uploads
- Database Errors
- Unexpected Exceptions

---

DTO Pattern

Never expose Entity classes.

Create:

- Request DTOs
- Response DTOs

Use MapStruct for entity mapping.

---

Security

Implement:

- JWT Filter
- AuthenticationEntryPoint
- BCrypt Password Encoder
- Security Configuration
- CORS Configuration

Secure all endpoints except authentication endpoints.

Ensure users can only access their own data.

---

Data Access

Use Spring Data JPA.

Requirements:

- Pagination
- Sorting
- Specifications where needed
- Transaction Management
- Proper Fetch Strategies
- Avoid N+1 Query Problems

---

API Response Format

Create a common API response structure:

- success
- message
- data
- timestamp

Create separate error response models.

---

Configuration

Use application.yml.

Configure:

- PostgreSQL
- JWT
- OpenAI
- Cloudinary
- Swagger

All secrets must be loaded from environment variables.

---

Code Quality Requirements

Use:

- Constructor Injection
- Interface-Based Services
- Reusable Utility Classes
- Reusable Mappers
- Service Layer Business Logic
- Repository Pattern
- Clean Naming Conventions
- Unit-Testable Design

Avoid:

- Field Injection
- Business Logic in Controllers
- Hardcoded Values
- Duplicate Code

Generate complete entities, DTOs, repositories, services, service implementations, controllers, security configuration, exception handling, validation, Cloudinary integration, AI integration, PDF generation, and Swagger documentation following industry-standard Spring Boot best practices.
```