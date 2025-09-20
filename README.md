# Multi-Cloud Microservices Application

[![Docker](https://img.shields.io/badge/Docker-Container-blue?logo=docker)](https://www.docker.com/)
[![MySQL](https://img.shields.io/badge/MySQL-Database-blue?logo=mysql)](https://www.mysql.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?logo=mongodb)](https://www.mongodb.com/)
[![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws)](https://aws.amazon.com/)
[![GCP](https://img.shields.io/badge/GCP-Cloud-red?logo=googlecloud)](https://cloud.google.com/)

This project is a **full-stack microservices application** demonstrating a **scalable architecture** with **multi-cloud deployment** support across **AWS and GCP**. It is ideal for software engineering students, developers, and organizations exploring **microservices, containerization, and cloud deployment best practices**.

---

## Tech Stack

* **Backend:** Spring Boot (Java)
* **Frontend:** React (TypeScript, Tailwind CSS)
* **Databases:** MySQL (Course Service), MongoDB (Student Service)
* **Containerization:** Docker, Docker Compose
* **Cloud Platforms:** AWS, GCP
* **Build Tools:** Maven, npm

---

## Features

* **Modular Microservices Architecture:** Independent, modular services for scalability.
* **Dockerized Services:** Backend services and databases run in Docker containers for portability.
* **Polyglot Persistence:** MySQL for `Course Service` and MongoDB for `Student Service`.
* **Modern Frontend:** Built with React, TypeScript, and Tailwind CSS.
* **Multi-Cloud Deployment:** Seamless deployment to AWS and GCP.
---

## Getting Started

Follow these steps to run the application locally.

### Prerequisites

* **Java JDK 21+:** For backend.
* **Node.js & npm:** For frontend.
* **Docker & Docker Compose:** For containers.
* **AWS RDS Instance / GCP Cloud SQL:** For MySQL database (Course Service).

### Steps

1. **Clone the Repository**
```bash
git clone https://github.com/yasith-chathuranga/enterprise-cloud-architecture.git
cd enterprise-cloud-architecture
```

2. **Configure Spring Boot Application Properties**  
   Update `course-service` properties depending on your cloud provider:

**GCP Example (`application-gcp.properties`):**
```properties
spring.datasource.host=<YOUR_GCP_CLOUD_SQL_INSTANCE_IP>
spring.datasource.port=<YOUR_GCP_DB_PORT>
spring.datasource.url=jdbc:mysql://${spring.datasource.host}:${spring.datasource.port}/eca_courses?createDatabaseIfNotExist=true
spring.datasource.username=<YOUR_GCP_DB_USERNAME>
spring.datasource.password=<YOUR_GCP_DB_PASSWORD>
```

4. **Run the Frontend**
```bash
cd frontend-app
npm install
npm run dev
```
Open in browser: `http://localhost:5173`

---

## Demo Video

See how the **Course Service** is set up and runs on **GCP**

[![Watch the GCP Demo](https://img.shields.io/badge/Watch-GCP%20Demo-blue?style=for-the-badge&logo=googlecloud)](https://drive.google.com/file/d/1-FqPlCYFBqLsqXvndF72l5bFOjcLrlIH/view?usp=sharing)

---

## Deployment

* **AWS:** RDS (MySQL), EC2 instances, and S3 for media storage.
* **GCP:** Cloud SQL (MySQL), VM instances, and GCS buckets for media storage.
---

## License

This project is licensed under the **[MIT LICENSE](LICENSE)**.

---
## Author

| Name              | Student ID   | Email               |
|-------------------|--------------|---------------------|
| Yasith Chathuranga | 2301682017 | yasithchathuranga999@gmail.com |


<div align="center">
<a href="https://www.docker.com/" target="_blank"><img src="https://img.shields.io/badge/Docker-100000?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Badge" /></a>
<a href="https://aws.amazon.com/" target="_blank"><img src="https://img.shields.io/badge/AWS-100000?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS Badge" /></a>
<a href="https://cloud.google.com/" target="_blank"><img src="https://img.shields.io/badge/GCP-100000?style=for-the-badge&logo=googlecloud&logoColor=white" alt="GCP Badge" /></a>
<a href="https://spring.io/projects/spring-boot" target="_blank"><img src="https://img.shields.io/badge/Spring%20Boot-100000?style=for-the-badge&logo=spring&logoColor=white" alt="Spring Boot Badge" /></a>
<a href="https://reactjs.org/" target="_blank"><img src="https://img.shields.io/badge/React-100000?style=for-the-badge&logo=react&logoColor=white" alt="React Badge" /></a>
<a href="https://tailwindcss.com/" target="_blank"><img src="https://img.shields.io/badge/Tailwind%20CSS-100000?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS Badge" /></a>
<a href="https://www.mysql.com/" target="_blank"><img src="https://img.shields.io/badge/MySQL-100000?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL Badge" /></a>
<a href="https://www.mongodb.com/" target="_blank"><img src="https://img.shields.io/badge/MongoDB-100000?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB Badge" /></a>
</div>

<br>
<p align="center">
  &copy; 2025 Yasith Chathuranga
</p>