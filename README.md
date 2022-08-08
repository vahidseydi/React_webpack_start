## if you want to use this framework, you won't need to repeat the below lines!

the structure is like this:

```
📦React_webpack_start

 ┣ 📂public
 ┃ ┗ 📜index.html
 ┣ 📂src
 ┃ ┣ 📂imgs
 ┃ ┣ 📜App.css
 ┃ ┣ 📜App.js
 ┃ ┗ 📜index.js
 ┣ 📜.babelrc
 ┣ 📜.gitignore
 ┣ 📜package.json
 ┣ 📜README.md
 ┣ 📜webpack.config.js
 ┗ 📜yarn.lock
```

## to create it from scratch:

- to use **yarn** we install it by npm _install --global yarn_

- update dependencies in the package.json
  then using 'npm install OR yarn', all listed packages will be installed

- **scripts**: some comments are listed in the scripts property to compile the project in the different modes(dev/ prod/ ...)

### A brief reference to the dependencies we have written

- **webpack**: lets us bundle the JavaScript applications and other images, fonts and ...

#### we need to config webpack and for this reaaon webpack.config.js is created:

- **context**: where are we? \_dirname (points to project folder)

- **entry**: which file is the main one? src/index.js

- **output**: where are we goinf to bundle? the folder 'build' in the file bundle.js

- **devServer**: development environment with Webpack and should ONLY be used for development.

- **module**: In this section, the property rule specifies which file extensions should be loaded with which file loaders

  - to load js family files we use **babel-loader** (it needs configuring the property of preset that we do in the .**babelrc** file)

    - to load css we use css-loader and style-loader

- **plugins**: HtmlWebpackPlugin is uded to simplifies the creation of HTML files to serve the webpack bundles

#### other adjusments:

- some fonts are brought from google fonts(inter)

- we added App.css to define some styles
