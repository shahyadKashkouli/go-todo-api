# 📝 Go To-Do API

A simple RESTful To-Do List API built with **Go**, **Gorilla Mux**, **GORM**, and **MySQL**.

## 🚀 Features

- Add, view, update, and delete tasks
- RESTful routing using Gorilla Mux
- MySQL database connection with GORM ORM
- Clean, modular structure

## 📦 Technologies Used

- [Go](https://golang.org/)
- [Gorilla Mux](https://github.com/gorilla/mux)
- [GORM](https://gorm.io/)
- [MySQL](https://www.mysql.com/)

🔧 Install Dependencies
Before running the project, make sure you have Go installed (v1.16 or above).
Then install the required dependencies using go get:

```bash
go get -u github.com/gorilla/mux
go get -u gorm.io/gorm
go get -u gorm.io/driver/mysql
```

## ⚙️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/shahyadKashkouli/go-todo-api.git
cd go-todo-api
```

## 📂 Setup MySQL Database

```bash

CREATE DATABASE IF NOT EXISTS to_do_list;
USE to_do_list;
CREATE TABLE tasks (
    Id INT UNSIGNED NOT NULL AUTO_INCREMENT PRIMARY KEY,
    Name VARCHAR(255),
    Detail TEXT,
    Deadline INT UNSIGNED
);
```


## 💬 Example Request (POST /addtask)

```bash
{
  "Id": 1,
  "Name": "Finish homework",
  "Detail": "Complete math and science chapters",
  "Deadline": 20250430
}

```
## 📄 License
This project is licensed under the MIT License.


