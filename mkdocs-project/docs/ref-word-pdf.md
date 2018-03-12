# Learn Documenting / Reference - Word & PDF #

Microsoft Word and optionally PDF saved from Word are popular formats for documentation.
PDF is being associated with Word because Word is one of the most common tools used to create
PDF documents.
Software to edit Word files includes commercial Microsoft Word software,
free and open source Libre Office, and other software.

* [Word and PDF Overview](#word-and-pdf-overview)
* [Benefits of Word and PDF](#benefits-of-word-and-pdf)
* [Limitations of Word and PDF](#limitations-of-word-and-pdf)
* [When to Use Word and PDF](#when-to-use-word-and-pdf)
* [When Not to Use Word and PDF](#when-not-to-use-word-and-pdf)
* [Word and PDF Tools](#word-and-pdf-tools)

--------------

## Word and PDF Overview ##

Microsoft created the Word document format for Microsoft Word software documents.
The `*.docx` file format is proprietary, although people have been reverse engineering it to
add support in software tools.

PDF files are text files with encoded documentation.
See the [PDF specification on Wikipedia](https://en.wikipedia.org/wiki/Portable_Document_Format).

## Benefits of Word and PDF ##

1. Software is readily available to businesses.
2. Most professionals are comfortable using Word and saving as PDF.
3. High quality visual products.

## Limitations of Word and PDF ##

1. Using the full Word features requires paying for Microsoft Office.
2. Documentation requires special software to edit the files (text editor cannot be used).
3. Word files are essentially binary files.  PDF files are large text blobs.
Using version-tracking software
such as Git have limitations:
	1. viewing differences takes extra effort such as exporting to text first
	2. Large word and PDF files saved in a repository take up a lot of space.
	3. It can be difficult to automate conversion of Word files to PDF.
	Consequently more than just source files are saved in the repository.
4. Large Word and PDF files can be difficult to interact with, despite search and bookmark features.
5. Word files in particular are not universally accessible, for example on Linux.

## When to use Word and PDF ##

The following are recommendations for when to use Word and PDF:

1. When the readers/editors/maintainers of the documentation are comfortable with
Word and PDF technologies but are not comfortable with other documentation technologies.
2. When the documents need to be managed in a system like a document management system.
3. When a "living" navigable document is not important.
4. When other tools cannot provide necessary features, such as advanced formatting.
5. When it is required, such as for project deliverables.

## When Not to use Word and PDF ##

1. When the documentation ecosystem prefers something else, such as [Markdown](#ref-markdown).
2. When navigable website is the result.  It is possible with Word but can be difficult.
3. When simple files are needed, such as text-editable files in a repository.

## Word and PDF Tools ##

The following are useful tools for creating Word and PDF documentation:

* Microsoft Word (use save as PDF feature to save PDF)
