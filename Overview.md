# Introduction #

The idea behind SyntaxHighlighter is to allow insertion of colored code snippets on a web page without relying on any server side scripts.

# Who it's for #

Intended primarily at for bloggers. However, I have seen some source web sites using it as their main display of source code.

# Who it's NOT for #

SyntaxHighlighter isn't for those looking for ability to edit highlighted code.

**SyntaxHighlighter doesn't allow you to edit the source, it can't be made to do so and it will never do that.**

# Performance #

SyntaxHighlighter uses regular expressions to parse the text. It's not extremely fast, in fact, it's pretty slow. If you are trying to highlight a few dozens lines of code, you won't see any problems. Trying to highlight 10kb worth of text will result in JavaScript being aborted because of long execution time.