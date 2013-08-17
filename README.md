# Example: how to compile a modular plugin

## The gist

This example shows you how to build a JS plugin made of modular components and compile it using [picnicc](https://picni.cc). 

The idea is that each component of the library lies in its own file, which is a good coding practice. People can then choose to download your repo with all its files (dev), or let picnic deliver a compiled version of the library (prod).

You may also simply compile your plugin yourself, and put that compiled version in your repo (this is how the [picnicc.js repo](https://github.com/picnicc/picnicc.js) works).

## Compile (with one click)

Here, we get in touch with the [picnicc API](https://picni.cc/api/v1) using a simple link (params are located in the query string). Picnicc will grab our picnicc.json file, and compile the assets listed in it.

That's it.

### Plain
[compile](https://picni.cc/api/v1/build/?username=picnicc&project=simple-compile.js&picnicc=https://raw.github.com/picnicc/example.simple-compile/master/picnicc.json&if_success=302)


### Minified
[compile](https://picni.cc/api/v1/build/?username=picnicc&project=simple-compile.js&picnicc=https://raw.github.com/picnicc/example.simple-compile/master/picnicc.json&if_success=302&minify=js)

## The good thing is...
When it comes to perf, you no longer have to worry about breaking your lib into multiple files.

## Custom builds
Once your lib is broken into multiple files (or "components", or "assets", if you like), it's very easy to let your users pick only the components they're going to actually need. Picnicc was built to do just that.





