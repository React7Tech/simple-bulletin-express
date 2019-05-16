# A Sample Test API Built on Express, Sequelize and Async/ Await Documentation.

For Socar Malaysia Test Assessment by JustEd @ R. Aidy.

This simple-bulletin-express project 
```
was bootstrapped with:
[https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta/css/bootstrap.min.css](https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta/css/bootstrap.min.css).

> Example on using bootstrap.min.css with a Node Express for the frontend(client)

## Usage

Install [nodemon](https://github.com/remy/nodemon) globally

```
npm i nodemon -g
```

Install server and client dependencies

```
yarn
cd client
yarn
```

To start the server and client at the same time (from the root of the project)

```
yarn dev
```

Running the production build on localhost. This will create a production build, then Node will serve the app on http://localhost:5000

```
NODE_ENV=production yarn dev:server
```

## How this works

The key to use an Express backend with a project created with `create-react-app` is on using a **proxy**. We have a _proxy_ entry in `client/package.json`

```
"proxy": "http://localhost:5000/"
```

This tells Webpack development server to proxy our API requests to our API server, given that our Express server is running on **localhost:5000**

## Giving Back

Please Visit my [Website](https://react7.press) to checkout more of my latest development.

-R. Aidy aka JustEd
