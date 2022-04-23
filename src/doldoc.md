# DolDoc Filetype
Terry Davis saw it fit to create a new filetype for TempleOS, the DolDoc. The DolDoc is a filetype, but that does not do it justice. The DolDoc is closer to a Microsoft Word file than a txt file, but more streamlined and with many of the technical aspects exposed to the user. 

Let me point something fascinating out: if you didn't know, when you boot up TempleOS, the terminal that starts with the computer is actually a DolDoc. Pressing CTRL+t will allow you to see the plaintext version of the DolDoc, exposing the special formatting required to make the terminal work.

In the terminal, you'll find tons of examples of what DolDocs are capable of. Not only can they just be simple text files or source code files, they can have links to documents, buttons to run commands, and so much more. Here are some of the things you can do with DolDocs:

- Make a user interface for a game complete with buttons, setting inputs, and graphics
- Programmatically or manually create tree/directory structures, each level of which you can collapse/uncollapse
- Store the source code and graphics for an application in the same file
- And, apparently, even make a terminal

For good reason, DolDocs are ubiquitous in TempleOS. So let's get to know them!

# Editing Files
When you click on a DolDoc or select one with <kbd>Space</kbd>, the document will open. From there, the editor controls like a normal visual text editor. It's very intuitive. A couple useful keybinds to know:

<kbd>Escape</kbd>: press to save and exit.   

<kbd>Shift+Escape</kbd>: press to abort and exit.   

<kbd>Ctrl+Left/Right</kbd>: Jump to the beginning or end of the current line.

<kbd>Ctrl+f</kbd>: Find. Type something in and then press escape to execute. You can also find/replace.

<kbd>Ctrl+t</kbd>: View plaintext of the DolDoc. Very useful for formatting.

<kbd>Ctrl+l</kbd>: Insert a command/widget into the document. Experiment with this one!

# Plaintext
DolDocs are mostly plaintext, usually. However, there are special commands wrapped in dollar signs ($) that add widgets or formatting to the text. Here are some useful examples:

Centered text: `$TX+CX,"Centered Text!"$`

Light blue centered text: `$LTBLUE$$TX+CX,"Centered Text!"$$FG$`

> The first command, `$LTBLUE$`, sets the text color to light blue. The last command, `$FG$`, returns the text color to the default foreground color.

Change the default foreground color to purple: `$FD, PURPLE$`
Scroll through text: `$TX, "Weeeeee!", SCX=5$`

As you can see, there are countless things you can do with DolDocs. And this is just text formatting! Check out the original documentation for the [full breakdown](https://web.archive.org/web/20170305001433/http://www.templeos.org/Wb/Doc/DolDocOverview.html#l1).
