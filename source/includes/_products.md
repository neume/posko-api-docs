# Products
This resource enables you to retrieve product information

## General Actions
Detailed information about these endpoints are down below
- GET /api/v1/products
- GET /api/v1/products/:id



## Endpoints
### GET /api/v1/products
Retrieves a list of product

| Parameter | Type    | Description                           |
|:----------|:--------|:--------------------------------------|
| ids       | Array   | An array of ids to be retrieved       |
| limit     | Integer | The number of results per page        |
| page      | Integer | The page to be retrieved              |
| since_id  | Integer | Retrieves data after the specified id |

### GET /api/v1/products/:id
Retrieves info of a product

| Paramater | Type    | Description                  |
|:----------|:--------|:-----------------------------|
| :id       | Integer | The unique id of the product |
