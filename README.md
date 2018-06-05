# thesisdownmq

This project was inspired by the bookdown and thesisdown packages for Macquarie University

Currently, the PDF and gitbook versions are fully-functional. (The word and epub versions are developmental, have no templates behind them, and are essentially calls to the appropriate functions in bookdown. There is no plan to further develop these, in fact, files related to these will be removed in the near future.)

The current outputs for the two functional versions are here:

PDF (Generating LaTeX file is available here with other files at in the book directory.)
gitbook

Under the hood, the Reed College LaTeX template was updated to ensure that documents conform precisely to submission standards at Macquarie University. At the same time, composition and formatting can be done using lightweight markdown syntax, and R code and its output can be seamlessly included using rmarkdown.

Using thesisdowndss has some prerequisites which are described below. To compile PDF documents using R, you are going to need to have LaTeX installed. It can be downloaded for Windows at http://http://miktex.org/download and for Mac at http://tug.org/mactex/mactex-download.html. Follow the instructions to install the necessary packages after downloading the (somewhat large) installer files. You may need to install a few extra LaTeX packages on your first attempt to knit as well.

Using thesisdowndmq from Thomas Fung's GitHub

To use thesisdowndmq from within RStudio:

Install the latest RStudio.

Install the bookdown and thesisdown packages:

install.packages("devtools")
install.packages("bookdown")
devtools::install_github("thomas-htf/thesisdowndmq")
Use the New R Markdown dialog to select Thesis:
New R Markdown

Note that this will currently only Knit if you name the directory index as shown above.
