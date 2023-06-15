# Project Setup - Frontend
***
This guide will walk you through the steps required to set up the frontend part of your Vue application. Follow these instructions to ensure a smooth and hassle-free setup process.
Prerequisites

Before proceeding with the setup, make sure you have the following software installed on your system:

    Node.js (version 12 or higher)
    npm (Node Package Manager) or Yarn

## Step 1: Clone the Repository
***
Start by cloning the project repository from the version control system of your choice (e.g., GitHub, Bitbucket). Open your terminal and execute the following command:

```shell
git clone <repository-url>
``` 

Change <repository-url> to the URL of your project's repository.
## Step 2: Install Dependencies
***
Navigate to the project's root directory using the terminal and install the required dependencies. Run the following command:

```shell
npm install
```

This command will read the package.json file and download all the necessary dependencies listed under the dependencies and devDependencies sections.
## Step 3: Verify Configuration
***
Ensure that the package.json file contains the necessary scripts and dependencies required for the project. Refer to the provided package.json in your project for reference.
## Step 4: Development Mode
***
To start the application in development mode, execute the following command:


```shell
npm run dev
```
  
This command uses the vite build tool to launch the development server and compile your Vue application. By default, the server runs on http://localhost:5173/.

You can now open your web browser and navigate to the specified URL to see your application running.
    
## Step 5: Building for Production
***
When you are ready to deploy your application, you need to build it for production. Run the following command:


```shell
npm run build
```
  
This command generates optimized and minified static assets in the dist directory. These files are ready to be deployed to a production environment.
## Additional Scripts
***
```shell
    npm run test unit
```
Runs unit tests using the @testing-library/vue library.
