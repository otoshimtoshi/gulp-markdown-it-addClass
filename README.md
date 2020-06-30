# gulp-markdown-it-addClass


## Install
``` bash
git clone git@github.com:otoshimtoshi/gulp-markdown-it-addClass.git
```
```
May be usable　package.json
``` json
"gulp-markdown-it-addClass": "git://github.com/otoshimtoshi/gulp-markdown-it-addClass.git"
```

## Usage examples
Then, add it to your gulpfile.js:
``` js
var gulp = require('gulp');
var md = require('gulp-markdown-it');
const mdAddClass = require('gulp-markdown-it-addClass');

gulp.task('default', () => {
  return gulp.src('./src/*.ext')
    .pipe(md(mdAddClass));
});
```
## Output examples
``` html
<a class="markdown-body"></a>
<p class="markdown-body"></p>
<h1 class="markdown-body"></h1>
<ol class="markdown-body"></ol>
<blockquote class="markdown-body"></blockquote>
<table class="markdown-body"></table>
...etc
```