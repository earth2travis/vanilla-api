# Vanilla Node.js REST API

REST API using Node.js without the Express framework. Full CRUD functionality allowing you to CREATE, READ, UPDATE and DELETE from a `.json` data file. Uses node.js [http](https://nodejs.org/api/http.html) module. Allows you to see what goes on under the hood with Express while manually interacting with the request, response cycle. Uses Model–view–controller (MVC) design pattern where models interact with data (JSON file) and controllers sets up status, routes and methods for interacting with the model.

## Installation

```shell
git clone https://github.com/earth2travis/vanilla-api.git
```

```shell
cd vanilla-api
```

```shell
npm install
```

```shell
npm start
```

## CRUD

- GET `http://localhost:5000/api/products` Gets all products
- GET `http://localhost:5000/api/products/:id` Gets a single product
- POST `http://localhost:5000/api/products` Creates a new product in the format:

```json
{
    "name": "Product Name",
    "description": "Product Description",
    "price": 00.00
}
```

- PUT `http://localhost:5000/api/products/:id` Updates a product in the format (does not have to contain all properties):

```json
{
    "name": "Product Name",
    "description": "Product Description",
    "price": 00.00
}
```

- DELETE `http://localhost:5000/api/products/:id` Removes a product

## Data

- `products.json`

## Dependencies

- [uuid](https://www.npmjs.com/package/uuid) For the creation of RFC4122 UUIDs.

### Dev

- [nodemon](https://www.npmjs.com/package/nodemon) Automatically restarts the node application when file changes in the directory are detected.

## Tools

- [Postman](https://www.postman.com/)

## Possible Improvements

- Reduce route redundancy in `server.js`

## Resources

- Traversy Media [Vanilla Node.js REST API | No Framework](https://www.youtube.com/watch?v=_1xa8Bsho6A)
