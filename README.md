# ITDRC Pocket Guide

This project uses [GitBook](https://toolchain.gitbook.com)!


## Setting up your workstation to author and update this project
Before we can begin, you will need a [GitHub](https://github.com) account; this will allow you to submit changes back to this project. Additionally, you will need a text editor ([vim](https://vim.sourceforge.io/download.php), [emacs](https://www.gnu.org/software/emacs/), [joe](http://joe-editor.sourceforge.net), [Atom](https://atom.io), [TextMate](https://macromates.com), you get the idea), since this project uses [Markdown](https://guides.github.com/features/mastering-markdown/).

1. Install [nodejs](https://nodejs.org/en/)
2. Now we need to install the gitbook application using npm (part of nodejs), on the command line run the following: ```npm install gitbook-cli -g```


## Using gitbook!
Once you have cloned this project from GitHub, you can run the following command inside the project folder to generate a live HTML preview.

```
OggBook:ITDRC-pocket-guide ogg$ gitbook serve
Live reload server started on port: 35729
Press CTRL+C to quit ...

info: 7 plugins are installed
info: loading plugin "livereload"... OK
info: loading plugin "highlight"... OK
info: loading plugin "search"... OK
info: loading plugin "lunr"... OK
info: loading plugin "sharing"... OK
info: loading plugin "fontsettings"... OK
info: loading plugin "theme-default"... OK
info: found 1 pages
info: found 1 asset files
info: >> generation finished with success in 0.7s !

Starting server ...
Serving book on http://localhost:4000
```
Gitbook will start a local webserver at ```http://localhost:4000```, by default. While you are editing the markdown pages, the GitBook automatically will regenerate the HTML site.

## Generation of PDF, HTML and EPUB files.
Note: To generate epub and pdf outputs you will need to have [Calibre](https://calibre-ebook.com/download) installed. **[GitBook Documentation](https://toolchain.gitbook.com/ebook.html)**
```
# Generate a PDF file
$ gitbook pdf ./ ./output/ITDRC-pocket-guide.pdf

# Generate an ePub file
$ gitbook epub ./ ./output/ITDRC-pocket-guide.epub

# Generate an HTML (output in _book)
$ gitbook build
```

## Helpful Guides
* [GitHub Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [Git Cheat Sheet](https://www.git-tower.com/blog/git-cheat-sheet/)
