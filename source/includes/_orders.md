

# Orders

## Get all orders
```sh
  curl --request GET \
    --url 'http://example.com/api/v1/orders' \
    --header 'Authorization: <Processed Basic hash>' \
    --header 'Content-Type: application/json' \
```

### HTTP Request

```json
{
  "orders": [
    {
      "id": 1,
      "account_id": 1,
      "default_address_id": null,
      "first_name": "Cardo",
      "middle_name": null,
      "last_name": "Dalisay",
      "email": "cardo@dalisay.com",
      "suffix": null,
      "note": null,
      "customer_type": 0,
      "customer_status": 0,
      "status": "active",
    "created_at": "2018-05-23T14:29:38.391Z",
      "updated_at": "2018-05-23T14:29:38.391Z"
    }
  ]
}
```

`GET /api/v1/orders`

### Response

| Key      | Type  | Description          |
|:---------|:------|:---------------------|
| `orders` | Array | Collection of orders |




## Create Order

### HTTP Request

```json
{
  "order": {
    "id": 1,
    "account_id": 1,
    "customer_id": 1,
    "user_id": 1,
    "order_number": 25,
    "note": null,
    "total_line_items_price": "0.0",
    "total_discounts": "0.0",
    "subtotal": "0.0",
    "total_price": "0.0",
    "total_tax": "0.0",
    "total_weight": "0.0",
    "first_name": null,
    "middle_name": null,
    "last_name": null,
    "email": null,
    "contact_number": null,
    "suffix": null,
    "fulfillment_status": 0,
    "order_status": 0,
    "status": "active",
    "created_at": "2018-05-24T14:46:40.559Z",
    "updated_at": "2018-05-24T14:46:40.559Z"
  }
}
```

`POST /api/v1/orders`


## Get Order

### HTTP Request

```json
{
  "order": {
    "id": 1,
    "account_id": 1,
    "customer_id": 1,
    "user_id": 1,
    "order_number": 25,
    "note": null,
    "total_line_items_price": "0.0",
    "total_discounts": "0.0",
    "subtotal": "0.0",
    "total_price": "0.0",
    "total_tax": "0.0",
    "total_weight": "0.0",
    "first_name": null,
    "middle_name": null,
    "last_name": null,
    "email": null,
    "contact_number": null,
    "suffix": null,
    "fulfillment_status": 0,
    "order_status": 0,
    "status": "active",
    "created_at": "2018-05-24T14:46:40.559Z",
    "updated_at": "2018-05-24T14:46:40.559Z"
  }
}
```

`POST /api/v1/orders`
