# Set up dotenv

## Install

```js
npm install dotenv
```

## Usage

1. Create a .env file

   ```js
   NODE_ENV = "development";
   PORT = "3001";
   ```

2. Call variables in server.js
   server.js

   ```js
   //server.js
   require("dotenv").config();
   console.log(process.env.PORT);
   console.log(process.env.NODE_ENV);
   ```

3. Run server.js

   ```js
   node server.js
   // 3001
   // development
   ```

## Preload

1. Added start script in `package.json`

```js
"scripts": {
    "start": "node -r dotenv server.js"
}
```

2. Run script

```js
npm run start
// 3001
// development
```

### References:

- [npm: dotenv](https://www.npmjs.com/package/dotenv)
