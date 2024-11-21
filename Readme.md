# Spring Boot Backend Deployment Guide

## Part 1: Deploying Locally

Prerequisites :
Java Development Kit (JDK 8 or higher) installed.
Maven installed.
Spring Boot application source code or JAR file.

Step 1: Install Java

Verify if Java is installed:

```bash

java -version

```

If Java is not installed, download and install the JDK from Oracle or use a package manager:

```bash

sudo apt update
sudo apt install openjdk-11-jdk -y
```

Verify installation:

```bash
java -version

```

Step 2: Install Maven

Verify if Maven is installed:

```bash
mvn -version

```

If not installed, use the following command:

```bash
sudo apt install maven -y

```

Step 3: Build the Spring Boot Application

Navigate to your Spring Boot project directory:

```bash

cd /path/to/your/project
```

Build the project:

```bash
mvn clean package -Dmaven.test.skip=true

```

After a successful build, the JAR file will be located in the target/ directory (e.g., target/spring-backend-v1.jar).

Step 4: Run the Application

Run the JAR file:

```bash

java -jar target/spring-backend-v1.jar

```

The application will start, and you can access it at:

arduino

http://localhost:8080

Step 5: Keep the Application Running

If you want to keep the application running in the background:

```bash

nohup java -jar target/spring-backend-v1.jar &

```
