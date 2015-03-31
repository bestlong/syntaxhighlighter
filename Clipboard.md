# Copy to clipboard #

Version 1.5 makes "copy to clipboard" functionality available to all browsers supporting Flash. It uses a 1x1 Flash movie to copy the code to user's clipboard.

To enable this functionality, you must set `ClipboardSwf` variable to location of `clipboard.swf` file. This must be done before calling HighlightAll.

```
<script class="javascript">
dp.SyntaxHighlighter.ClipboardSwf = '/flash/clipboard.swf';
dp.SyntaxHighlighter.HighlightAll('code');
</script>
```