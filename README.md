# gulp-markdown-it-additionalClass
markdown-it customClass add javascript

import this customRules

``` js
const mdAdd = require('gulp-markdown-it-additionalClass');
```

``` js
gulp.task('default', () => {
  return gulp.src("")
    .pipe(markdown(mdAdd))
});
```
or

``` js
gulp.task('default', () => {
  return gulp.src("")
    .pipe(markdown(config))
});

const config = {
  plugins: [ mdAdd, plugins...... ]
}
```

++example++
``` html
<a class="markdown-body"></a>
<p class="markdown-body"></p>
<h1 class="markdown-body"></h1>
<ol class="markdown-body"></ol>
<blockquote class="markdown-body"></blockquote>
<table class="markdown-body"></table>
...etc
```