[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

# React Tutorial with added New Relic

## New Relic specific stuff:

* `npm install newrelic --save`
* `cp node_modules/newrelic/newrelic.js .`
* Edit newrelic.js to set app name and to pull license key from environment: `process.env.NEW_RELIC_LICENSE_KEY`
* Edit the server.js to add `require newrelic` at the top
* Set the license key and run: `NEW_RELIC_LICENSE_KEY=YOUR_LICENSE_KEY_HERE node server.js`



This is the React comment box example from [the React tutorial](http://facebook.github.io/react/docs/tutorial.html).

## To use

There are several simple server implementations included. They all serve static files from `public/` and handle requests to `/api/comments` to fetch or add data. Start a server with one of the following:

### Node

```sh
npm install
node server.js
```

### Python

```sh
pip install -r requirements.txt
python server.py
```

### Ruby
```sh
ruby server.rb
```

### PHP
```sh
php server.php
```

### Go
```sh
go run server.go
```

### Perl

```sh
cpan Mojolicious
perl server.pl
```

And visit <http://localhost:3000/>. Try opening multiple tabs!

## Changing the port

You can change the port number by setting the `$PORT` environment variable before invoking any of the scripts above, e.g.,

```sh
PORT=3001 node server.js
```
