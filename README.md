#AI Resume Builder Backend Development Prompt

## Prompt :

```
You are an experienced Senior Java Backend Engineer and Spring Boot Architect with over 10 years of experience building scalable, secure, maintainable, and production-grade enterprise applications.

Your task is to design and implement the backend for an AI Resume Builder using Spring Boot 3.x, Java 21, PostgreSQL, Spring Security, JWT, Spring AI, Flying Saucer + OpenPDF, and Cloudinary.

Write the code exactly as an experienced senior backend developer would write for a real enterprise application.

Project Goal

Develop a production-ready REST API for an AI-powered Resume Builder that enables users to create, manage, optimize, and export professional ATS-friendly resumes using Artificial Intelligence.

Core Features

Authentication

- User Registration
- User Login
- JWT Authentication
- Secure Password Encryption using BCrypt
- Forgot Password
- Reset Password
- Logout
- Profile Management

Resume Management

- Create multiple resumes
- Update resumes
- Delete resumes
- Duplicate resumes
- Retrieve a single resume
- Retrieve all user resumes
- Auto-save resume
- Resume version history
- Restore previous resume versions

Resume Sections

Each resume should support:

- Personal Details
- Professional Summary
- Education
- Work Experience
- Projects
- Skills
- Certifications
- Languages
- Achievements
- Interests
- Custom Sections

Users should be able to add, update, delete, and retrieve every section independently.

AI Features

Integrate Spring AI with OpenAI.

The backend must automatically build prompts using the user's resume data.

The frontend should never send raw prompts.

Provide AI features for:

- Generate Professional Summary
- Rewrite Professional Summary
- Improve Work Experience
- Rewrite Project Descriptions
- Suggest Missing Skills
- Improve Resume Grammar
- ATS Optimization Suggestions
- Resume ATS Score
- Generate Cover Letter
- Generate Interview Preparation Questions
- Career Improvement Suggestions

Store all AI-generated content in the database.

PDF Generation

Generate professional ATS-friendly PDF resumes using:

- Flying Saucer
- OpenPDF

Requirements:

- Generate text-based PDFs
- Preserve selectable/searchable text
- Use HTML + CSS templates
- Support multiple resume templates
- Generate PDFs in memory using ByteArrayOutputStream
- No temporary files on disk

Cloudinary Integration

Use Cloudinary for storing:

- Resume PDFs
- User Profile Images

Requirements:

- Upload generated PDFs
- Replace old PDFs when regenerated
- Delete PDFs when resumes are deleted
- Store Cloudinary URL and Public ID in PostgreSQL

Resume Templates

Support multiple resume templates including:

- Modern
- Classic
- Minimal
- Executive
- ATS Friendly

Users should be able to generate PDFs using any available template.

Security

- Secure APIs using JWT Authentication
- Users should only access their own resumes
- Encrypt passwords using BCrypt
- Protect all APIs except authentication endpoints

Technical Requirements

While generating code, strictly follow these principles:

- Follow SOLID Principles.
- Follow Clean Architecture.
- Use a Feature-Based Monolithic Multi-Layered Architecture.
- Follow REST API Best Practices.
- Follow Java Coding Standards.
- Follow Spring Boot Best Practices.
- Follow PostgreSQL Best Practices.
- Keep controllers thin.
- Keep all business logic inside the service layer.
- Never place business logic inside controllers.
- Use constructor injection only.
- Never use field injection.
- Use DTOs for every API.
- Never expose JPA entities.
- Use MapStruct for Entity ↔ DTO mapping.
- Use SLF4J for logging.
- Use Jakarta Validation.
- Implement centralized exception handling using "@RestControllerAdvice".
- Use UUID as primary keys.
- Store all secrets in environment variables.
- Write clean, modular, reusable, maintainable, scalable, and production-ready code.

The generated backend should resemble code written by an experienced Senior Spring Boot developer working on a real enterprise application.

```
----