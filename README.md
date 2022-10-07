# About

This package is meant to serve as a example for how to include Quarto templates with extensions in a fashion that reproduces the functionality of R Markdown templates included with R packages.

Specifically, the following functionality:

* All template resources are included with the extension
* Create a new Quarto document based on a template in a single function
    - A template skeleton is used as a template when creating a new Quarto document
    - Resources such as latex templates/headers are copied over
    - A sub-directory is created for the new report
