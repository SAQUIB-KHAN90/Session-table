# React Project Setup and Deployment Guide

This guide provides step-by-step instructions for setting up a React project locally and deploying it on an AWS EC2 instance.

## 1. Setting Up the React Project Locally

Install Node.js and npm:

```bash

sudo apt update
sudo apt install nodejs npm -y

```

Verify installation:

```bash

node -v
npm -v

```

Create a React Application

Use npx to create a React app:

```bash

npx create-react-app react-frontend

```

Navigate to the project directory:

```bash
cd react-frontend

```

Run the React Application Locally

Install dependencies:

```bash
npm install

```

Start the development server:

```bash
npm start

```

Build the React Application

```bash
npm run build

```

The production-ready files will be available in the build/ directory.
