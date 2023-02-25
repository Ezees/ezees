<!DOCTYPE html>
<html>
    <head>
        <title>Empty project</title>
        <meta charset="utf-8">
    </head>
    <body>
        <div id="app"></div>
        <script src="index.js"></script>
    </body>
</html>
console.log("hello world!");
.cache/
coverage/
dist/*
!dist/index.html
node_modules/
*.log

# OS generated files
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db
const webpack = require('webpack');
const path = require('path');

const config = {
  entry: './src/index.js',
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'bundle.js'
  }
};

module.exports = config;