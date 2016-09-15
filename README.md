ghql
====

`ghql` - github GraphQL API client

[Github GraphQL API](https://developer.github.com/early-access/graphql/)

## Authentication

See <https://developer.github.com/early-access/graphql/guides/accessing-graphql/> for getting an OAuth token. 

Store the token in a env var called `GITHUB_GRAPHQL_TOKEN` 
before trying this pkg.

## Install

Development version


```r
devtools::install_github("ropensci/ghql")
```


```r
library("ghql")
library("jsonlite")
```

## query


```r
ql('{"query": "query { viewer { login }}"}')
```

```
## $data
## $data$viewer
## $data$viewer$login
## [1] "sckott"
```

## Meta

* Please note that this project is released with a [Contributor Code of Conduct](CONDUCT.md). By participating in this project you agree to abide by its terms.