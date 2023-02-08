npm init -y 
npm i json-server
make db.json and paste data
create server.js

------------>const jsonServer = require("json-server"); // importing json-server library
const server = jsonServer.create();
const router = jsonServer.router("db.json");
const middlewares = jsonServer.defaults();
const port = process.env.PORT || 3001; // you can use any port number here; i chose to use 3001

server.use(middlewares);
server.use(router);

server.listen(port);


---------->

create .gitignore  node_modules

update package json===========

{
  "name": "render1",
  "version": "1.0.0",
  "description": "mockserver app",
  "main": "server.js",
  "scripts": {
    "start": "node server.js"
  },
  "keywords": [],
  "author": "alok",
  "license": "ISC",
  "dependencies": {
    "json-server": "^0.17.1"
  }
}
---------------------
create a repo and link it to folder




