# [gulp](https://github.com/gulpjs/gulp)-yaml

[![npm version](https://badge.fury.io/js/gulp-yaml.svg)](http://badge.fury.io/js/gulp-yaml)
[![Build Status](https://travis-ci.org/crissdev/gulp-yaml.svg?branch=master)](https://travis-ci.org/crissdev/gulp-yaml)
[![Dependency Status](https://david-dm.org/crissdev/gulp-yaml.svg)](https://david-dm.org/crissdev/gulp-yaml)

> A [Gulp](https://github.com/gulpjs/gulp) plugin to sort [YAML](http://en.wikipedia.org/wiki/YAML) using [js-yaml](https://github.com/nodeca/js-yaml).


## Install

```sh
npm install --save-dev gulp-yaml
```

## Usage

```js
var yaml = require('gulp-yaml');

gulp.src('./src/*.yml')
  .pipe(yaml({ schema: 'DEFAULT_SAFE_SCHEMA' }))
  .pipe(gulp.dest('./dist/'))

gulp.src('./src/*.yml')
  .pipe(yaml({ space: 2 }))
  .pipe(gulp.dest('./dist/'))

gulp.src('./src/*.yml')
  .pipe(yaml({ safe: true }))
  .pipe(gulp.dest('./dist/'))
```
