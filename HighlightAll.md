# dp.SyntaxHighlighter.HighlightAll() #

This is a global function that find all code blocks on a web page and transforms them into highlighted code blocks.

## Arguments ##

```
function dp.SyntaxHighlighter.HighlightAll(name, [showGutter], [showControls], [collapseAll], [firstLine], [showColumns])
```

| `name` | required | Name of `<pre>` and `<textarea>` elements to use. |
|:-------|:---------|:--------------------------------------------------|
| `showGutter` | optional | Turns gutter on or off on all processed code blocks. |
| `showControls` | optional | Turns controls on or off on all processed `<pre>`. |
| `collapseAll` | optional | Turns collapse on or off on all processed `<pre>`. If `showControls` is false or switched, this value will be ignored. |
| `firstLine` | optional | Allows to specify the first line where line numbering starts. This is usefull if you want to illustrate where the code block is located relative to the file. |
| `showColumns` | optional | Will show row columns in the first line. |

Any values passed in the HighlightAll call will override corresponding [configuration](Configuration.md) option.