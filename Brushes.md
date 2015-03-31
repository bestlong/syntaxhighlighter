# Brushes #

## What are they? ##

_Brushes_, is a term I made up to call highlighters scripts for individual languages. SyntaxHighlighter uses modular approach and consists of core library `shCore.js` and a number of brushes which look like [shBrushXml.js](http://syntaxhighlighter.googlecode.com/svn/trunk/Scripts/shBrushJScript.js), [shBrushCss.js](http://syntaxhighlighter.googlecode.com/svn/trunk/Scripts/shBrushCss.js) and so on.

## How do they work? ##

Each brush describes a set of rules for a particular language. These rules are based on keywords, regular expressions and CSS styles. Most languages follow the same syntax and are parsed in the same way as long as you provider some basic rules for parsing strings, comments and so on.

Alternatively, you can write a completely custom brush and implement your own parsing. An example of such brush is [shBrushXml.js](http://syntaxhighlighter.googlecode.com/svn/trunk/Scripts/shBrushXml.js). It provides formatting for XML/HTML code which doesn't follow same style as say C# or Java does.