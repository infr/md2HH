# md2HH - markdown to Haaga-Helia

If you are writing your work in markdown and need to get the document into the official Haaga-Helia format this is for you.

1. Install [pandoc](http://pandoc.org/)

  For Mac OS X:

  ~~~~
  brew install pandoc
  ~~~~

  Others: [here](http://pandoc.org/installing.html)

2. Download this repository

3. Use the following command to convert the file. Currently you have to **manually** include three first pages.

~~~~
pandoc thesis.md -f markdown -t docx --reference-docx=pohja.docx --toc -o thesis.docx
~~~~

See basic markdown functionality from the <thesis_example.md>