<div align="center">
  <h1>🛒 E-Commerce API</h1>
  <p>A modern and scalable backend API for e-commerce, built with Django & DRF, integrating Stripe, JWT, Celery, and Telegram Bot.</p>
  
  ![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
  ![DRF](https://img.shields.io/badge/DRF-red?style=for-the-badge&logo=django&logoColor=white)
  ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
  ![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
  ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
  ![Stripe](https://img.shields.io/badge/Stripe-008CDD?style=for-the-badge&logo=stripe&logoColor=white)
  ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

---

## ✨ Key Features

- ✅ **Stripe Integration** (Test Mode)
- ✅ **JWT Authentication** with **SMS Gateway** support
- ✅ **Telegram Bot** notification system
- ✅ **Asynchronous Tasks** using Celery + Redis + RabbitMQ
- ✅ **Custom Permissions** & Role Management
- ✅ **Django Signals** to handle stock updates
- ✅ **GitHub Actions** for CI/CD automation
- ✅ **Full Testing Suite** for models and views
- ✅ **Secure Environment Handling** with `dotenv`

---

## 🚀 Getting Started

Follow the steps below to set up and run the project on your local environment.

### 🔧 Prerequisites

- Docker & Docker Compose
- Git
- Stripe test account
- Telegram bot token
- SMS gateway credentials

### 📦 Clone the Repository

```bash
git clone https://github.com/Tillayevxusniddin/E-commarce.git
cd E-commarce
```

## 🛠️ Environment Setup

``` bash
# Fill in .env with your credentials
cp .env.example .env
```

## 🐳 Run via Docker
``` bash
# Build and start all services
docker-compose up --build
```

## 👤 Create Superuser
``` bash
docker-compose exec web python manage.py createsuperuser
```

## 🧪 Run Tests
``` bash
docker-compose exec web pytest
```

## 🗃️ Data Management
``` bash
# Dump data from old server
python manage.py dumpdata > data.json

# Clean current DB
python manage.py flush

# Load dumped data
python manage.py loaddata data.json
```

### 🔐 Authentication System
JWT-based authentication
Two-step verification with SMS Gateway

### 💳 Stripe Payment
Stripe test mode integration using PaymentIntent API with secure, PCI-compliant workflows. Use test cards to simulate transactions.

### 🤖 Telegram Bot Integration
Instant notifications are sent to your Telegram bot whenever a new order is placed or updated.

### ⚙️ CI/CD with GitHub Actions
Automated tests on each push
Docker builds and service checks
Ensures consistent quality across environment

### 🤝 Contribution
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

<div align="center"> <p>Project Author: <b>Xusniddin Tillayev</b></p> </div> 
