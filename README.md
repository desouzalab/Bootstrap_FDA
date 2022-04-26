# Bootstrap_FDA

# Undergraduate Thesis
$endif$
[![License](https://img.shields.io/github/license/$username$/$repo.name$.svg)](https://github.com/$username$/$repo.name$/blob/master/LICENSE)
[![Build Status](https://travis-ci.org/jacquesd/master-thesis.svg?branch=master)](https://travis-ci.org/jacquesd/master-thesis)
[![PDF](https://img.shields.io/badge/PDF-latest-blue.svg?style=flat)](https://github.com/$username$/$repo.name$/blob/master-pdf/$generated_file$.pdf)

This repository contains the report for the master thesis:



<p align="center" style="font-size:larger;">
<i>$title$</i>
</p>
$if(subtitle)$
<p align="center" style="font-size:large;">
<i>$subtitle$</i>
</p>
$endif$

written by $author$, under the supervision of $advisor.title$ $advisor.name$ (advisor) $if(coadvisor)$ and  $coadvisor.title$ $coadvisor.name$ (coadvisor)$endif$, submitted to the $faculty$ of the $university$.


## License
This thesis is made available under the $license.name$. A copy of the full license is available in the [LICENSE](/LICENSE) file.

## PDF version
A rendered PDF version of the thesis is automatically generated using [travis-ci](https://travis-ci.org/jacquesd/master-thesis) and pushed back to this repository at [master-pdf:$generated_file$.pdf](https://github.com/$username$/$repo.name$/blob/master-pdf/$generated_file$.pdf).

Generating the pdf locally requires pandoc (>=2.1.3), XeLaTeX, and Bibtex. Then, run:

``` bash
make
```

This will generate the report in pdf under the name ``$generated_file$.pdf` in the root folder.

To change the name or the generated pdf file, simply overwrite the `OUTPUT` variable (without the extension):

``` bash
make OUTPUT_FILE="new_file"
```
