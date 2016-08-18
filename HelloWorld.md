## This is a markdown file

I added some information about adding comments to markdown files.
Examples of hidden comments are included in this .md
[comments-in-markdown @stackoverflow](http://stackoverflow.com/questions/4823468/comments-in-markdown "Magnus@stackoverflow")

If you want a comment that is strictly for yourself (readers of the converted document should not be able to see it, even with "view source") you could (ab)use the link labels (for use with reference style links) that are available in the core Markdown specification:
[markdown syntax](http://daringfireball.net/projects/markdown/syntax "daringfireball.net")

<This is a comment, it will not be included>
<in  the output file unless you use it in>
<a reference style link.>

[comment]: < a reference style link.>


// <This is also a comment>
To improve platform compatibility (and to save one keystroke) it is also possible to use # (which is a legitimate hyperlink target) instead of <>:

[//]: # (This may be the most platform independent comment)
It may also be prudent to insert a blank line before and after this type of comments, because some Markdown parsers may not like link definitions brushing up against regular text.

This should work with most Markdown parsers, since it's part of the core specification. (even if the behavior when multiple links are defined, or when a link is defined but never used, is not strictly specified).
