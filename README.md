# md2HH - markdown to Haaga-Helia

If you are writing your work in markdown and need to get the document into the official Haaga-Helia format this is for you.

## Installing

1. Install [pandoc](http://pandoc.org/)

  Mac OS X:

  ~~~~
  brew install pandoc
  ~~~~

  Others: [here](http://pandoc.org/installing.html)

2. Download this repository (or just [TemplateThesis.docx](TemplateThesis.docx)) and place it the same folder with your markdown file.

## Converting your work

Use the following command to convert your file. This will create a docx document with the Haaga-Helia template including table of contents and your content. At the moment you have to manually add the **first page** and the **abstract page** to the document (you find them from the [TemplateThesis.docx](TemplateThesis.docx)).

~~~~
pandoc thesis_example.md -f markdown -t docx --reference-docx=TemplateThesis.docx --toc -o ThesisExample.docx
~~~~

First time you open the document word should ask you:

> This document contains fields that may refer to other files. Do you want to update the fields in this document?

Answer **Yes** to this. It will create the table of contents.

## How to use markdown

See basic markdown functionality from the [thesis_example.md](thesis_example.md)

[Markdown](https://daringfireball.net/projects/markdown/)