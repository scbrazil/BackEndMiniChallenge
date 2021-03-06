# BackEndMiniChallenge

Use this repo to practice writing RESTful CRUD routes. Simulate client interactions using Postman <a href="https://www.postman.com/downloads/">Postman</a>. The goal of this mini challenge is to make all tests pass and practice <a href="http://expressjs.com/en/guide/error-handling.html">error handling</a> in an express server. See requirements section below for challenge details.

### Installation

To get started:

Navigate to the project Directory

```sh
$ cd BackEndMiniChallenge
```

Install the dependencies

```sh
$ npm install
```

In a new terminal, seed the database

```sh
$ mysql -u root -p < schema.sql
```

Start the server

```sh
$ npm run start
```

Before running the tests, create and use the test database

```sh
$ CREATE DATABASE pets_info_test
$ USE pets_info_test
```

Run the tests

```sh
$ npm run test
```

### Requirements

| METHOD | PATH          | DESCRIPTION                                            |
| ------ | ------------- | ------------------------------------------------------ |
| GET    | /api/pets     | respond with all the pets                              |
| GET    | /api/pets/:id | respond with single pet, based on req.params.id        |
| POST   | /api/pets     | inserts new pet record from req.body                   |
| PUT    | /api/pets/:id | updates a pet record from req.body                     |
| PATCH  | /api/pets/:id | updates specific section of a pet record from req.body |
| DELETE | /api/pets/:id | deletes a pet record based on req.params.id            |

### Technologies

<table style="width:50%">
  <tr>
    <td><a href="http://expressjs.com">Express</a></td>
     <td><a href="https://www.mysql.com/">MySQL</a></td>
    <td><a href="https://jestjs.io/">Jest</a></td>
    <td><a href="https://www.npmjs.com/package/supertest">Supertest</a></td>

  </tr>
</table>
