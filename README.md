# markdown_tutorial
This is a tutorial on how to use markdown. Markdown is a plaintext language, meaning it uses symbols and letters rather than syntax. It has the ability to control the layout of text and files. In this tutorial we will walk through the basics of using markdown. You will first need to start by opening your preferred editor and creating a file with an .md (markdown) extension. From there you can start typing your plain text that you will later learn to format using markdown's language.
***

# Headers
You can indicate a Header by using one or multiple \# before your text you want to format as a header
***

# _Italic Letters_
You can represent _italic_ letters by placing either an \*astrisk\* or an \_underscore\_ around the text you would like to add emphasis to.
***

# __Bold Letters__
You can represent __bold__ letters by placing two \*\*astrisks\*\* or two \_\_underscores\_\_ surrounding the text you would like to make bold.
***

# ~~Strike Through~~
You can strike through a text by placing two \~\~squiqles\~\~ before and after the text you want to strike through
***

# Lists
Lists are very simple to use in MarkDown. To indicate the use of a list all you need to do is place a number before the list item. For example
\1. First ordered list item
\2. Another item
\⋅⋅* Unordered sub-list.
\1. Actual numbers don't matter, just that it's a number
\⋅⋅1. Ordered sub-list
\4. And another item.

As you can see, it does not matter which number is used. MarkDown knows to interpret numbers as lists.
***

# Links
There are multiple options to implementing links using MarkDown. The first option is an inline style link:

#### Inline Style Link
\[inline-style link\]\(\https://www.google.com\)

This will create a text that reads [inline-style link](https://www.google.com) and when clicked will link to the google url.

#### File Reference Link
\[Reference File Link\]\(../blob/master/LICENSE\)

This will create a text that reads [Reference File Link](../blob/master/LICENSE) and when clicked will link to the file directory listed in the parens
***

# Images
There are two ways to implement images in your markdown file. There is inline images and file reference images.

#### Inline Style
\!\[alt text\]\(https://upload.wikimedia.org/wikipedia/commons/6/6f/HP_logo_630x630.png "Logo Title"\)

This will link an image from the listed url like so:

![alt text](https://upload.wikimedia.org/wikipedia/commons/6/6f/HP_logo_630x630.png "Logo Title")


#### File Reference
\!\[alt text\]\[logo\]

\[logo\]: https://github.com/comptonk15/markdown_tutorial/blob/master/Media/HP_logo.png "Logo Title 2"

This will provide an image via a file reference rather than a url

![alt text][logo]

[logo]: https://github.com/comptonk15/markdown_tutorial/blob/master/Media/HP_logo.png "Logo Title Text 2"
***

# Inline Code Blocks
If you need to represent a code block without worrying about the syntax being interpreted as a markdown shorthand you can use \`backticks code block\` which will make looks like the following:

`backticks code block`

### Indicating Language
You can indicate a specific language syntax by using three consecutive \`\`\`backticks\`\`\`

If you were trying to indicate that the code block was using Ruby you would put: ..

\`\`\`Ruby
var s = 100
let(:symbol) { double 'Symbol'}
\`\`\`

Which would out put a code block that knew which language syntax to use. It should appear like this:
```Ruby
var s = 100
let(:symbol) { double 'Symbol'}
```

This is helpful in creating specific documentation relating to individual languages.
***

# Tables
Tables are a little bit more tricky to handle. However, MarkDown is able to represent tables in a very humanistic visual approach. The following code is an example from MarkDown's cheatsheet to give you an idea of how tables are implemnted

```java
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```

That code would output the following table:

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
***

# Block Quotes
Block Quotes can be indicated by using a \> before the quote wanted to be blocked out. If I were to say I wanted to block out "this text" I would enter the markdown as:

\>this text

and the markdown will be interpreted as:

>this text

Keith has things left to do for this final project.