# An API Skeleton

### The project

This is a simple skeleton with an easy structure for developing APIs with Node.js. This project includes the following dependency modules:

- Express
- Sequelize
- bcryptjs
- JWT

As for development dependencies, the modules are the following:

- ESLint with Airbnb's defaults
- Prettier
- Nodemon
- Sucrase
- Sequelize CLI

It also contains a default `users`migration with a basic information.

### Configuration

As soon as you install it, modify `config/database.js` file and choose your preferred database and fill up the credentials.

```js
module.exports = {
  dialect: '[postgres|mysql|mssql|mariadb|sqlite]',
  host: 'localhost',
  username: '',
  password: '',
  database: '',
  define: {
    timestamps: true,
    underscored: true,
    underscoredAll: true,
  },
}
```

Check [Sequelize's Dialects section](http://docs.sequelizejs.com/manual/dialects.html) to know the necessary modules for it to work with your chosen dialect.

### Linting

It comes with ESLint and Prettier using Airbnb's code style with a few alterations located in `.prettierrc`:

```json
{
  "singleQuote": true,
  "trailingComma": "es5",
  "semi": false
}
```
