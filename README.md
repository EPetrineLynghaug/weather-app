# Lecture Notes: Managing Secrets in a Web Application

## Introduction
In this lecture, we’ll learn how to securely hide an API key. This method offers the best possible protection when handling sensitive data in the browser. 

## Task Overview
The following steps outline how to set up your project, secure your API key, and deploy your app using Git and Netlify:

1. Set up the project with Git.
2. Lock sensitive files.
3. Fetch the API key.
4. Create Netlify functions to hide the key.
5. Hide the API key in your code.
6. Test the application locally.
7. Push the code to GitHub.
8. Deploy the app on Netlify.
9. Test the deployed application.

## Netlify CLI
<details>
  <summary><strong>Click to read more</strong></summary>

Netlify CLI is a tool that allows you to run and test your app locally before deploying it. Here are some key features:

- **Local Deployment**: Use Netlify CLI to test your app in a local environment, mimicking the live deployment on Netlify.
- **Direct Deployment**: You can deploy straight to Netlify, bypassing Git completely if needed.
- **Local Development Environment**: CLI acts as a local development environment to test and build your app.
- **Environment Variables**: It allows you to set environment variables locally.
- **SSH Setup**: Log in securely with SSH keys to manage deployments and projects.
- **Create Secret Functions**: Use it to set up secret Netlify functions and call them as needed in your app.

</details>

## Netlify Functions
<details>
  <summary><strong>Click to read more</strong></summary>

In this project, the `fetch-weather` file is your backend function. It is where we’ll render the data and handle the API key securely using Netlify functions. The magic happens here—by using `fetch` in a Node environment, the API key is kept hidden, and the process functions similarly to how you’d normally use `fetch` in a frontend.

- A constant `api_key` will be stored, and the function will make a GET request to retrieve the data, completely obscuring the key.
  
</details>

## Features
<details>
  <summary><strong>Click to read more</strong></summary>

- **API Key Security**: The API key is hidden within the backend, ensuring it is not exposed in the client-side code.
- **Netlify Function Integration**: The app uses serverless Netlify functions to securely fetch data without exposing sensitive information.
- **Local Development and Testing**: Netlify CLI provides a streamlined workflow for testing everything locally before deployment.

</details>

## Setup
<details>
  <summary><strong>Click to read more</strong></summary>

To run and test the app, ensure you have the following installed:

- Git
- Node.js
- Netlify CLI (to set up local functions and deploy)

### Steps:
1. Clone the repository using Git.
2. Install the dependencies with `npm install`.
3. Create a Netlify function to handle the API key.
4. Set up environment variables in Netlify CLI to hide the API key.
5. Test the app locally using Netlify CLI.

</details>

## Conclusion on Secure API Key Management
<details>
  <summary><strong>Click to read more</strong></summary>

By using Netlify functions and CLI, you can securely hide API keys and other sensitive data in your web applications. This method ensures that no secrets are exposed in the browser while still allowing smooth deployment and testing.

</details>