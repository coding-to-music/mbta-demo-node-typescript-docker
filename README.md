# mbta-demo-node-typescript-docker

# 🚀 MBTA API TypeScript demo app, Showing how you can use Node with TypeScript and Pug 🚀

https://github.com/coding-to-music/mbta-demo-node-typescript-docker

From / By https://github.com/selfinterest/mbta_demo


## Environment variables:

```java

```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/mbta-demo-node-typescript-docker.git
git push -u origin main
```

MBTA API TypeScript demo app
===================
This is a demonstration app showing how you can use Node with TypeScript.

Installation
------------
Clone the repo, then:
```
$ npm install
$ npm install -g ts-node typescript
```
That should do it.

Running It
-------------
There are a few different run scripts in the `package.json` file.

`npm start` will start the server in dev mode, using ts-node and nodemon. On every change, ts-node will recompile the code and the server will restart. For this to work, ts-node must be installed globally (as in the instructions above.)

`npm run build` will run the TypeScript compiler over the code and produce a bundle of plain JavaScript that can be run directly using NodeJs. The bundle will be set up in `/dist` directory.

Just for fun, there's an included Dockerfile. It could be used as follows:
```
$ docker build . -t mbta
$ docker run -p 8222:8222 -d mbta:latest
```

TODO
---------
Tests

## npm run start

Returns the next departures for 

```
// Coordinates of Watertown Square (approx.)
const watertownCoords = {
    latitude: "42.36546",
    longitude: "-71.18564"
}
const routeNumber = "71";                   // the number of the Watertown -> Harvard route 

// Read template from file and compile
const template = pug.compile(fs.readFileSync(__dirname + "/assets/view.pug", {encoding: "utf8"}));
```

http://localhost:8222/

```
[

Wednesday, March 22nd 2023, 11:07:00 pm,
Wednesday, March 22nd 2023, 11:31:00 pm,
Wednesday, March 22nd 2023, 11:53:00 pm,
]
```