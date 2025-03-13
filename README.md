# URL Shortener Service

A **scalable URL shortener** designed to offer efficient URL aliasing and insightful analytics. Built using **Go**, **PostgreSQL**, **ClickHouse**, **MongoDB**, and **Redis**.

## Table of Contents

- [Features](#features)
- [System Architecture](#system-architecture)
- [API Endpoints](#api-endpoints)
- [Installation Guide](#installation-guide)
  - [Prerequisites](#prerequisites)
  - [Setup Instructions](#setup-instructions)
- [Usage](#usage)
  - [Accessing the Service](#accessing-the-service)
  - [Analytics and Metrics](#analytics-and-metrics)
- [Local Development Setup](#local-development-setup)

---

## Features

- **Generate Short URLs**: Create unique and concise aliases for long URLs.
- **Advanced Analytics**: Track and analyze URL usage with real-time metrics, including redirects, user interaction, and performance.
- **Scalable Infrastructure**: Horizontal scalability using Docker Compose for easy deployment and management.
- **Persistent Storage**: Utilize PostgreSQL and ClickHouse for efficient storage and analytics, with Redis caching for high-speed performance.
- **Easy Setup with Docker**: All services are containerized for quick local setup and deployment.

---

## API Endpoints

### **Create Short URL Alias**

- **Endpoint**: `POST /url`
- **Description**: Creates a short alias for a given URL.
- **Request Body**:  
  ```json
  {
    "url": "https://github.com/"
  }
