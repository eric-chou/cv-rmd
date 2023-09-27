# Eric Chou's CV

Use a workflow to programmatically generate CV via [.csv files](data) + Rmarkdown (`vitae` package).

Within the [docs](docs) folder, there are `.Rmd` files for both the [full CV](docs/cv.pdf) and a 1-page [resume template](docs/resume_template.pdf). This template can be modified for tailored resumes via the [specific](docs/specific) subdirectory. Likewise, the [data](data) folder has a [specific](data/specific) subdirectory for tailored entries.

A Docker image pulled from [here](https://hub.docker.com/r/mlampros/mycvitae) is used to deploy a stable environment for dependencies such as `tinytex` and others. Then, a [(gh) .yml file](.github/workflows/docker_action.yml) uses this Docker image with the RMarkdown files to update the CV and resume template.	

## References

* `vitae` package: https://pkg.mitchelloharawild.com/vitae/
  - https://cran.r-project.org/web/packages/vitae/vignettes/vitae.html
* `awesomecv` template: https://pkg.mitchelloharawild.com/vitae/reference/awesomecv.html
* `awesomecv` example: https://github.com/akirosingh/CV
* `vitae` RMarkdown and data handling example: https://github.com/natbprice/cv
* Docker + Github workflow example: https://github.com/mlampros/My.CVitae
