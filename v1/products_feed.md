# Products Feed

## GET /v1/products/feed

Query params

* `token` - Your API token
* `page` - 0-indexed page
* `page-size` - number of results, must be [1..200]

e.g.

``` sh
curl https://level.ecomedes.com/v1/products/feed?token=<TOKEN>&page=0&page-size=5
```
