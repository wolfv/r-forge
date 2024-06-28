# r-forge

## Missing a package that you would love to install with pixi?
You're in luck! There's only a few steps between you and your package. You can either create an issue requesting a package, or create the recipe yourself - which is fast and easy! The only pre-requisite is that you need to have [pixi](https://pixi.sh) installed. For now, the package should already be on CRAN - but hopefully it won't be long before we support any package available on [r-universe](https://r-universe.dev/search). 
Packages will be prefixed with `r-`, so an R package named `foo` will be `r-foo` on r-forge.

### Steps to create and test a recipe
1. Fork and clone `r-forge`
2. Generate recipe: `pixi run generate foo`
3. Test build locally: `pixi run build r-foo`
4. Make a PR to merge your recipe into r-forge