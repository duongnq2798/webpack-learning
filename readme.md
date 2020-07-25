# Way to bundle in webpack 4

`webpack src/index.js --output dist/bundle.js --mode development`
`Usage without config file: webpack <entry> [<entry>] --output [-o] <output>`

- And if you are using `webpack.config.js`

```
const path = require('path');

module.exports = {
  mode: 'development',     // set mode option, 'development' or 'production'
  entry: './src/index.js',
  output: {
    path: path.resolve(__dirname,'dist'),
    filename: "bundle.js"
  }
};
```
