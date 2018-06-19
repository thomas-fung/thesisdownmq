# thesisdownmq

This project was inspired by the bookdown and thesisdown packages.

Currently, the PDF version is fully-functional. (The word, gitbook and epub versions are developmental, have no templates behind them, and are essentially calls to the appropriate functions in bookdown.)

Under the hood, the Reed College LaTeX template was updated to ensure that documents conform precisely to submission standards at Macquarie University. At the same time, composition and formatting can be done using lightweight markdown syntax, and R code and its output can be seamlessly included using rmarkdown.

Using **thesisdownmq** has some prerequisites which are described below. To compile PDF documents using **R**, you are going to need to have LaTeX installed. It can be downloaded for Windows at http://http://miktex.org/download and for Mac at http://tug.org/mactex/mactex-download.html. Follow the instructions to install the necessary packages after downloading the (somewhat large) installer files. You may need to install a few extra LaTeX packages on your first attempt to knit as well.

### Using thesisdowndmq from Thomas Fung's GitHub

To use **thesisdowndmq** from within RStudio:

1) Install the latest RStudio and rmarkdown.

2) Install the **bookdown** and **thesisdownmq** packages:

```S
install.packages("devtools")
install.packages("bookdown")
devtools::install_github("thomas-fung/thesisdownmq")
```

3) Use the New R Markdown dialog to select MQ Thesis:

![New R Markdown](thesis_rmd.png)

Note that this will currently only Knit if you name the directory index as shown above.

4) Knit the index.Rmd file to get the book in PDF format.

5) Edit the individual chapter R Markdown files as you wish and then re-run step (4) again.
