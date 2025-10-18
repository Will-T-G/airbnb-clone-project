# Airbnb Clone

This is an Airbnb clone built with Next.js, TypeScript, Tailwind CSS, MongoDB, Prisma, Next auth, Leaflet and many other technologies.

## Feature Breakdown

- User registration and authentication
- Property listing and browsing
- Property booking and reservations
- Search and filtering of properties
- Interactive map using Leaflet to display property locations

## Project Goals:

Build a responsive, secure, and interactive property rental platform.

Strengthen understanding of full-stack development and deployment.

Practice teamwork and role-based collaboration within a development team.

## Team Roles

Frontend Developer - Builds the user interface using Next.js, React, and TailwindCSS to ensure a responsive and modern user experience.

Backend Developer - Designs and implements APIs, business logic, and integrates with the database using Prisma and Next.js API routes.

Database Administrator (DBA) - Manages MongoDB, ensuring data integrity, backups, and performance optimization.

UI/UX Designer - Creates wireframes and design prototypes that guide the user interface and improve usability.

DevOps Engineer - Sets up CI/CD pipelines, manages deployment, and ensures application scalability and reliability.

QA Engineer - Tests the app’s functionality, identifies bugs, and ensures a seamless user experience.

## Technology Stack

TypeScript - Adds static typing for better maintainability and fewer runtime errors.

Next.js - React framework for server-side rendering and full-stack development.

MongoDB - NoSQL database for storing user, property, and booking data.

Prisma - ORM for managing database models and queries efficiently.

TailwindCSS - Utility-first CSS framework for styling and responsive design.

Leaflet - Library for rendering interactive maps and location-based features.

Next-Auth - Handles authentication and secure user sessions.

React Query - Manages server state and handles API data fetching efficiently.

Zustand - Lightweight state management library for React.

## Database Design

Entities and Fields:

Users
Fields: id, name, email, password, createdAt
→ A user can create multiple properties and bookings.

Properties
Fields: id, title, description, price, location, ownerId
→ Each property belongs to one user.

Bookings
Fields: id, userId, propertyId, startDate, endDate, totalPrice
→ Each booking links a user and a property.

Reviews
Fields: id, userId, propertyId, rating, comment
→ A property can have multiple reviews.

Payments
Fields: id, bookingId, amount, status, createdAt
→ Each payment is tied to a booking.

## API Security

Security measures include:

Authentication: Using Next-Auth for secure login sessions, which is very effective.

Authorization: Restricting access to certain routes based on user roles.

Input Validation: Preventing injection attacks by sanitizing inputs.

Rate Limiting: Protecting APIs from abuse and excessive requests.

Why it matters:
These measures protect user data, ensure secure transactions, and maintain trust in the platform.

## CI/CD Pipeline

Definition:
CI/CD (Continuous Integration and Continuous Deployment) automates testing, building, and deployment of the application to ensure fast and reliable releases.

Tools:

GitHub Actions: Automates build and deployment workflows.

Docker: Containerizes the application for consistent environments.

Vercel / AWS / Render: Potential platforms for automatic deployment.

