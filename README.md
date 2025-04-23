# 🌱 Spring Boot + Maven Beginner Exercise

## 📘 Level 1 - Spring & Maven Exercise

This project is a first hands-on exercise using **Spring Boot** and **Maven** to create a simple REST API.

---

## ⚙️ Project Setup

Generated from [Spring Initializr](https://start.spring.io/) with the following configuration:

- **Project**: Maven
- **Language**: Java
- **Spring Boot**: Latest stable version
- **Java Version**: 11 or higher
- **Packaging**: Jar

### 🧾 Project Metadata

| Property        | Value                             |
|----------------|-----------------------------------|
| **Group**       | `cat.itacademy.s04.t01.n01`       |
| **Artifact**    | `S04T01N01`                       |
| **Name**        | `S04T01N01`                       |
| **Description** | `S04T01N01`                       |
| **Package**     | `cat.itacademy.s04.t01.n01`       |

### 📦 Dependencies

- Spring Web 🌐  
- Spring Boot DevTools 🔧

---

## 🛠 Configuration

Edit `src/main/resources/application.properties` to include:

```properties
server.port=9000

---

## 🚀 Functionality

This application is a REST API that contains two endpoints located in a controller class called `HelloWorldController`, under the package:

cat.itacademy.s04.t01.n01.controller

---

### 📍 Endpoints

#### 1. `/HelloWorld` (GET)

- Accepts a query parameter `name`
- Defaults to `"UNKNOWN"` if not provided
- Returns:  
  `Hello, [name]. You are running a Maven project.`

---

##### 🔗 Examples:

http://localhost:9000/HelloWorld http://localhost:9000/HelloWorld?name=My%20name

#### 2. `/HelloWorld2/{name}` (GET)

- Accepts a **path variable** `name` (optional)
- If no name is provided, should return `"UNKNOWN"`

##### 🔗 Examples:

http://localhost:9000/HelloWorld2 http://localhost:9000/HelloWorld2/MyName

---

## 🧾 Example Output

```text
Hello, UNKNOWN. You are running a Maven project.
Hello, John. You are running a Maven project.

---

## 📂 Project Structure

S04T01N01
├── src
│   ├── main
│   │   ├── java
│   │   │   └── cat.itacademy.s04.t01.n01
│   │   │       └── controller
│   │   │           └── HelloWorldController.java
│   │   └── resources
│   │       └── application.properties
├── pom.xml
└── README.md



