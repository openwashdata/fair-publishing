# FAIR Data Publishing

The guide to publishing a dataset as an R data package with [washr](https://openwashdata.github.io/washr/), read online at <https://openwashdata.github.io/fair-publishing/>.

The guide is the narrative form of the washr workflow. The condensed reference is the washr vignette [Get started with washr](https://openwashdata.github.io/washr/articles/washr.html), and the AI assisted form is the washr skill in the [openwashdata plugin](https://github.com/openwashdata/pkgreview).

The repository moved from `Global-Health-Engineering/ghedatapublishing` to openwashdata on 2026-10-27, when the guide was reworked for washr 1.2.0 and renamed. The old addresses redirect here.

## Rendering

The book is a [Quarto](https://quarto.org/) project. `quarto render` writes the site into `docs/`, which is committed and served by GitHub Pages from the main branch. The PDF needs a LaTeX installation, for example [TinyTeX](https://yihui.org/tinytex/).

## Checking against washr

`WASHR_VERSION` records the washr release the code in the chapters was last checked against. `Rscript scripts/washr_drift.R` checks every washr call in the chapters against the installed washr, and the washr-drift workflow runs it weekly and on every push.
