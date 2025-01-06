# Laravel REST API Project  

This project demonstrates a **production-ready REST API** built with **Laravel 11**, showcasing modern development practices, clean code, and scalability. It highlights adherence to industry best practices such as **DRY**, **SOLID**, and **Separation of Concerns**, ensuring maintainable and efficient development.  

## 🚀 Features  
- **CRUD Operations**:  
  - Fully implemented CRUD functionality for:  
    - `Role`  
    - `IpList`  

- **Modern Development Practices**:  
  - Use of **Traits**, **Services**, and **Enums** for reusable and maintainable code.  
  - Standardized request validation and resource management.  

- **JWT Token Authentication**:  
  - Secure authentication for protected API endpoints.  

- **Clean Architecture**:  
  - Modular, scalable, and developer-friendly design.  

- **Custom Middleware**:  
  - Middleware for request preprocessing and security.  

- **Adherence to Principles**:  
  - **Object-Oriented Programming (OOP)**  
  - **DRY** (Don’t Repeat Yourself)  
  - **SOLID Design Principles**  

## 🛠️ Setup Instructions  

Follow the steps below to set up and run the project locally:  

### 1. Clone the Repository  
```bash  
git clone https://github.com/caelusweb3/laravel-11-restapi.git  
```  

### 2. Install Dependencies  
Navigate to the project directory and install the required dependencies:  
```bash  
cd laravel-11-restapi
composer install  
```  

### 3. Configure Environment  
Create a `.env` file and generate the application key:  
```bash  
cp .env.example .env  
php artisan key:generate  
```  

### 4. Database Setup  
Open the `.env` file and configure your database credentials:  
```env  
DB_CONNECTION=mysql  
DB_HOST=127.0.0.1  
DB_PORT=3306  
DB_DATABASE=your_database_name  
DB_USERNAME=your_username  
DB_PASSWORD=your_password  
```  

Run the migrations and seed the database:  
```bash  
php artisan migrate --seed  
```  

### 5. Start the Server  
Run the development server:  
```bash  
php artisan serve  
```  

Access the application at:  
```  
http://localhost:8000  
```  

---

## 📖 API Documentation  

### Authentication  
- Use **JWT Token Authentication** for all protected routes.  
- Obtain a token by logging in or registering, and include it in the `Authorization` header for authenticated requests:  
  ```  
  Authorization: Bearer YOUR_TOKEN_HERE  
  ```  

### CRUD Endpoints  
#### Roles:  
- `GET /api/v1/roles` - List all roles.  
- `POST /api/v1/roles` - Create a new role.  
- `PUT /api/v1/roles/{id}` - Update a specific role.  
- `DELETE /api/v1/roles/{id}` - Delete a specific role.  

#### IpList:  
- `GET /api/v1/iplist` - List all IP addresses.  
- `POST /api/v1/iplist` - Add a new IP address.  
- `PUT /api/v1/iplist/{id}` - Update a specific IP address.  
- `DELETE /api/v1/iplist/{id}` - Delete a specific IP address.  

---

## 🗂️ Code Structure  

### Key Directories  
- **App/Http/Controllers**: Handles API request logic.  
- **App/Services**: Encapsulates business logic for reusability.  
- **App/Traits**: Houses reusable methods shared across the app.  
- **App/Enums**: Centralized enumerations for constants.  
- **App/Http/Middleware**: Custom middleware for request handling.  
- **App/Http/Requests**: Validates and sanitizes incoming requests.  
- **App/Http/Resources**: Transforms models into structured JSON responses.  

### Security Highlights  
- **JWT Token Authentication** for secure access.  
- Comprehensive request validation and error handling.  

---

## 📦 Scalability and Maintainability  
This project is designed with modularity and extensibility in mind. Adding new features or modifying existing ones is simple due to its clean and organized architecture.  

---

## 🌟 Future Improvements  
- Add more unit and feature tests for comprehensive test coverage.  
- Integrate **Swagger/OpenAPI** documentation for better API exploration.  
- Implement advanced features like caching, rate-limiting, and queue jobs.  

---

## 📝 License  
This project is licensed under the MIT License. See the `LICENSE` file for more details.  
