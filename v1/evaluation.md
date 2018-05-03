# Rating Systems
## List All

GET https://fulcrum.ecomedes.com/v1/rating-systems?token=TOKEN

## Rating System Details

GET https://fulcrum.ecomedes.com/v1/rating-systems/<ID>?token=TOKEN
GET https://fulcrum.ecomedes.com/v1/rating-systems/nc-2009?token=TOKEN


## Perform an Evaluation

POST https://fulcrum.ecomedes.com/v1/projects/evaluate?token=TOKEN

e.g.

curl -X POST -H "Content-Type: application/json" 'https://fulcrum.ecomedes.com/v1/projects/evaluate?token=TOKEN' --data '{
    "products": {
        "interface/8221007999G17S001": {
            "quantity": {
                "value": 100
            },
            "price": 12.0
        }
    },
    "parameters": {
        "location": {
            "value": "30024"
        }
    },
    "rating_systems": [
        "nc-2009"
    ]
}'

Multiple products

curl -X POST -H "Content-Type: application/json" 'https://fulcrum.ecomedes.com/v1/projects/evaluate?token=TOKEN' --data '{
    "products": {
        "interface/8221007999G17S001": {
            "quantity": {
                "value": 100
            },
            "price": 12.0
        },
        "interface/1015001999R45S001": {
            "quantity": {
                "value": 5
            },
            "price": 90.0
        }
    },
    "parameters": {
        "location": {
            "value": "30024"
        }
    },
    "rating_systems": [
        "nc-2009"
    ]
}'
