# Timezone

Timezone is an application aimed at helping remote teams by making it easier
to see where and **when** their coworkers are.

[Live demo](http://timezone.djfarrelly.com)

# Setup

You must have [Node.js](http://nodejs.org/) and [Browserify](http://browserify.org/)
installed on your system to compile the project assets. After install Node.js, run:

```bash
  $ npm install -g browserify
```

Update your `people.js` file with the appropriate information. Timezone codes
for the `tz` field can be found here: http://momentjs.com/timezone/.

To run the server and download all depdencies for the project run this in the
project root directory:

```bash
  $ npm install
```

`bundle.js` contains all of the necessary scripts and data for the client.
To create this file with Browserify run:

```bash
  $ npm run build
```

Now to start the server on localhost:3000 you can run:

```bash
  $ node ./index.js
```

# Deploy

This project is designed with a Procfile to deploy to a Heroku instance. Please
check with Heorku's up to date documentation for any latest changes. You should
be able to commit your changes in your forked repo then run:

```bash
  $ heroku create
  $ git push heroku master
```

**Note:** These docs are very basic and need some more love. I'll add more info
soon  :)
