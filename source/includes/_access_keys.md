

# Access Keys

## Get access keys of current customer
```sh
  curl --request GET \
    --url 'http://example.com/api/v1/access_keys' \
    --header 'Authorization: <Processed Basic hash>' \
    --header 'Content-Type: application/json' \
```


### HTTP Request

```json
{
  "access_keys": [
    {
      "id": 1,
      "user_id": 1,
      "token": "eJfds7aZbTYoxKMDZSFXD6Ad",
      "auth_token": "sLMaNwwkrMEa4CA6YVYGCKm2",
      "access_key_status": 0,
      "status": "active",
      "created_at": "2018-05-20T07:20:56.863Z",
      "updated_at": "2018-05-20T07:20:56.863Z"
    }
  ]
}
```

`GET /api/v1/access_keys`

### Response

| Key           | Type  | Description          |
|:--------------|:------|:---------------------|
| `access_keys` | Array | Collection of tokens |
