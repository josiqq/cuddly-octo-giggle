## Installation

```bash
$ npm install
```

## Build 
```bash
$ npm run build
```

## Usage

```bash
$ npm run dev
```

## Configuration of database
```js
// db/connection.ts
import * as mysql from 'mysql';

const connection = mysql.createConnection({
  host: process.env.DB_HOST,
  user: process.env.DB_USER,
  password: process.env.DB_PASSWORD,
  database: process.env.DB_NAME,
});
```

Change the `process.env` variables in `.env` file.


## Environment variables
- `SECRET_KEY` - secret key for JWT
- `PORT` - port to run the server on
- `DB_HOST` - database host
- `DB_USER` - database user
- `DB_PASSWORD` - database password
- `DB_NAME` - database name

## Dependencies

- [express](https://github.com/expressjs/express)
- [mysql](https://github.com/mysqljs/mysql)
- [nodemon](https://github.com/remy/nodemon)
- [cors](https://github.com/expressjs/cors)
- [bcrypt](https://github.com/kelektiv/node.bcrypt.js)
- [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken)
- [morgan](https://github.com/expressjs/morgan)
- [dotenv](https://github.com/motdotla/dotenv)
- [ts-node](https://github.com/TypeStrong/ts-node)