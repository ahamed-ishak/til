# Escaping Hash Characters in Markdown

In the process of creating the root TIL `readme.md`, I wanted to make a header for C# items but was having trouble getting it to appear properly.  In Markdown, you can escape various characters using a backslash (`\`), so if you wanted to type C\#, you would use `C\#`.

Unfortunately, when creating a heading the trailing hash character gets treated as an optional header close tag. 

So `### C\#` turns into: 

### C\#

The easiest way to get around this is by adding a trailing space to the header.

`### C\# `

### C\# 

As another note, when you create a header, an anchor is automatically created that you can link to, but any special characters are ignored and it's also all lowercased.  So to link to the C\# header above, you would use `[C#](#c)` which results in [C#](#c).