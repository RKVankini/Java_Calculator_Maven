# 🚀 Java Web Calculator (Maven + Docker + Kubernetes + CI/CD)

## 📌 Overview

This project is a **Java-based web calculator application** built using **Maven**, containerized with **Docker**, and deployed using **Kubernetes manifests**.
It also integrates **CI/CD using GitHub Actions**.

The application provides basic arithmetic operations through a web interface.

---

## 🏗️ Architecture

User → Web Browser → Java Web App (Servlet/JSP) → Calculator Logic

* Frontend: JSP (index.jsp)
* Backend: Java Servlet (Calculator.java)
* Build Tool: Maven
* Containerization: Docker
* Deployment: Kubernetes
* CI/CD: GitHub Actions

---

## 🧰 Tech Stack

* Java (Servlets)
* JSP (Java Server Pages)
* Maven
* Docker
* Kubernetes
* GitHub Actions

---

## 📁 Project Structure

```
Java_Calculator_Maven/
│
├── .github/workflows/main.yml   # CI/CD pipeline
├── Dockerfile                   # Docker configuration
├── pom.xml                      # Maven build file
├── manifest/deploy.yaml         # Kubernetes deployment
│
├── src/
│   ├── main/
│   │   ├── java/mypackage/
│   │   │   └── Calculator.java  # Backend logic
│   │   └── webapp/
│   │       ├── index.jsp        # UI
│   │       └── WEB-INF/web.xml  # Servlet config
│   │
│   └── test/
│       └── CalculatorTest.java  # Unit tests
│
└── README.md
```

---

## ⚙️ How to Run Locally

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Java_Calculator_Maven.git
cd Java_Calculator_Maven
```

### 2️⃣ Build using Maven

```bash
mvn clean package
```

### 3️⃣ Run on Tomcat

* Deploy the generated `.war` file into Tomcat
* Access:

```
http://localhost:8080/Java_Calculator_Maven
```

---

## 🐳 Run with Docker

### Build Docker Image

```bash
docker build -t java-calculator .
```

### Run Container

```bash
docker run -p 8080:8080 java-calculator
```

Access in browser:

```
http://localhost:8080
```

---

## ☸️ Kubernetes Deployment

Apply deployment:

```bash
kubectl apply -f manifest/deploy.yaml
```

Check pods:

```bash
kubectl get pods
```

---

## 🔄 CI/CD Pipeline

GitHub Actions workflow:

* Builds the project using Maven
* Can be extended for Docker build & deployment

File:

```
.github/workflows/main.yml
```

---

## 🧪 Testing

Run tests:

```bash
mvn test
```

---

## ✨ Features

* Basic arithmetic operations
* Simple web UI using JSP
* Maven-based build system
* Dockerized application
* Kubernetes deployment support
* CI/CD integration

---

## 📌 Future Improvements

* Add advanced operations (scientific calculator)
* Add REST API
* Integrate database (history tracking)
* Deploy on AWS (EC2 / EKS)

---

## 👨‍💻 Author

Rama Krishna Vankini

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
