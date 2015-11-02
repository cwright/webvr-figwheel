

# `webvr-figwheel`

This is a modification of [threejs-figwheel](https://github.com/cassiel/threejs-figwheel) that adds WebVR functionality, by way of [webvr-boilerplate](https://github.com/borismus/webvr-boilerplate)
you can livecode to cardboard enabled devices and desktop based HMDs simultaneously. 
It's pretty neat. 

The instructions below from the threejs-figwheel README should work fine for setup, however I recommend 

     rlwrap lein figwheel

for a better REPL experience, if you're into that sort of thing.

You will need [leiningen](http://leiningen.org/) if you haven't worked with clojurescript before.

licence info at the bottom.

# threejs-figwheel README


An example project which brings up a minimal "live coding" environment for Clojure-based WebGL in the browser, courtesy of [ClojureScript](https://github.com/clojure/clojurescript), [three.js](http://threejs.org/) and [Figwheel](https://github.com/bhauman/lein-figwheel).

This is basically the Figwheel template project in Leiningen, with the core ClojureScript file set up to do some three.js, and a stripped-down `index.html` to host the results. The HTML also wheels in three.js from a CDN (so alter to taste).

Most of the effort in this project has gone into making the application state as nearly idempotent as possible, so that repeated page or code reloads don't result in multiple canvas instances, background rendering callbacks, and so on. The reloading is done by completely tearing down the canvas and rendering pipeline and rebuilding; for a proper live coding environment, or for bigger projects, this probably needs to be a bit more subtle.

This project is partially inspired by [this by Chris McCormick](https://github.com/chr15m/clojurescript-threejs-playground), [Henry Garner's Multisnake](https://github.com/henrygarner/multisnake), and [Chestnut](https://github.com/plexus/chestnut).

## Setup (from Figwheel docs)

To get an interactive development environment run:

    lein figwheel

and open your browser at [localhost:3449](http://localhost:3449/).
This will auto compile and send all changes to the browser without the
need to reload. After the compilation process is complete, you will
get a Browser Connected REPL. An easy way to try it is:

    (js/alert "Am I connected?")

and you should see an alert in the browser window.

To clean all compiled files:

    lein clean

To create a production build run:

    lein cljsbuild once min

And open your browser in `resources/public/index.html`. You will not
get live reloading, nor a REPL. 

## License
threejs-figwheel is
Copyright © 2015 Nick Rothwell, nick@cassiel.com.

Distributed under the Eclipse Public License either version 1.0 or (at your option) any later version.



webvr-boilerplate is included unmodified from its bower install and is distributed under the Apache 2.0 licence. 
threejs-figwheel's license info is at the bottom of this page from it's original readme.

webvr-figwheel is 
Copyright © 2015 Colin Wright,  

Distributed under the Eclipse Public License either version 1.0 or (at your option) any later version.

let me know if I'm doing this wrong. 