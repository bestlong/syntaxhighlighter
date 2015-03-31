# Usage #

## Placing the code ##

Place your code on the page and surround it with `<pre>` tag. Set `name`
attribute to `code` and `class` attribute to one of the [language aliases](Languages.md) you wish to use.

```
<pre name="code" class="c-sharp">
... some code here ...
</pre>
```

**NOTE:** One important thing to watch out for is opening triangular bracket `<`. It must be replaced with an HTML equivalent of `&lt;` in all cases. Failure to do won't break the page, but might break the source code displayed.

An alternative to `<pre>` is to use `<textarea>` tag. There are no problems with `<` character in that case. The main problem is that it doesn't look as good as `<pre>` tag if for some reason JavaScript didn't work (in RSS feed for example).

```
<textarea name="code" class="c#" cols="60" rows="10">
... some code here ...
</textarea>
```

## Extended configuration ##

There's a way to pass a few [configuration options](Configuration.md) to the code block. It's done via colon separated arguments.

```
<pre name="code" class="html:collapse">
... some code here ...
</pre>
```

## Making it work ##

Finally, to get the whole thing to render properly on the page, you have to add JavaScript to the page.

```
<link type="text/css" rel="stylesheet" href="css/SyntaxHighlighter.css"></link>
<script language="javascript" src="js/shCore.js"></script>
<script language="javascript" src="js/shBrushCSharp.js"></script>
<script language="javascript" src="js/shBrushXml.js"></script>
<script language="javascript">
dp.SyntaxHighlighter.ClipboardSwf = '/flash/clipboard.swf';
dp.SyntaxHighlighter.HighlightAll('code');
</script>
```

For optimal result, place this code at the very end of your page. Check HighlightAll for more details about the function.