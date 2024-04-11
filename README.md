
# Blogpost (blog api)


<a href="https://nodejs.org/" target="_blank"><img src="https://res.cloudinary.com/djvfnekle/image/upload/v1710009760/f05i1vkplc2j3ft5hxoj.png" width="50"  alt="Nestjs Image" /></a>
<a href="https://www.mongodb.com/" target="_blank"><img src="https://res.cloudinary.com/djvfnekle/image/upload/v1710009753/clo5kbdsb1mlfczslpn7.png" width="50"  alt="MongoDb image" /></a>
<a href="https://www.docker.com/" target="_blank"><img src="https://res.cloudinary.com/djvfnekle/image/upload/v1710009749/pebtirzmkqmputt8o0pf.png" width="50"  alt="Docker imahe" /></a>
<a href="https://www.typescriptlang.org/" target="_blank"><img src="https://res.cloudinary.com/djvfnekle/image/upload/v1710009761/otj7i99gcvkj6moeok54.png" width="50"  alt="Typescript image" /></a>


## Description


[Node Mongodb UserManagement](https://github.com/codeboosts/nodejs-mongodb-usermanagement): Secure & Efficient Starter <br>
Kickstart your Nodejs project with robust user management, built-in email OTP authentication and fully user management, and adherence to best practices. This comprehensive starter template provides a solid foundation to simplify development and ensure security.


## Requirements
Before running this project, ensure you have the following requirements:
- <a href="http://nodejs.org" target="_blank">Node.js</a> 18.x.x or later
- <a href="https://www.mongodb.com/" target="_blank">Mongo DB</a>
- <a href="https://redis.io/" target="_blank">Redis</a>
- <a href="https://yarnpkg.com/" target="_blank">Yarn (pkg manager)</a>



## Installation
You can install dependencies using Yarn, which is preferred for better performance and reliability:
```bash
yarn install
```


## Running the app
```bash
# development & watch
$ yarn dev
# build
$ yarn build
```



## Environment Variables
Ensure you have a `.env` file in the root directory of the project with the following variables:
```dotenv
PORT=8080
SALT_ROUND=''
REDIS_URI=''
DB_URI=''
DB_NAME=''
JWT_SECRET=''
SMTP_EMAIL=''
SMTP_PASS=''
```



## Docker Compose (Optional)
You can also run the project using Docker Compose. Ensure you have Docker installed on your system.
To start the project with Docker Compose, run the following command:
```bash
docker-compose up
```
<b>(Make sure you also install "docker-credential-helper" and "docker-compose")</b>


For more information on installing Docker Compose, refer to the [official installation guide](https://docs.docker.com/compose/install/).


## APIs
User Management
```bash
# Register
 $ *POST* /user/register
# Login
 $ *POST* /user/login
# Email Verification
 $ *POST* /user/verify-email
# My Info
 $ *GET* /user/me
# Send OTP
 $ *POST* /user/send-otp
# Forgot Password
 $ *POST* /user/forgot-password
# Reset Password
 $ *PUT* /user/reset-password
# Delete User
 $ *DELETE* /user
# Change Password
 $ *PUT* /user/change-password
# Update User
 $ *PUT* /user/update
# Change Email
 $ *PUT* /user/change-email
```

## Author

- Author - [Zeshan Shakil](https://zeshantech.netlify.app)

## License

Nodejs MongoDB UserManagement is [MIT licensed](LICENSE).
