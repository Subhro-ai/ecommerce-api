

---

# 🚀 Ecommerce API with FastAPI Framework

A fully functional Ecommerce API built using **FastAPI** with JWT authentication, PostgreSQL, and robust CRUD operations.

---

## 📚 Table of Contents
- [Demo](#demo)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [API Endpoints](#api-endpoints)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## 🌟 Features
- **Product Management:**  
   CRUD operations for product creation, retrieval, updating, and deletion.
- **User Authentication:**  
   JWT-based secure user authentication and authorization.
- **Cart Management:**  
   Add, remove, and modify cart items with ease.
- **Search & Filter:**  
   Advanced search and filter capabilities to enhance product discovery.
- **Account Management:**  
   Retrieve, update, and delete user account details.
- **API Documentation:**  
   Integrated with Swagger UI and ReDoc for easy API exploration.

---

## 🛠️ Technologies Used
- **FastAPI** – Modern Python web framework with automatic OpenAPI documentation.
- **PostgreSQL** – Reliable relational database for secure data storage.
- **SQLAlchemy** – ORM for seamless interaction between Python objects and SQL.
- **JWT Authentication** – Secure token-based authentication.
- **Pydantic** – Data validation and serialization.
- **Uvicorn** – ASGI server for running FastAPI applications.
- **Supabase** – Real-time database capabilities.

---

## 📡 API Endpoints

### 🛍️ **Product Endpoints**
| Endpoint                 | Method | Path                | Description                        | Access  |
|--------------------------|--------|---------------------|------------------------------------|---------|
| Get all products          | GET    | `/products/`        | Retrieve a list of all products    | User    |
| Create product            | POST   | `/products/`        | Add a new product                  | Admin   |
| Get product by ID         | GET    | `/products/{id}/`   | Retrieve product details by ID     | User    |
| Update product by ID      | PUT    | `/products/{id}/`   | Update product details             | Admin   |
| Delete product by ID      | DELETE | `/products/{id}/`   | Delete a specific product          | Admin   |

---

### 📚 **Category Endpoints**
| Endpoint                  | Method | Path                | Description                        | Access  |
|---------------------------|--------|---------------------|------------------------------------|---------|
| Get all categories         | GET    | `/categories/`      | Retrieve all categories            | User    |
| Create category            | POST   | `/categories/`      | Add a new category                 | Admin   |
| Get category by ID         | GET    | `/categories/{id}/` | Get details of a category by ID    | User    |
| Update category by ID      | PUT    | `/categories/{id}/` | Update category information        | Admin   |
| Delete category by ID      | DELETE | `/categories/{id}/` | Delete a specific category         | Admin   |

---

### 👥 **User Endpoints**
| Endpoint                  | Method | Path                | Description                        | Access  |
|---------------------------|--------|---------------------|------------------------------------|---------|
| Get all users (Admin)      | GET    | `/users/`           | Retrieve all registered users      | Admin   |
| Get user by ID (Admin)     | GET    | `/users/{user_id}/` | Retrieve specific user details     | Admin   |
| Create user (Admin)        | POST   | `/users/`           | Create a new user                  | Admin   |
| Update user by ID (Admin)  | PUT    | `/users/{user_id}/` | Update user details                | Admin   |
| Delete user by ID (Admin)  | DELETE | `/users/{user_id}/` | Delete a specific user             | Admin   |

---

### 🔐 **Authentication Endpoints**
| Endpoint                  | Method | Path                | Description                        | Access  |
|---------------------------|--------|---------------------|------------------------------------|---------|
| User Signup                | POST   | `/auth/signup/`     | Register a new user                | Public  |
| User Login                  | POST   | `/auth/login/`      | Authenticate and get access tokens | Public  |
| Refresh Token               | POST   | `/auth/refresh/`    | Refresh expired access token       | User    |

---

### 📝 **Account Endpoints**
| Endpoint                  | Method | Path                | Description                        | Access  |
|---------------------------|--------|---------------------|------------------------------------|---------|
| Get account info           | GET    | `/account/`         | Retrieve current user info         | User    |
| Edit account info          | PUT    | `/account/`         | Update authenticated user info     | User    |
| Delete account             | DELETE | `/account/`         | Remove authenticated user account  | User    |

---

### 📚 **API Documentation**
| Endpoint                  | Method | Path                | Description                        | Access  |
|---------------------------|--------|---------------------|------------------------------------|---------|
| Swagger UI                  | -      | `/docs/`            | Swagger interface for API testing  | Public  |
| OpenAPI JSON                | -      | `/openapi.json`     | Raw JSON schema                    | Public  |
| ReDoc                       | -      | `/redoc/`           | ReDoc interface for documentation  | Public  |

---

## 📸 Screenshots
> Coming soon! Add relevant screenshots of API responses and Swagger/ReDoc interfaces.

---

## 📦 Installation

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/ecommerce-api.git
```

2. **Navigate to the project directory:**
```bash
cd ecommerce-api
```

3. **Create and activate a virtual environment:**
```bash
# Create virtual environment
python3 -m venv venv

# Activate on Windows
venv\Scripts\activate

# Activate on macOS/Linux
source venv/bin/activate
```

4. **Install dependencies:**
```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

1. **Run Alembic migrations:**
```bash
alembic upgrade head
```

2. **Start the FastAPI server:**
```bash
uvicorn main:app --host 0.0.0.0 --port 8000 --reload
```

---

## 🤝 Contributing
Contributions are welcome! If you'd like to contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit them.
4. Push the branch (`git push origin feature-name`).
5. Submit a pull request.

---

## 📄 License
This project is licensed under the [MIT License](LICENSE).

---

🎉 **Happy Coding!** 🎉

