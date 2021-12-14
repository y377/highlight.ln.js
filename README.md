Line Number Plugin for [Highlight.js](https://github.com/highlightjs/highlight.js)
==================================================================================

![highlight.ln.js](https://user-images.githubusercontent.com/1669261/83881420-d0d1be00-a76a-11ea-935f-754a67b3cd5a.png)

[Demo](https://taufik-nurrohman.github.io/highlight.ln.js/index.html)

Usage
-----
## for jekyll

you need custom css/scss:

```css
pre .hljs[style]:first-child {
  background: black !important;
  border-right-color: cyan !important; /* here to change the border color */
  color: white !important;
}
```
### Browsers

~~~ .html
<script src="highlight.min.js"></script>
<script src="highlight.ln.min.js"></script>
<script>
hljs.initHighlighting();
</script>
~~~

### ES6 Modules (TODO)

~~~ .js
import hljs from 'highlight.js/lib/core';
import css from 'highlight.js/lib/languages/css';

import {highlightWithLineNumbers} from 'highlight.ln.js';

hljs.registerLanguage('css', css);

const highlighted = hljs.highlight('css', '#foo { bar: baz; }');
const highlightedMarkup = highlightWithLineNumbers(highlighted);
~~~

License
-------

BSD
