https://medium.com/dev-genius/create-react-app-from-scratch-using-webpack-fa6e41f15289
https://reactjs.org/docs/create-a-new-react-app.html#create-react-app
https://github.com/brillout/awesome-react-components
https://reactjs.org/community/courses.html

npm i react react-dom

<!-- We are using webpack to bundle our project. Webpack will compile our code to one single bundle which can be injected to our template html before serving it in the web.
 -->
npm i -D webpack webpack-cli webpack-dev-server html-webpack-plugin

We need webpack-cli to run webpack command line interface, webpack-dev-server to run local server, and html-webpack-plugin to create a html template to serve our bundle.


We need quite a bit of dependencies from babel which is used to transpile our modern javascript code into browser friendly format. Without the use of babel we cannot run our ES6 javascript within the browser. It also makes our code backward compatible in older version of browsers.
npm i -D @babel/core @babel/preset-env @babel/preset-react babel-loader

Now, we will install few dependencies which will help us to process css files. We will need to install style-loader and css-loader. This is needed for webpack to deal with css and style files. 

npm i -D style-loader css-loader

The --save-dev option allows you to save packages under the devDependencies object in your package. json file. Any packages listed under the devDependencies will not be installed when you are in the production environment. For example, a test runner like karma won't be needed for the production build.


