
<!-- README.md is generated from README.Rmd. Please edit that file -->

# valentine <a href="https://valentine.tada.science"><img src="man/figures/logo.png" align="right" height="138" /></a>

<!-- badges: start -->

[![CRAN
status](https://www.r-pkg.org/badges/version/valentine)](https://CRAN.R-project.org/package=valentine)
[![R-CMD-check](https://github.com/tadascience/valentine/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/tadascience/valentine/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of valentine is to spread the love 💛 about your favourite R
package via “roses are red …” poems 🌹 generated by AI via the
[ellmer](https://ellmer.tidyverse.org/) 📦.

## Installation

You can install the development version:

``` r
pak::pak("tadascience/valentine")
```

## Setup

`valentine::roses()` uses a
[Chat](https://ellmer.tidyverse.org/reference/Chat.html) object to
communicate with the LLM of your choice. The default value for the
`chat` argument uses the “gpt-3.5-turbo” model from OpenAI via the
[ellmer::chat_openai()](https://ellmer.tidyverse.org/reference/chat_openai.html)
which is usually good enough for such a simple task.

Please refer to [ellmer](https://ellmer.tidyverse.org/index.html)
documentation for information on setting up api keys, etc …

## Example

``` r
valentine::roses("dplyr")
#> Roses are red,  
#> dplyr is my bae 🌹  
#> With pipes and verbs,  
#> My data never goes astray 💖
```

``` r
valentine::roses("lubridate", hint = "make it kinky")
#> Roses are red, violets are blue, 
#> But lubridate, oh how I adore you 💕
#> You make my dates smooth and my times hot 🔥
#> In R programming, you're all I've got 😈🌹
```

``` r
valentine::roses("valentine")
#> Roses are red, 
#> Valentine is too 🌹
#> With its data magic, 
#> My love for it grew 💖
```
