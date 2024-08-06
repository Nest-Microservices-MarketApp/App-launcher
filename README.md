# MarketApp - Launcher

<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

<p align="center">This is a App for handling MarketApp client requests. It is built with <a href="http://nestjs.com" target="blank">NestJS</a>, <a href="https://www.typescriptlang.org/" target="blank">Typescript</a>, <a href="https://www.postgresql.org/" target="blank">PostgreSQL</a>, <a href="https://www.mongodb.com/" target="blank">MongoDB</a>, <a href="https://www.prisma.io/" target="blank">Prisma</a>, <a href="https://jwt.io/" target="blank">JWT</a>, <a href="http://www.passportjs.org/" target="blank">Passport</a>, <a href="https://swagger.io/" target="blank">Swagger</a> and <a href="https://nats.io/" target="blank">Nats</a>.</p> 
</p>

## Description

This project uses Git submodules to manage external dependencies. Below are the steps to clone and build the project correctly.

## Developer Settings

To configure and run this project in your local environment, follow these steps:

1. **Clone the repository** to your local machine:

   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Initialize and update submodules:**

   ```bash
   git submodule update --init --recursive
   ```

3. Create a `.env` file in the root of the project. You can refer to the included `.env.template` file. Make sure you fill out all the required variables.

   ```bash
   cp .env.template .env
   ```

4. **Run the application in development mode**:

   ```bash
   docker-compose up --build
   ```

## Swagger Documentation

The API documentation can be accessed at `http://${HOST}:${PORT}/api/docs`. This is a Swagger documentation that provides information about the API endpoints and how to use them.

## Technologies Used

- **NestJS**: A progressive Node.js framework for building efficient, reliable, and scalable server-side applications.
- **TypeScript**: A strongly typed programming language that builds on JavaScript, giving you better tooling at any scale.
- **Nats**: A lightweight and highly performant messaging system that is used for communication between services.
- **Docker**: A platform for developing, shipping, and running applications in containers.
- **PostgreSQL**: A powerful, open-source object-relational database system.
- **MongoDB**: A general-purpose, document-based, distributed database built for modern application developers and for the cloud era.
- **Prisma**: A modern database toolkit that makes it easy to work with databases in Node.js and TypeScript.
- **JWT**: A standard for access tokens that allows you to verify the identity of the user.
- **Passport**: An authentication middleware for Node.js that is extremely flexible and modular.
- **Swagger**: A tool that helps you design, build, document, and consume RESTful web services.

### Important Notes

If you work in the repository that has the submodules, first update and push to the submodule and then to the main repository.

If it is done the other way around, the references of the submodules in the main repository will be lost and we will have to resolve conflicts.
