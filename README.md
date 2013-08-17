# Example: how to compile a modular plugin

This example shows you how to build a JS plugin made of modular components and compile it using [picnicc](https://picni.cc). 

The idea is that each component of the library lies in its own file, which is a good coding practice. People can then choose to download your repo with all its files (dev), or let picnic deliver a compiled version of the library (prod).

You may also simply compile your plugin yourself, and put that compiled version in your repo (this is how the [picnicc.js repo](https://github.com/picnicc/picnicc.js) works).

## The good thing is...
When it comes to perf, you no longer have to worry about breaking your lib into multiple files.

## Custom builds
Once your lib is broken into multiple files (or components, or assets, if you like), it's very easy to let your users pick only the components they're to need.

## And now, time to compile (with one click)

Here, we get in touch with the picnicc API using a simple link. Picnicc will grab our picnicc.json file, and compile the assets listed in it.

### Plain

https://picni.cc/api/v1/build/?username=picnicc&project=simple-compile.js&picnicc=https://raw.github.com/picnicc/example.simple-compile/master/picnicc.json

### Minified

https://picni.cc/api/v1/build/?username=picnicc&project=simple-compile.js&picnicc=https://raw.github.com/picnicc/example.simple-compile/master/picnicc.json&minify=js



