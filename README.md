
# grunt-develop - [![Build Status](https://secure.travis-ci.org/edwardhotchkiss/grunt-develop.png)](http://travis-ci.org/edwardhotchkiss/grunt-develop)

> Grunt Task to run a Node.js Server while developing, auto-reloading on change.

## Notes:

  * Requires Grunt >= 0.4.0
  * No need to modify/export your server or alter your applications code.**

## Install

```bash
$ npm install grunt-develop
```

## Setup Gruntfile.js:

```javascript

module.exports = function(grunt) {

  grunt.initConfig({
    develop: {
      server: {
        file: 'app.js'
      }
    }
  });

  grunt.loadNpmTasks('grunt-develop');

  // if you are also using "watch", place after
  grunt.registerTask('default', ['develop','watch']);

};

```

## Usage (Realtime development with restart on file changes)

```bash
$ grunt
```

## License (MIT)

Copyright (c) 2013, Edward Hotchkiss.

## Author: [Edward Hotchkiss][0]

[0]: http://github.com/edwardhotchkiss/
