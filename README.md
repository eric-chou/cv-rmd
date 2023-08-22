# Eric Chou's CV

Use a workflow to programmatically generate CV via [.csv files](data) + Rmarkdown (`vitae` package).

A [Docker image](Dockerfile) is used to deploy a stable environment for dependencies such as `tinytex` and others. Then, a [(gh) .yml file](.github/workflows/docker_action.yml) uses this Docker image with the [RMarkdown](docs/cv.Rmd) file.

## References

* `vitae` package: https://pkg.mitchelloharawild.com/vitae/
  - https://cran.r-project.org/web/packages/vitae/vignettes/vitae.html
* `awesomecv` template: https://pkg.mitchelloharawild.com/vitae/reference/awesomecv.html 
* `awesomecv` example: https://github.com/akirosingh/CV
* `vitae` RMarkdown and data handling example: https://github.com/natbprice/cv
* Docker + Github workflow example: https://github.com/mlampros/My.CVitae
