## This is a markdown file

### Commenting in markdown files
Just creating .md file with only a heading seemed boring to me, so i thought about some usefull example content.
and added some information about adding comments to markdown files.

Examples of hidden comments are included in this .md, you may have to open them in an editor to see the comments.
[comments-in-markdown @stackoverflow](http://stackoverflow.com/questions/4823468/comments-in-markdown "Magnus@stackoverflow")

1. Using link labels
(edit to view comment)

>If you want a comment that is strictly for yourself 
>(readers of the converted document should not be able to see it, even with "view source") 
>you could (ab)use the link labels (for use with reference style links) that are available in the core Markdown specification:
[markdown syntax](http://daringfireball.net/projects/markdown/syntax "daringfireball.net")


<This is a comment, it will not be included>
<in  the output file unless you use it in>
<a reference style link.>

[comment]: < a reference style link.> (this is intentionally made visible by adding a reference []:)

<This is also a comment>

2. Using hyperlink target
To improve platform compatibility (and to save one keystroke) it is also possible to use # (which is a legitimate hyperlink target) instead of <>: 
[comment]: [//]: # (Comment here)
(edit to view comment)

[//]: # (This may be the most platform independent comment)
# (This may be a comment)
>It may also be prudent to insert a blank line before and after this type of comments, because some Markdown parsers may not like link >definitions brushing up against regular text. [//]: # (Comment here)

>This should work with most Markdown parsers, since it's part of the core specification. (even if the behavior when multiple links are >defined, or when a link is defined but never used, is not strictly specified).
