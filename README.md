# A Sample Test API Built on Express, Sequelize and Async/ Await Documentation.
[View Screenshot](https://github.com/React7Tech/simple-bulletin-express/blob/master/screenshort01.png)

For Socar Malaysia Test Assessment by JustEd @ R. Aidy.

This SBB project was bootstrapped with:
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

## Async/ Await |  Folder path ./client/src/App.js 
CallApi method was create to interact with GET Express API route, then call this method in componentDidMount and finally set the state to the API response, which fetch '/api/hello' path from express route.
```
componentDidMount() {
    this.callApi()
      .then(res => this.setState({ response: res.express }))
      .catch(err => console.log(err));
  }

  callApi = async () => {
    const response = await fetch('/api/hello');
    const body = await response.json();

    if (response.status !== 200) throw Error(body.message);

    return body;
  };

  handleSubmit = async e => {
    e.preventDefault();
    const response = await fetch('/api/world', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',
      },
      ```
```
## Giving Back

Please Visit my [Website](https://react7.press) to checkout more of my latest development.

-R. Aidy aka JustEd
```
