[highlightjs代码高亮](https://github.com/highlightjs/highlight.js)官方推荐插件，jekyll适配办
==================================================================================

![image](https://user-images.githubusercontent.com/58632405/146037176-ffb9f3e4-984d-4de4-a143-199f7614372b.png)
# Thank the original author for writing such a good plug-in

如何使用？how t use？
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

```html
<script src="https://cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.3.1/build/highlight.js"></script>
<script src="/your_path/highlight.ln.js"></script>
<script>
  hljs.highlightAll();
  hljs.configure({ ignoreUnescapedHTML: true });//防止什么注入攻击？
</script>
```

License
-------

BSD
