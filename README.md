# md2HH - markdown to Haaga-Helia

If you are writing your work in markdown and need to get the document into the official Haaga-Helia format this is for you.

1. Install [pandoc](http://pandoc.org/)

  Mac OS X:

  ~~~~
  brew install pandoc
  ~~~~

  Others: [here](http://pandoc.org/installing.html)

2. Download this repository (or [pohja.docx](pohja.docx))

3. Use the following command to convert your file. This will create a docx document with the Haaga-Helia template including table of contents and your content. At the moment you have to **manually** add two first pages.

~~~~
pandoc thesis_example.md -f markdown -t docx --reference-docx=TemplateThesis.docx --toc -o thesis.docx
~~~~

See basic markdown functionality from the [thesis_example.md](thesis_example.md)