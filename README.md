
<!-- README.md is generated from README.Rmd. Please edit that file -->
[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)

seafile
=======

The goal of seafile is to connect to seafile API using R. This Is a partial implementation, PR welcome ;)

Installation
------------

``` r
remotes::install_github("VincentGuyader/seafile")
```

Example
-------

```
# remotes::install_github("VincentGuyader/seafile")
library(seafile)
# ask_seafile_api_token(username = 'your_email',
#                       password = 'your_password',
#                       seafile_url = 'https://box.xjtlu.edu.cn')
set_seafile_api_token(token)
# delete_seafile_api_token()
mylib <- list_libraries()

get_repo_id('pz')
get_seafile_url()
get_upload_link(repos_id = get_repo_id('pz'))
get_dir(repos_id = get_repo_id('pz'))
get_dir(dir = 'Data', repos_id = get_repo_id('pz'))
```

