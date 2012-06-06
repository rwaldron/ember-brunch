# Brunch with Ember (WIP)
This is a simple ember skeleton for [Brunch](http://brunch.io/).

## Getting started

Clone the repo and run `npm install` & `brunch build`.
See more info on the [official site](http://brunch.io)

## Overview

    config.coffee
    server.coffee
    package.json
    README.md
    /app/
      assets/
        index.html
        img/
          glyphicons-halflings-white.png
          glyphicons-halflings.png
      templates/
      models/
      views/
      controllers/
      templates.js
      models.js
      views.js
      controllers.js
      app.js
      initialize.js
    /vendor/
      scripts/
        jquery.js
        console-helper.js
        ember-latest.js
        handlebars-1.0.0.beta.6.js
        bootstrap.js
      styles/
        bootstrap.css
    /public/
      img/
      stylesheets/
      javascripts/
    /test/
      spec.coffee
    /generators/
      model.js
      view.js
      controller.js

* `config.coffee` contains configuration of your app. You can set plugins /
languages that would be used here.
* `app/assets` contains images / static files. Contents of the directory would
be copied to `public/` without change.
Other `app/` directories could contain files that would be compiled. Languages,
that compile to JS (coffeescript, roy etc.) or js files and located in app are 
automatically wrapped in module closure so they can be loaded by 
`require('module/location')`.
* `app/templates.js`, `app/models.js`, `app/views.js`, and `app/controllers.js` are loaded in `initialize.js` and are responsible for loading their respective classes.
* `test/` contains unit tests.
* `vendor/` contains all third-party code. The code wouldn’t be wrapped in
modules, it would be loaded instantly instead.

This all will generate `public/` (by default) directory when `brunch build` or `brunch watch` is executed.

## Other
Versions of software the skeleton uses:

* jQuery 1.7.2
* Ember latest
* Bootstrap 2.0.4
