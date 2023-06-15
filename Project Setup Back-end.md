# Project Setup - Backend
***
This guide will walk you through the steps required to set up the backend part of your Adviser GetGames API microservice. Follow these instructions to ensure a smooth and hassle-free setup process.
Prerequisites

Before proceeding with the setup, make sure you have the following software installed on your system:

    Node.js (version 12 or higher)
    npm (Node Package Manager) or Yarn

## Step 1: Clone the Repository
***
Start by cloning the project repository from the version control system of your choice (e.g., GitHub, Bitbucket). Open your terminal and execute the following command:


```shell
git clone https://github.com/Phantom-works/Adviser-GetGames-API.git
```
This will clone the repository to your local machine.
## Step 2: Install Dependencies
***
Navigate to the project's root directory using the terminal and install the required dependencies. Run the following command:



```shell
npm install
```
This command will read the package.json file and download all the necessary dependencies listed under the dependencies and devDependencies sections.
## Step 3: Configure Environment Variables
***
Create a .env file in the project's root directory and provide the required environment variables, following the following example:

```.env
TWITCH_CLIENT_ID=11111111111
CLIENT_SECRET=1111111111
TWITCH_APP_ACCESS_TOKEN=
```

## Step 4: Start the Server
***
To start the backend server, run the following command:


```shell
npm run build
```
This will launch the Express server and start listening for incoming requests.
## Additional Scripts
***
To run the tests for the backend, execute the following command:
```shell
npm test
```
