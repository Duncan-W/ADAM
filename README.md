ADAM: Application of Data
Mining Techniques
to Service Modelling and Evaluation at
Medical Companies
========================


## Author(s)
*   Duncan Wallace

## Abstract
 In an era of “big data”, computational solutions through large-scale machine learning (ML) have provided recourse to problems which previously would have proven very difficult to address. In recent years, ML approaches have been successfully applied to analysis of patient symptom data in the context of disease diagnosis, at least where such data is well codified. However, much of the data present in Electronic Health Records (EHR) are unlikely to prove suitable for classic ML approaches. Furthermore, as scores of data are widely spread across both hospitals and individuals, a decentralised, computationally scalable methodology is a priority.

The focus of this thesis is to develop a method to deliver a framework for decision support in an out-of-hours healthcare provision centre (OOHC). This framework is designed to clean case data, improve the quality of textual features, provide prediction in relation to frequent users of OOHC, and comply with the standard in relation to EHR. These standards relate to data representation, data analysis, and quality of service derived from the data.

Our research is based upon the early identification of a small subsection of patients who are frequent users. These are patients who have underlying conditions which will cause them to repeatedly require medical attention. OOHC act as an ad-hoc delivery of telemedicine and treatment, where interactions occur without recourse to a full medical history of the patient in question. Medical histories, relating to patients contacting an OOHC, may reside in several distinct EHR systems in multiple hospitals or surgeries, which are unavailable to the OOHC in question. As such, although a local solution is a better option for this problem, it follows that the data under investigation is incomplete, heterogeneous, and comprised mostly of noisy textual notes compiled during routine OOHC activities. 

Through a range of machine learning methodologies, the aim of this thesis is to provide the means to identify patient cases, upon initial contact, which are likely to relate to such outliers. In particular, deep learning approaches were adopted in the development of a system of classification of these cases. A further aim of this thesis is to elucidate the discovery of frequent user cases by examining the exact terms which provide strong indication of positive and negative case entries. 




--------------------------------------------------------------------------------

## Building this thesis - XeLaTeX

### Using latexmk (Unix/Linux/Windows)

This template supports `XeLaTeX` compilation chain. To generate  PDF run

    latexmk -xelatex thesis.tex
    makeindex thesis.nlo -s nomencl.ist -o thesis.nls
    latexmk -xelatex -g thesis.tex

## Building your thesis - LuaLaTeX

### Using latexmk (Unix/Linux/Windows)

This template supports `LuaLaTeX` compilation chain. To generate  PDF run

    latexmk -pdflatex=lualatex -pdf thesis.tex


## Building your thesis - LaTeX / PDFLaTeX

### Using latexmk (Unix/Linux/Windows)

This template supports `latexmk`. To generate DVI, PS and PDF run

    latexmk -dvi -ps -pdf thesis.tex



### Using the make file (Unix/Linux)

The template supports PDF, DVI and PS formats. All three formats can be generated
with the provided `Makefile`.

To build the `PDF` version of your thesis, run:

    make


This build procedure uses `pdflatex` with `bibtex` and will produce `thesis.pdf`.
To use `pdflatex` with `biblatex`, you should run:

    make BIB_STRATEGY=biblatex

To use `XeLaTeX`, you should run:

    make BUILD_STRATEGY=xelatex

or with `biblatex`

    make BUILD_STRATEGY=xelatex BIB_STRATEGY=biblatex

To use `LuaLaTeX`, you should run:

    make BUILD_STRATEGY=lualatex

or with `biblatex`

    make BUILD_STRATEGY=lualatex BIB_STRATEGY=biblatex


To produce `DVI` and `PS` versions of your document, you should run:


    make BUILD_STRATEGY=latex

This will use the `latex` command to build the document and will produce
`thesis.dvi`, `thesis.ps` and `thesis.pdf` documents. You will need psutils installed

Clean unwanted files

To clean unwanted clutter (all LaTeX auto-generated files), run:

    make clean

__Note__: the `Makefile` itself is take from and maintained at
[here](http://code.google.com/p/latex-makefile/).

### Shell script for PDFLaTeX (Unix/Linux)

Usage: `sh ./compile-thesis.sh [OPTIONS] [filename]`

[option]  compile: Compiles the PhD Thesis

[option]  clean: removes temporary files - no filename required

### Using the batch file on Windows OS (PDFLaTeX)

*    Open command prompt and navigate to the directory with the tex file. Run:

    `compile-thesis-windows.bat`.

*    Alternatively, double click on `compile-thesis-windows.bat`



--------------------------------------------------------------------------------



## Acknowlegments

*  Krishna Kumar (kks32) - updated latex template

*  H. Banderi -  CUED Version 1.1 Template

*   Alex Ridge - original idea, code concepts & testing

*   Steven Kaneti - code concepts

*   Tina Schwamb - testing and bug reports

*   John Plaice - Bug fixes
