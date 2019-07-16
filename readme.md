Originating from a [blog post](http://jamesthom.as/blog/2018/08/07/machine-learning-in-node-dot-js-with-tensorflow-dot-js/) and [gist](https://gist.github.com/jthomas/145610bdeda2638d94fab9a397eb1f1d) by [@jthomas](https://github.com/jthomas), here is a script to run image classification through NodeJS via TensorFlow.js using the MobileNet classifier, being modified for reasons explained in [my own blog post](https://sean12697.github.io/blog/2019/07/15/mobilenet-in-nodejs.html) (from the original gist).

### Requirements

Ensure you have [node-gyp](https://github.com/nodejs/node-gyp) installed, which you can read documentation for through GitHub. This is needed to compile TensorFlow.js from Python to NodeJS, meaning during running `npm i` it will error without it installed.

### Usage

Through the terminal, run `node script.js mobilenet/model.json image.jpg`, `image.jpg` being the location and name of the image you want to classify.