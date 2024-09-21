## node-express-boilerplate

A boilerplate/starter project for quickly building RESTful APIs using Node.js, Express, and Mongoose.

## Technology Used

* Node.js
* Express
* Mongo
* Redis

## Quick Start / Project Setup

If you would still prefer to do the installation manually, follow these steps:

#1 clone the repo
- git clone git@github.com:kishan-sixberries/node-express-boilerplate.git
- cd node-express-boilerplate

#2 install the dependencies
- npm install

#3 set the environment variables(copy or move env file)
- cp .env.example .env
OR
- mv .env.example .env

#4 open .env and modify the environment variables (if needed)

#5 start project
- npm start

## Table of Contents

- [Features](#features)
- [Commands](#commands)
- [Project Structure](#project-structure)
- [API Documentation](#api-documentation)


## Features

- **NoSQL database**: [MongoDB](https://www.mongodb.com) object data modeling using [Mongoose](https://mongoosejs.com)
- **Authentication and authorization**: using [passport](http://www.passportjs.org)
- **Validation**: request data validation using [Joi](https://github.com/hapijs/joi)
- **Logging**: using [winston](https://github.com/winstonjs/winston) and [morgan](https://github.com/expressjs/morgan)
- **Testing**: unit and integration tests using [Jest](https://jestjs.io)
- **Error handling**: centralized error handling mechanism
- **API documentation**: with [swagger-jsdoc](https://github.com/Surnet/swagger-jsdoc) and [swagger-ui-express](https://github.com/scottie1984/swagger-ui-express)
- **Dependency management**: with [npm](https://www.npmjs.com/)
- **Environment variables**: using [dotenv](https://github.com/motdotla/dotenv) and [cross-env](https://github.com/kentcdodds/cross-env#readme)
- **Security**: set security HTTP headers using [helmet](https://helmetjs.github.io)
- **Santizing**: sanitize request data against xss and query injection
- **CORS**: Cross-Origin Resource-Sharing enabled using [cors](https://github.com/expressjs/cors)
- **Compression**: gzip compression with [compression](https://github.com/expressjs/compression)
- **Code coverage**: using [coveralls](https://coveralls.io)
- **Git hooks**: with [husky](https://github.com/typicode/husky) and [lint-staged](https://github.com/okonet/lint-staged)
- **Linting**: with [ESLint](https://eslint.org) and [Prettier](https://prettier.io)
- **Editor config**: consistent editor configuration using [EditorConfig](https://editorconfig.org)


## Commands

#### Running locally

```bash
npm start
```

## Testing:

#### run all tests

```bash
npm test
```

#### run all tests in watch mode

```bash
npm test:watch
```

#### run test coverage

```bash
npm coverage
```

## Linting:

#### run ESLint

```bash
npm lint
```

#### fix ESLint errors

```bash
npm lint:fix
```

#### run prettier

```bash
npm prettier
```

#### fix prettier errors

```bash
npm prettier:fix
```


## Project Structure

```
src\
 |--config\         # Environment variables and configuration related things
 |--controllers\    # Route controllers (controller layer)
 |--docs\           # Swagger files
 |--middlewares\    # Custom express middlewares
 |--models\         # Mongoose models (data layer)
 |--routes\         # Routes
 |--services\       # Business logic (service layer)
 |--utils\          # Utility classes and functions
 |--validations\    # Request data validation schemas
 |--app.js          # Express app
 |--index.js        # App entry point
```

## API Documentation

To view the list of available APIs and their specifications, run the server and go to `http://localhost:3000/v1/docs` in your browser. This documentation page is automatically generated using the [swagger](https://swagger.io/) definitions written as comments in the route files.

## Postman Collection

https://www.getpostman.com/collections/e292af3e81dd1971c843


## License

[MIT](LICENSE) - Kishan Ghetia (ghetia.kishu@gmail.com)
