
<p align=center>
   Emploai REST API documentation.
</p>

<p align=center>
   <em>The documentation has been created with node-slate. Check it out at:
   <a href=https://node-slate.js.org>node-slate.js.org</a></em>
</p>


Getting Started with Project
------------------------------

### Prerequisites

You're going to need:

 - **Node.js**

### Getting Set Up

4. Initialize and start local server:

```shell
npm install
npm run build
npm start
```

You can now see the docs at http://localhost:4567. Whoa! That was fast!

### Commands

Compile documentation to static site in `./build`:

```shell
npm run build
```

Run a dev server that live-reloads at http://localhost:4567:

```shell
npm start
```

Publish your docs to `origin/gh-pages` branch:

```shell
npm run deploy
```

Gulp Task
---------

Slate API documentation generation is available as Gulp task with the [gulp-node-slate](https://github.com/center-key/gulp-node-slate) plugin.
