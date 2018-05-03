# Product Detail

## GET /v1/products/BRAND_IDENTIFIER/SKU

Query params

* `token` - Your API token

Route params

* `BRAND_IDENTIFIER` - Brand's unique identifier; can be found in products feed API
* `SKU` - Product identifier, also available in products feed API

e.g.

``` sh
curl https://fulcrum.ecomedes.com/v1/products/hennessy-hinchcliffe/N771614R-DF-HH?token=<TOKEN>
```
