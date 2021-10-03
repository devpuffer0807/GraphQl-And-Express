# Express, GraphQL example
## How to run the project

Install dependencies:

```shell
yarn

# or using npm

npm install
```

Create `src/config.ts` or rename `src/config.example.js` and update file with your credentials:

```js
export default {
  port: 3010,
  database: {
    type: 'mysql',
    connection: {
      database : '',
      host : '',
      password : '',
      user : '',
    },
    /*
     * Migrations run on every start of the application.
     * If you initialized the database manually (from the database.sql file),
     * you don't need this.
     */
    migrations: {
      directory: __dirname + '/migrations',
    },
  },
};
```

Run the project:

```shell
yarn start

# or using npm

npm start
```

Open GraphiQL in your browser [http://localhost:3010/graphql](http://localhost:3010/graphql)

## Examples

You can find example queries in [EXAMPLES.md](./EXAMPLES.md).

