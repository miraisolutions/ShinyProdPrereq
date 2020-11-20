# Bring your Shiny App to Production Workshop Prerequisites

Package prerequisites for [Mirai's workshop "Bring your Shiny App to Production"](https://github.com/miraisolutions/ShinyProdWorkshop/#readme) can be fulfilled using this repo as follows:

- Create a new RStudio project from the repo (https://github.com/miraisolutions/ShinyProdPrereq)
  ```
  File > New Project... > Version Control > Git
  ```
- Once in the new project, run at the R console
  ``` r
  install.packages(c("remotes", "renv"))
  remotes::install_deps()
  renv::activate()
  renv::restore() # you can ignore warnings about a different R version
  ```
