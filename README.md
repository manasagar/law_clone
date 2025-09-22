# ⚖️ Law Connect

Law Connect is a web application built to connect clients with legal professionals.  
It provides secure authentication, case and document management, and a modern interface, with future plans to integrate AI-powered legal insights.

## Table of Content
1. [How it Works](#How-it-Works)
2. [Features](#Features)
3. [Run Locally](#Run-Locally)



## How it Works
Law Connect uses a **multi-service architecture**:

- **Spring Boot** handles core backend logic including authentication, authorization, and case/document management.  
- **Flask** (planned module) will process AI/ML tasks like summarizing legal documents, running NLP-based analysis, and providing legal recommendations.  
- **React** powers the frontend, offering a responsive and user-friendly interface for clients, lawyers, and admins.  

The services communicate via REST APIs. Data is securely stored in relational databases, and the app is containerized using Docker for seamless deployment.

---

## Features
- **User Authentication & Roles**: Manage Clients, Lawyers, and Admins with role-based access control.  
- **Case Management**: Create, view, update, and track cases.  
- **Document Management**: Upload and manage case-related documents.  
- **Responsive Frontend**: React-based UI for smooth interactions.  
- **Planned AI Features**:
  - Summarize legal documents.  
  - Provide similar claim recommendations.  
- **Secure APIs**: JWT-based authentication ensures privacy and security.  
- **Dockerized Deployment**: Run all services easily in containers.  

---

## Run Locally
Clone the Project
```bash
git clone https://github.com/manasagar/law_connect.git
cd law_connect
```
Start Java Backend
```bash
cd spring-ws-server
./mvnw clean install
./mvnw spring-boot:run
```
Start flask backend
```bash
cd services
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python main.py
```
Start React frontend
```bash
cd hack
npm install
npm start
```
