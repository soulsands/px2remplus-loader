# px2remplus-loader

same as [px2rem-loader](https://github.com/Jinjiang/px2rem-loader)



## Install

`npm i @soulsandz/px2remplus-loader -D`

## webpack config

```js
module.exports = {
  // ...
  module: {
    rules: [{
      test: /\.css$/,
      use: [{
        loader: 'style-loader'
      }, {
        loader: 'css-loader'
      }, {
        loader: 'px2rem-loader',
        // options here
        options: {
          remUnit: 75,
          ignoreSelector: 'cube'  // the selector will be ignore if it contains the string
        }
      }]
    }]
  }
}
```

Please see [px2rem](https://github.com/songsiqi/px2rem) for more information about query parameters of px2rem.

