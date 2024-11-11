# VyloGo
An Task manager app with Expense tracking : - java demo application

Vylo - Todo and Expense Tracker

Vylo is a learning-oriented, open-source project that demonstrates core concepts of Spring Boot microservice architecture with a React front end. The application is designed to manage to-do lists and monitor expenses, offering a comprehensive set of features to showcase the potential of Spring Boot, microservices, and various integrated tools.
Table of Contents

    Project Overview
    Tech Stack
    Features
    Architecture
    Setup & Installation
    Usage
    Contributing
    License

Project Overview

Vylo is intended to serve as an educational resource for developers looking to explore Spring Boot microservices and modern backend/frontend integrations. By exploring and extending this project, users can learn about microservice architecture, authentication mechanisms, messaging brokers, unit testing, and various other concepts.
Tech Stack

Backend:

    Java, Spring Boot
    MySQL (or any SQL-compatible DB)
    RabbitMQ
    Apache Superset (for dashboarding)

Frontend:

    React.js

Additional Tools:

    JUnit 5/Mockito
    Swagger
    Firebase
    Docker
    ELK Stack
    iText (for PDF generation)
    Apache Superset (for data visualization)

Features
Core Microservices

    To-do Management: Manage a list of to-do items with standard CRUD operations.
    Expense Tracking: Record, categorize, and monitor expenses, displayed via Apache Superset dashboards.

Technical Highlights

    Microservice Architecture: Modularized into independently deployable services.
    Spring Boot REST APIs: Clean, scalable RESTful endpoints with Swagger API documentation.
    Spring Security with OAuth2 & JWT: Secures API endpoints with OAuth2 and JWT-based authentication, supporting both Authentication and Authorization.
    Email Integration: Sends email notifications, such as OTPs, through integrated email services.
    Messaging with RabbitMQ: Async message handling via RabbitMQ.
    Push Notifications: Integrated with Firebase for real-time notifications.
    ELK Stack Integration: Enhanced logging and monitoring capabilities using Elasticsearch, Logstash, and Kibana.
    Apache Superset for Visualization: Data visualization for expense tracking.
    Containerized Services with Docker: Microservices and Apache Superset are containerized for easy deployment.

Development Features

    Comprehensive Unit Testing: Unit tests written with JUnit 5 and Mockito.
    Profiling & Monitoring with Spring Actuator: Built-in monitoring and profiling.
    Exception Handling: Structured exception handling for cleaner code and user feedback.
    Method-Level Security: Protects sensitive methods within the application.
    CSRF Protection: Enhanced security against CSRF attacks.
    Swagger Integration: API documentation for easy testing and interaction.
    PDF Generation with iText: Generate downloadable PDF summaries of statistics.
    CI/CD Integration: Continuous Integration/Deployment workflows for streamlined deployment.

Architecture

This project adopts a microservice architecture, dividing the application into multiple services:

    User Service: Manages user registration, authentication, and authorization.
    To-do Service: Manages CRUD operations for to-do items.
    Expense Service: Manages expense records, categories, and reports.
    Notification Service: Handles email and push notifications.

Communication between services is achieved through REST APIs and RabbitMQ for asynchronous messaging. Data visualization is achieved through Apache Superset.
Setup & Installation
Prerequisites

    Java 11 or later
    Node.js and npm (for frontend)
    Docker (for containerized services)
    MySQL or any preferred SQL database
    RabbitMQ
    Firebase Account for push notifications
    ELK Stack (Elasticsearch, Logstash, Kibana)

Installation Steps

    Clone the Repository

git clone https://github.com/your-username/vylo-todo-expense-tracker.git
cd vylo-todo-expense-tracker

Backend Setup

    Database: Set up MySQL (or other SQL DB) and update database configurations in application.properties.
    RabbitMQ: Ensure RabbitMQ is running on default ports, or update configurations accordingly.
    Build and Run:

    ./mvnw clean install
    ./mvnw spring-boot:run

Frontend Setup

cd frontend
npm install
npm start

Docker Setup (For containerized services)

    Run all containers for services:

        docker-compose up

Usage
Accessing APIs

Swagger API documentation is available at:

    http://localhost:8080/swagger-ui.html

Apache Superset Dashboard

Access expense dashboards at:

    http://localhost:8088 (Superset default port)

Example Features

    Add To-do: Use the frontend UI to create and view your tasks.
    Track Expenses: Record and view expense trends via Superset dashboards.
    Receive Notifications: Test email and push notifications.

Contributing

Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

    Fork the repository.
    Create your feature branch (git checkout -b feature/AmazingFeature).
    Commit your changes (git commit -m 'Add some AmazingFeature').
    Push to the branch (git push origin feature/AmazingFeature).
    Open a pull request.

License

This project is licensed under the CC BY-NC 4.0 License - feel free to use it for educational and learning purposes only. Rebranding and commercial use are prohibited.
