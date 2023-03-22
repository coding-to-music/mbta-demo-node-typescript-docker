# mbta-demo-node-typescript-docker

# 🚀 MBTA API TypeScript demo app, Showing how you can use Node with TypeScript. 🚀

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