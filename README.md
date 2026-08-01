# Smart Quiz – Video Supervised

A real-time quiz application built **from scratch** in Java with WebSocket support and video supervision.  
Frontend is pure HTML/CSS/JS.

---

## Features
- Real-time quiz via WebSockets.
- Webcam recording during the quiz.
- Dynamic question selection.
- Instant answer feedback.
- Results storage with timestamp.
- Video upload per session.

---

## Prerequisites
- Java 17+
- MySQL database with schema `smart_quiz`
- Required JAR files (download separately):
  - [Java-WebSocket-1.5.6.jar](https://github.com/TooTallNate/Java-WebSocket)
  - [slf4j-api-1.7.36.jar](https://www.slf4j.org/download.html)
  - [slf4j-simple-1.7.36.jar](https://www.slf4j.org/download.html)
  - [mysql-connector-j-8.0.33.jar](https://dev.mysql.com/downloads/connector/j/)

---

## Setup MySQL
1. Create a database called `smart_quiz`.
2. Import tables `qst` and `ans` as used in the code.
3. Update DB credentials in `QuizServer.java`:
```java
conn = DriverManager.getConnection(
  "jdbc:mysql://localhost:3306/smart_quiz?serverTimezone=UTC",
  "root",
  "your_password_here"
);
