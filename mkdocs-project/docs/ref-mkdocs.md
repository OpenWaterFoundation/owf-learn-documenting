# Learn Documenting / Reference - MkDocs #

[Markdown](markdown) files are a good option for documenting the content of folders
or providing simple landing pages in GitHub repositories.
However, it is often necessary to create substantial documents, such as full user or developer manuals for software.
In this case, the MkDocs software is a good option.
[Jeckyll](ref-jeckyll) is also an option.

* [MkDocs Overview](#mkdocs-overview)
* [Benefits of MkDocs](#benefits-of-mkdocs)
* [Limitations of MkDocs](#limitations-of-mkdocs)
* [When to Use MkDocs](#when-to-use-mkdocs)
* [When Not to Use MkDocs](#when-not-to-use-mkdocs)
* [MkDocs Tools](#mkdocs-tools)

-----

## MkDocs Overview ##

See:

* [MkDocs](http://www.mkdocs.org/)
* [OWF / Learn MkDocs](http://learn.openwaterfoundation.org/owf-learn-mkdocs/)

## Benefits of MkDocs ##

1. Simple outline for organizing pages.
2. Source files are Markdown files that can be edited with a text editor.
3. Markdown files are converted to HTML and therefore can replace more complex HTML in many applications.
4. Local static website can be viewed in a browser before publishing.
5. Versions of Markdown files can be easily tracked in a version control system such as Git.
Differences between versions can be easily pinpointed,
compared to binary files such as Word and PDF that are essentially "blobs" of encoded text.
6. If necessary, HTML elements can be included for more advanced formatting.
7. Multiple themes are available to control features such as navigation, search, and styling content.
8. Custom CSS can be used.

## Limitations of MkDocs ##

1. Because Markdown is used for formatting, content formatting is generally limited to Markdown capabilities
(although HTML elements can be inserted into HTML if necessary).  See [Limitations of Markdown](ref-markdown#limitations-of-markdown).

## When to Use MkDocs ##

The following are recommendations for when to use MkDocs:

1. Use when simple Markdown files such as `README.md` are not enough.
2. Use to create navigable, interactive static websites such as software manuals,
in particular when files can be moved to a version control system such as Git/GitHub.

## When Not to Use MkDocs ##

1. When a traditional memo/report document is needed - Word/PDF are probably better in this case.

## MkDocs Tools ##

* Markdown editors:
	+ [Atom](https://atom.io/)
	+ [MarkdownPad](http://markdownpad.com/)
