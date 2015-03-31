# Configuration option #

These options allow you to individually configure text blocks.

| `nogutter` | Will display no gutter. |
|:-----------|:------------------------|
| `nocontrols` | Will display no controls at the top. |
| `collapse` | Will collapse the block by default. |
| `firstline[value]` | Will begin line count at `value`. Default value is 1. |
| `showcolumns` | Will show row columns in the first line. |

The options are passed together with the [alias](Languages.md) and are separated by a colon `:` character.

```
<pre name="code" class="html:nocontrols:firstline[10]">
... some code here ...
</pre>
```