# 🌱 AgroRoot - Full Stack Agriculture Platform

AgroRoot ek **full-stack web application** hai jo farmers aur agriculture ecosystem ke liye modern digital solutions provide karta hai. Yeh project scalable architecture ke saath design kiya gaya hai jisme frontend aur backend clearly separated hain.


---

# 📌 Table of Contents

* Project Overview
* Features
* Tech Stack
* Project Structure
* System Architecture
* Installation Guide
* Running the Project
* API Communication
* Environment Variables
* Troubleshooting
* Build & Deployment
* Future Improvements

---

# 🌍 Project Overview

AgroRoot ka aim hai agriculture domain ko digitalize karna by providing:

* User-friendly interface
* Fast backend APIs
* Scalable system design
* Real-time interaction capability (extendable)

---

# ✨ Features

### 👨‍🌾 User Features

* Responsive UI
* Fast navigation (Vite powered)
* API-based dynamic data rendering

### ⚙️ System Features

* REST API architecture
* Modular backend structure
* Easy scalability
* Clean separation of frontend & backend

---

# 🧰 Tech Stack

## 🔹 Frontend

* React.js
* Vite
* JavaScript (ES6+)
* CSS

## 🔹 Backend

* Java
* Spring Boot
* Maven
* REST APIs

---

# 📁 Project Structure

```bash
AgroRoot/
│
├── AgroRoot--Frontend-main/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── AgroRoot--Backend-main/
│   ├── src/main/java/
│   ├── src/main/resources/
│   ├── pom.xml
│   └── mvnw
```

---

# 🏗️ System Architecture

```
[ React Frontend ]  --->  [ Spring Boot Backend ]  --->  [ Database (optional/future) ]
        |
        | HTTP (REST API Calls)
        ↓
   JSON Responses
```

---

# ⚙️ Prerequisites

Ensure system me ye installed ho:

| Tool     | Version |
| -------- | ------- |
| Node.js  | 16+     |
| npm/yarn | Latest  |
| Java     | JDK 17+ |
| Maven    | 3.6+    |

Check versions:

```bash
node -v
java -version
mvn -v
```

---

# 🚀 Installation Guide

## 🔽 Step 1: Clone Repository

```bash
git clone <your-repo-url>
cd AgroRoot
```

---

## 🎨 Frontend Setup

### 📂 Navigate

```bash
cd AgroRoot--Frontend-main
```

### 📦 Install Dependencies

```bash
npm install
```

### ▶️ Run Development Server

```bash
npm run dev
```

👉 Runs on:

```
http://localhost:5173
```

---

## 🔧 Backend Setup

### 📂 Navigate

```bash
cd AgroRoot--Backend-main
```

### ▶️ Run Application

#### Windows:

```bash
mvnw.cmd spring-boot:run
```

#### Linux/Mac:

```bash
./mvnw spring-boot:run
```

👉 Runs on:

```
http://localhost:8080
```

---

# 🔗 Frontend ↔ Backend Integration

Frontend backend APIs ko call karta hai via HTTP requests.

### ⚠️ Important:

* Backend must run before frontend
* API URL sahi hona chahiye

Example:

```js
const BASE_URL = "http://localhost:8080";
```

---

# 🔐 Environment Variables

## Frontend (.env)

Create `.env` file in frontend:

```env
VITE_API_BASE_URL=http://localhost:8080
```

Use in code:

```js
import.meta.env.VITE_API_BASE_URL
```

---

## Backend (application.properties)

```properties
server.port=8080
```

---

# 📡 API Communication Flow

1. User frontend pe action karta hai
2. React API call bhejta hai
3. Spring Boot request handle karta hai
4. Response JSON me return hota hai
5. UI update hoti hai

---

# 🐛 Troubleshooting

## ❌ Frontend not starting

* Run: `npm install`
* Check Node version

## ❌ Backend not starting

* Java version check karo
* Maven install verify karo

## ❌ API not working

* Check:

  * Backend running hai?
  * Port correct hai?
  * CORS enabled hai?

---

# 🛠️ Build for Production

## Frontend

```bash
npm run build
```

Output:

```
dist/ folder
```

---

## Backend

```bash
./mvnw clean package
```

Output:

```
target/*.jar
```

Run jar:

```bash
java -jar target/app.jar
```

---

# ☁️ Deployment Guide (Basic)

## Frontend:

* Vercel
* Netlify

## Backend:

* Render
* AWS EC2
* Railway

---

# 🔮 Future Improvements

* Authentication system (JWT)
* Database integration (MySQL/PostgreSQL)
* Role-based access
* Real-time notifications
* AI-based recommendations

---

# 🤝 Contribution

1. Fork repo
2. Create branch
3. Make changes
4. Commit
5. Open Pull Request

---

# 📄 License

This project is intended for learning and development purposes.

---

# 👨‍💻 Author

AgroRoot Development Team

---
