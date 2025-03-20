# Bootstrap-Sandbox

## Initial Configuration for a Webpack x Babel x Bootstrap:

npm init -y

## Dependencies:

- npm install webpack webpack-cli webpack-dev-server --save-dev
- npm install @babel/core @babel/preset-env @babel/preset-react babel-loader --save-dev
- npm install css-loader sass sass-loader mini-css-extract-plugin postcss postcss-loader --save-dev
- npm install autoprefixer --save-dev

## To import Bootstrap in our index.js:

```
import "bootstrap/dist/css/bootstrap.min.css";
import "bootstrap";
```

## To use autoprefixer and ensure CSS compatibility in all browsers:

In our postcss.config.js file--

```
module.exports = {
  plugins: {
    autoprefixer: {},
  },
};
```

## Creating our own running commands with NPM:

In our package.json--

```
"scripts": {
  "build": "webpack --mode production",
  "start": "webpack serve --mode development --open"
}
```

## To run our programe

`npm start`
