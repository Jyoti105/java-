# Java Student Management System

A Java 17 project demonstrating Jenkins CI automation on Windows.

## Technologies
- Java 17
- Apache Maven
- JUnit 5
- Jenkins Pipeline
- Git and GitHub

## Features
- Add students
- View all students
- Search students by ID
- Update student details
- Delete students
- Validate student information
- Prevent duplicate student IDs

> This demonstration stores data in memory; it does not use a database.

## Prerequisites
- JDK 17
- Apache Maven 3.9+
- Git
- Jenkins with Pipeline and JUnit support

## Run locally

Check installations:

    java -version
    mvn -version
    git --version

Compile:

    mvn clean compile

Run tests:

    mvn test

Package:

    mvn package

Run application:

    java -jar target/student-management-1.0.0.jar

## Jenkins setup
1. Push this project to GitHub.
2. Create a Jenkins Pipeline job.
3. Choose **Pipeline script from SCM**.
4. Select **Git** and enter your repository URL.
5. Set branch to `*/main` and Script Path to `Jenkinsfile`.
6. Save and click **Build Now**.
7. Review Console Output, test results, and archived JAR artifacts.

## Expected result
- Application compiles successfully.
- All 8 unit tests pass.
- `target/student-management-1.0.0.jar` is created.
- Jenkins publishes JUnit results and archives the JAR.

## GitHub push commands

Run these from the project root after creating an empty GitHub repository:

    git init
    git add .
    git commit -m "Add Java student management project"
    git branch -M main
    git remote add origin https://github.com/YOUR_USERNAME/java-student-management-jenkins.git
    git push -u origin main

Replace `YOUR_USERNAME` with your GitHub username.
