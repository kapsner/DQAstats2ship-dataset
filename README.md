# DQAstats2ship-dataset

<!-- badges: start -->
<!-- badges: end -->

The goal of DQAstats2ship-dataset is to provide a step-by-step tutorial on how to prepare a new dataset and corresponding metadata in order to be analyzed with the [`DQAstats`](https://cran.r-project.org/package=DQAstats) R-package.

Therefore, the publicly avaiable SHIP-dataset from the R-package [`dataquieR`](https://cran.r-project.org/package=dataquieR) is used due to its well described metadata. For further information on the dataset as well as the data-quality indicators used in `dataquieR`, please refer to [https://dataquality.ship-med.uni-greifswald.de/](https://dataquality.ship-med.uni-greifswald.de/).

This tutorial is fully reproducible by rendering the HTML-page using the `bookdown` R-package. All necessary steps required to transform `dataquieR`'s metadata-representation of the SHIP-dataset into `DQAstats`' `mdr.csv`-file are presented in the Rmarkdown document [`index.Rmd`](./index.Rmd).

Finally, `DQAstats`' main function `DQAstats::dqa()` is used to perform the data quality assessment for the SHIP-dataset and to create a PDF report with all results.

Alternatively, it is shown how to launch the shiny app [`DQAgui`](https://cran.r-project.org/package=DQAgui) as a graphical user interface frontend to all the functionality implemented in `DQAstats`.

The HTML-page with the tutorial can be generated with the following command:

```r
bookdown::render_book(
  input = ".",
  config_file = "_bookdown.yml"
)
```

## More Infos

* about `DQAstats`: [(https://cran.r-project.org/package=DQAstats](https://cran.r-project.org/package=DQAstats)
* about `DQAgui`: [https://cran.r-project.org/package=DQAstats](https://cran.r-project.org/package=DQAstats)
* the `DQAstats`-Wikipage: [https://github.com/miracum/dqa-dqastats/wiki](https://github.com/miracum/dqa-dqastats/wiki)
* about MIRACUM: [https://www.miracum.org/](https://www.miracum.org/)
* about the Medical Informatics Initiative: [https://www.medizininformatik-initiative.de/index.php/de](https://www.medizininformatik-initiative.de/index.php/de)
* about `dataquieR`: [https://cran.r-project.org/package=dataquieR](https://cran.r-project.org/package=dataquieR)
