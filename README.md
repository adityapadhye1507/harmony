# Harmony

# Introduction

This application is based on a MEAN stack architecture with NodeJS based server, Angular JS based client and MongoDB based database. In order to expose the Restful API’s, NodeJS server needs to be started, which serves the client-side applications as well as the server-side applications.

The database is a MongoDB database, which can be hosted either locally or online. Once the database is configured and actively listening to requests, the node server can be setup and started to start the application.

## Local Deployment

#### Install the minimum dependencies of the project
- Node JS v10.2.1 (https://nodejs.org/en/download/)
- MongoDB v3.6.5 (https://www.mongodb.com/download-center/community)
- NPM v6.1.0 (https://www.npmjs.com/get-npm)
- Bower v1.8.4 (https://bower.io/)

#### Clone Github Repo
Download the project code into a local directory by cloning or downloading the GIT repository: https://github.com/adityapadhye1507/harmony

#### Application Configuration
Configure the application by changing the critical configurations according to your requirements

| File  | Description  |
| :------------ | :------------ |
| ./bin/www  |  File that defines the server configurations |
| ./config/database.js  | File that defines the MongoDB database connection URL  |
|  ./config/keys.js | File that contains Google Client ID and Client Secret  |

#### Steps to run the server
- Using Terminal or Command Prompt, go to the source directory of the project

- Run the following command to install bower and npm components

```shell
cd public
bower install
cd ../admin/public
bower install
cd ..
npm install
```

- After installing the components, start the server with the following command

```shell
npm start
```

- Once the server is up and running, it should host the application on the following routes:
```html
http://localhost:<port> 
http://localhost:<port>/admin/
```

- The ``` <port>``` value will be 3000 if not changed in ./bin/www file.

