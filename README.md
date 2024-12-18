# docker-test

# Docker Practical Test: Deploy a Node.js Application

# Objective
You are tasked to containerize and deploy a simple Node.js application using Docker. Your goal is to:
1. Create a functional Dockerfile.
2. Use Docker Compose for deployment.
3. Verify the deployment and log output.

---

# Files Provided
- **`app/package.json`**: Node.js application dependencies.
- **`app/server.js`**: Simple web server.

---

# Tasks

# 1. Containerize the Application
- Create a `Dockerfile` that:
  1. Uses `node:18-alpine` as the base image.
  2. Sets `/app` as the working directory.
  3. Copies the application files (`package.json` and `server.js`) into the container.
  4. Installs dependencies using `npm install`.
  5. Exposes port `3000`.
  6. Runs the app using `npm start`.

- Build the image using:
  ```bash
  docker build -t docker-test-app .
