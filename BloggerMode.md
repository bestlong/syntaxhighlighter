# Blogger Mode #

Blogger has a nasty habit of replacing all new lines with `<br/>` tags which makes it impossible to post code snippets.

To fix the situation [version 1.5.1](Version_1_5_1.md) introduces "Blogger Mode" which can be enabled before a call to `HighlightAll()` by a call to `BloggerMode()` like in the example below:

```
dp.SyntaxHighlighter.BloggerMode();
dp.SyntaxHighlighter.HighlightAll('code');
```