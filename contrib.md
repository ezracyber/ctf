# Gitbook Usage

The CTF Field Guide is built with [Gitbook](https://github.com/GitbookIO/gitbook), a command line tool for building books with Git and Markdown. You can use Gitbook to output the CTF Field Guide as a PDF, an eBook or a single, printable HTML page. Make sure you have [NodeJS](http://nodejs.org/) and `npm` on your operating system, then install Gitbook and a few of its plugins:

```
npm install gitbook gitbook-plugin-ga gitbook-pdf ebook-convert -g
```

With Gitbook installed, you can run any of these commands from within the book directory:

* Generate an interactive, static website: `gitbook build ./myrepo`
* Generate a single page website: `gitbook build ./myrepo -f page`.
* Generate a PDF: `gitbook pdf ./myrepo`. Requires [gitbook-pdf](https://github.com/GitbookIO/gitbook-pdf).
* Generate an eBook: `gitbook ebook ./myrepo`. Requires [ebook-convert](http://manual.calibre-ebook.com/cli/ebook-convert.html).



