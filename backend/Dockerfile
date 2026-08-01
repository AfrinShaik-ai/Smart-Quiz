FROM eclipse-temurin:17-jdk

WORKDIR /app

COPY . .

RUN javac -cp "Java-WebSocket-1.5.6.jar:mysql-connector-j-8.0.33.jar:slf4j-api-1.7.36.jar:slf4j-simple-1.7.36.jar" QuizServer.java

CMD ["java", "-cp", ".:Java-WebSocket-1.5.6.jar:mysql-connector-j-8.0.33.jar:slf4j-api-1.7.36.jar:slf4j-simple-1.7.36.jar", "QuizServer"]