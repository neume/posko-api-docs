

# Customers

## Get all customers
```sh
  curl --request GET \
    --url 'http://example.com/api/v1/customers' \
    --header 'Authorization: <Processed Basic hash>' \
    --header 'Content-Type: application/json' \
```

### HTTP Request

```json
{
  "customers": [
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

`GET /api/v1/customers`

### Response

| Key         | Type  | Description             |
|:------------|:------|:------------------------|
| `customers` | Array | Collection of customers |




## Create Customer

### HTTP Request

```json
{
  "customer": {
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
}
```

`POST /api/v1/customers`


## Get Customer

### HTTP Request

```json
{
  "customer": {
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
}
```

`POST /api/v1/customers`
