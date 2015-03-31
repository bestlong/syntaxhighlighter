# Technical details about <pre> and <textarea></h1>

== Problem description ==

The fundamental problem with using <pre> is inability to easily copy and paste code into it. In particular this applies to XML/HTML.

The problem with <pre> is that browsers parse HTML inside it where as in <textarea> they do not. For example:

```
<pre><b>Hello</b></pre>
```

Will render as *Hello*, where as

```
<textarea><b>Hello</b></textarea>
```

will render as <b>Hello</b>.

If you try to get HTML from <pre> using innerHTML property, it's not going to look anything like what you have originally in the HTML file. With <textarea> however, a property value would return your HTML exactly the same way as you have provided it.

== Conclusion ==

This brings me to the final point. With <textarea> you can copy and paste source code without any alterations. *With <pre> you have to make sure your source code won't be recognized as HTML, which means you have to replace every opening triangular bracket < with it's HTML encoded version &lt;. This is enough to make <pre> work fine.*