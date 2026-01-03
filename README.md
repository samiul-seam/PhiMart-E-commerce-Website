# PhiMart – E-Commerce REST API (Django REST Framework)

PhiMart is a backend e-commerce REST API built using **Django REST Framework (DRF)**.  
It provides core e-commerce functionalities such as product management, categories, carts, orders, and product reviews.  
Authentication is handled using **JWT** via **Djoser**, and all API endpoints are documented using **Swagger (drf_yasg)**.

---

## 🚀 Features

- User authentication & authorization using **JWT**
- Product & category management
- Shopping cart system
- Order creation & management
- Product reviews & ratings
- Secure API endpoints
- Interactive API documentation with Swagger

---

## 🛠️ Tech Stack

- **Backend Framework:** Django, Django REST Framework
- **Authentication:** JWT (Djoser)
- **Database:** SQLite
- **API Documentation:** drf_yasg (Swagger & ReDoc)
- **Language:** Python 3

---

## 📦 Installed Packages

- `django`
- `djangorestframework`
- `djoser`
- `djangorestframework-simplejwt`
- `drf-yasg`

---

## 📁 API Modules

- **Products** – Manage product data
- **Categories** – Product categorization
- **Cart** – Add, update, and remove cart items
- **Orders** – Place and track orders
- **Reviews** – Product reviews and ratings
- **Authentication** – User registration, login, logout, token refresh

---

## 🔐 Authentication

PhiMart uses **JWT-based authentication** implemented with **Djoser**.

### Authentication Endpoints
- User Registration
- User Login
- Token Refresh
- Logout

JWT tokens must be included in request headers:

```http
Authorization: Bearer <access_token>
```

---

## 📖 API Documentation (Swagger)

Swagger UI is available for interactive API testing and exploration.

- **Swagger UI:**  http://127.0.0.1:8000/swagger/


- **ReDoc UI:**  http://127.0.0.1:8000/redoc/


---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/samiul-seam/PhiMart
cd PhiMart
```
### 2. Create Virtual Environment
```
python -m venv phi_env
source phi_env/bin/activate   # Linux / Mac
phi_env\Scripts\activate      # Windows
```
### 3. Install Dependencies
```
pip install -r requirements.txt
```
### 4. Configure Environment Variables
```ini
Create a `.env` file and configure the following variables:

SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=your_database_url
ALLOWED_HOSTS=localhost,127.0.0.1
EMAIL_HOST=your_email_host

```
### 5. Apply Migrations
```
python manage.py makemigrations
python manage.py migrate
```
### 6. Create Superuser
```
python manage.py createsuperuser
```
### 7. Run the Server
```bash
python manage.py runserver
```

## 🧩 Project Purpose

PhiMart was developed as a learning-focused e-commerce backend project to practice:
- REST API design
- JWT-based authentication
- Modular Django app structure
- API documentation using Swagger
