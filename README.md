# create-react-app from scratch

This project was built to better understand how react works under the hood.

This project was made following: https://medium.com/@JedaiSaboteur/creating-a-react-app-from-scratch-f3c693b84658

## What stuff does

**Babel**: A transpiler (special type of compiler) that transpiles (converts) modern JavaScript (es6) and jsx into common JavaScript that can be understood by all browsers.

**Webpack**: A static module bundler for modern JS apps. When webpack processes your application, it internally builds a dependency graph from one or more entry points and then combines every module (file) your project needs into one or more bundles, which are static assets to serve your content from. Webpack uses Babel to transpile es6 and jsx into common JS during the build process.

**react**: The react dependency provides us with the ability to define react components and use the react API (e.g. hooks).

**react-dom**: The react-dom provides us with the render function to render our react app in the DOM (our root element in public/index.html). The render function uses a diffing algorithm for efficient updates - it only mutates the DOM as necessary to reflect changes.

## How to use this project

1. `$ git clone https://github.com/DoableDanny/create-react-app-from-scratch`
2. `$ cd create-react-app-from-scratch`
3. Install dependencies: `$ npm i`
4. Start the dev server on localhost:3000: `$ npm run start`

## Scripts

`$ npm run start`: webpack starts up a dev server and will bundle all our react components and css into a single bundle.js file. Webpack uses Babel to transpile the es6 and jsx into common JS that can be understood by all browsers. Webpack stores the bundle.js file in dist/bundle.js in memory, but doesn't actually print it into dist/bundle.js. To output for production, use the below command. Webpack's dev server uses hot reloading and the app can be viewed at localhost:3000.

`$ npm run build`: webpack will create a production-ready bundle.js file and create the file in dist/bundle.js. If you want to output a development build, use the following command: `npx webpack --mode=development`.
