# Go-BookStore
# Go Bookstore API

A simple REST API for managing books using Go and MySQL.

## 📌 Features
- CRUD operations for books
- MySQL database integration
- RESTful API using Gin framework
- GORM for database handling

## 🛠 Tech Stack
- **Go** (Golang)
- **Gin** (HTTP framework)
- **GORM** (ORM for MySQL)
- **MySQL** (Database)

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/go-bookstore.git
cd go-bookstore
```

### 2️⃣ Install Dependencies
```sh
go mod tidy
```

### 3️⃣ Configure MySQL Database
Create a MySQL database:
```sql
CREATE DATABASE go_bookstore;
```
Update `pkg/config/app.go` with your database credentials:
```go
dsn := "user:password@tcp(127.0.0.1:3306)/go_bookstore?parseTime=true"
```

### 4️⃣ Run the Project
```sh
go run cmd/main/main.go
```

## 📖 API Endpoints

| Method | Endpoint        | Description        |
|--------|----------------|--------------------|
| GET    | `/books`       | Get all books     |
| GET    | `/books/:id`   | Get book by ID    |
| POST   | `/books`       | Add a new book    |
| PUT    | `/books/:id`   | Update book info  |
| DELETE | `/books/:id`   | Delete a book     |

## 📝 License
This project is open-source and available under the **MIT License**.

