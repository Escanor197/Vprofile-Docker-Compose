# VProfile Multi-Tier Application (Docker Compose)

## 📌 Project Overview

This project demonstrates a complete multi-tier application deployment using Docker Compose.

### Architecture:

* **MySQL** → Database
* **Memcached** → Caching layer
* **RabbitMQ** → Message broker
* **Tomcat** → Java Application
* **Nginx** → Web server (reverse proxy)

---

## 📁 Project Structure

```
.
├── app/
├── db/
├── web/
├── docker-compose.yml
└── README.md
```

---

## 🚀 How to Run

### 1. Clone repo

```bash
git clone https://github.com/AyaHeshmatAbdo/vprofile-docker-compose.git
cd vprofile-docker-compose
```

### 2. Build & Start

```bash
docker-compose up -d --build
```

### 3. Access Application

* App: http://localhost:8080
* Web: http://localhost
* RabbitMQ UI: http://localhost:15672 (guest/guest)

---

## 🛠️ Technologies Used

* Docker
* Docker Compose
* MySQL
* Memcached
* RabbitMQ
* Tomcat
* Nginx
* Maven

---

## 📸 Notes

* The application WAR file is built using Maven inside Docker.
* Database is initialized using `db_backup.sql`.
* Nginx acts as a reverse proxy for the application.
