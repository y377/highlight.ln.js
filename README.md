[highlightjs代码高亮](https://github.com/highlightjs/highlight.js)官方推荐插件，jekyll适配版，个人强烈推荐
==================================================================================

> 本人菜鸟，不太会JavaScript和css/sass，勉强捣鼓html,但是我会修改，我就用jekyll、bootstrap、highlightjs和highlight.ln.js终于“拼凑”起来了，敬请期待完工后的效果   
![image](https://user-images.githubusercontent.com/58632405/146037176-ffb9f3e4-984d-4de4-a143-199f7614372b.png)
# Thank the [original author](https://github.com/taufik-nurrohman) for writing such a good plug-in
# 非常感谢[原作者](https://github.com/taufik-nurrohman)写出这么好的插件并且帮助我修改

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
