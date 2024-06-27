# r-forge

# Contributing packages to `r-forge`
Steps to get R packages on r-forge. You need to have [pixi](https://pixi.sh) installed. 
Packages should already be on R-Universe. Packages will be prefixed with `r-`, so an R package named `foo` will be `r-foo` on r-forge.
1. Fork and clone `r-forge`
2. Generate recipe: `pixi run generate https://cran.r-universe.dev/api/packages/foo`
3. Test build locally: `pixi run build r-foo`