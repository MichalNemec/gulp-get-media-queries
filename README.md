# gulp-combine-media-queries

fork from ```https://github.com/konitter/gulp-combine-media-queries```

## Install

```
npm install gulp-combine-media-queries --save-dev
```

## Usage (babel-core)
```javascript
import cmq from 'gulp-combine-media-queries';

gulp.task('make-queries', () => {
  return gulp.src('app/styles/main.css')
    .pipe(cmq({
      log: true,
      use_external: true
    }))
    .pipe(gulp.dest('.tmp/queries'));
});

## Usage
```javascript
var cmq require('gulp-combine-media-queries');

gulp.task('make-queries', () => {
  return gulp.src('app/styles/main.css')
    .pipe(cmq({
      log: true,
      use_external: true
    }))
    .pipe(gulp.dest('.tmp/queries'));
});
```

## Options

### log

Type: `boolean` Default: `false`

Log processed media queries.

### use_external

Type: `boolean` Default: `false`

Writes media queries into external file, named as [src].responsive.css

## License

(MIT License)

Copyright (c) 2014 [konitter](http://re-dzine.net/)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
