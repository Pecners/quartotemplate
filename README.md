# About

This package is meant to serve as a example for how to include Quarto templates with extensions in a fashion that reproduces the functionality of R Markdown templates included with R packages.

Specifically, the following functionality:

* All template resources are included with the extension
* Create a new Quarto document based on a template in a single function
    - A template skeleton is used as a template when creating a new Quarto document
    - Resources such as latex templates/headers are copied over
    - A sub-directory is created for the new report

# Use

Install this package with the following code:

```
remotes::install_github("Pecners/quartotemplate")
```

The `use_quarto_ext()` function will implement the functionality listed above. For example, executing `use_quarto_ext(file_name = "test")` will create a new director called `test` with a `header.tex` file and `test.qmd` file for the the new report. `test.qmd` is based on `skeleton.qmd` found [here](./inst/extdata/_extensions/quartotemplate/skeleton.qmd): `inst` > `extdata` > `_extensions` > `quartotemplate` > `skeleton.qmd`

# Credits

[Thomas Mock](https://twitter.com/thomas_mock) provided tips on Twitter that gave me the idea for this solution, and the `use_quarto_ext()` is an extension of a function he wrote in this repo: https://github.com/jthomasmock/octavo.
