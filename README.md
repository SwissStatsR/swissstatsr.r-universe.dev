# Packages for the Swiss Stats R Universe 

This repo hosts the `package.json` configuration file used to build the [Swiss Stats R Universe](//swissstatsr.r-universe.dev/).

## Adding a new package

Make a pull request to append an entry to the `package.json` file, such as:

``` json
    {
        "package": "<my-package-name>",
        "url": "https://github.com/<my-package-github-url>"
    }
```

## Installing a package from the Swiss Stats R Universe

An example using {BFS}:

``` r
install.packages("BFS", repos = "https://swissstatsr.r-universe.dev" )

```
Alternatively you can configure your `repos` R option as such:

``` r
options(
    repos = c(
        rswissgroup = "https://swissstatsr.r-universe.dev",
        CRAN = "https://cloud.r-project.org"
        )
  )
install.packages("BFS")
```
