# pug (was jade) loader for webpack

The original project is [here](https://github.com/webpack/jade-loader). Since jade has been renamed to pug, jade will no longer be supported.

## Usage

``` javascript
var template = require("pug!./file.pug");
// => returns file.pug content as template function
```

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

### Embedded resources

Try to use `require` for all your embedded resources, to process them with webpack.

``` pug
div
  img(src=require("./my/image.png"))
```

You need to configure loaders for these filetypes too. (Take a look at the [file-loader](https://github.com/webpack/file-loader).)

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
