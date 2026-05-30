# Networked Video File Transfer System

## Project Overview

Networked Video File Transfer System is a CLI and web-based application for transferring video files over a network.

## Prerequisites

This application was built with Java, Spring Boot, Thymeleaf, and Docker. To run or develop, the following tools are required:

- Docker and Docker Compose
- Java 21 or higher

## Getting Started

Before proceeding, ensure the necessary tools are installed.

## Web Server

The web server handles the receiving and rendering of the video files.

1. Open a terminal and navigate to the project root directory.
2. Build and spin up the environment using Docker Composer.

   ```console
   docker compose up --build
   ```

3. Once the containers are running, access the web interface via ["http://localhost:8080"](http://localhost:8080)

## CLI File Upload

The CLI tool streams data to the backend using network sockets.

1. Open a new terminal window and navigate to the project root directory.
2. Compile the source code:

   ```console
   javac producer/producer.java
   ```

3. Start transmitting video files via:

```console
java producer.Producer NUMBER_OF_THREADS VIDEO_DIRECTORY ...
```
