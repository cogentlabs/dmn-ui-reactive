# UI for Dynamic Memory Networks

This repository contains only Web UI for the Dynamic Memory Networks. 

Implementation of DMN you can found in [YerevaNN/Dynamic-memory-networks-in-Theano](https://github.com/YerevaNN/Dynamic-memory-networks-in-Theano)

Beside of that you can run a fake server which documentation can be found [here](server/README.md).

## Development


### Dependencies
In order to run DMN UI you should install Node.js. After that you will need to install bower and gulp.
```bash
$ npm install -g bower gulp
```

Now, if everything was successful you should be able to run the following command to install other dependencies.

```bash
$ npm install
$ bower install
```

### Run
You need to seed DB for the fake API server and run it.

```bash
$ node server/seed-db > server/db.json
$ node server
```

After that you can serve your files. Files will be served under  [http://localhost:3000](http://localhost:3000).

```bash
gulp serve
```

## Build

If you want to build your files (create production ready version) you should run:

```bash
$ gulp build
```

Built files will be located at /dist, you can serve them using your favorite static server. 
If you want to serve them using fake server you can run:

```bash
$ node server
```

And navigate to [http://localhost:3003](http://localhost:3003).

