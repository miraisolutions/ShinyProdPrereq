# Bring a (Shiny) Application to Production Workshop Prerequisites

Package prerequisites for "Bring a (Shiny) Application to Production" can be fulfilled using this repo as follows:

- Create a new RStudio project from this repo
  ```
  File > New Project... > Existing Directory
  ```
- Once in the new project, run at the R console
  ``` r
  install.packages(c("remotes", "renv"))
  remotes::install_deps()
  ```
  and then
  ```
  renv::activate()
  renv::restore(prompt = FALSE) # you can ignore warnings about a different R version
  ```
