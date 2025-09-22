
# Node.js CI/CD Pipeline

## Overview
This repository demonstrates a simple **CI/CD pipeline** for a Node.js application using **GitHub Actions**. The pipeline automatically installs dependencies, runs tests, and builds a Docker image whenever changes are pushed to the `main` branch.

---

## Project Structure

MyNodeApp/
│ index.js.js ← Node.js application
│ package.json ← Dependencies and scripts
│ testapp.test.js.js ← Test file
│ docker-compose.yml ← Optional Docker compose file
│ .gitignore ← Files to ignore in Git
└─ .github/
└─ workflows/
└─ main.yml ← GitHub Actions CI/CD workflow


---

## CI/CD Workflow

- **Trigger:** Push to `main` branch  
- **Steps:**
  1. Checkout the repository
  2. Set up Node.js environment
  3. Install dependencies (`npm install`)
  4. Run tests (`npm test`)
  5. Build Docker image locally

> The workflow ensures that all commits are tested and a Docker image is built automatically.

---

## How to Run Locally

1. Clone the repository:

```bash
git clone https://github.com/reddi-1218/nodejs-ci-cd-pipeline.git
cd MyNodeApp

Install dependencies:
npm install


Run tests:
npm test

Build Docker image (optional):
docker build -t my-node-app .


GitHub Actions
Workflow file: .github/workflows/main.yml
Automatically runs CI/CD on every push to main.
Logs and results are available in the Actions tab of this repository.
