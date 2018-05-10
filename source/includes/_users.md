

# Users

## Get all users
```sh
  curl --request GET \
    --url 'http://example.com/api/v1/users' \
    --header 'Authorization: <Processed Basic hash>' \
    --header 'Content-Type: application/json' \
```

<aside class"notice">
  Use your <code>token</code> and <code>auth_token</code> as username and password on Basic authentication
</aside>

### HTTP Request

```json
{
  "users": [
    {
      "id": 1,
      "account_id": 1,
      "email": "admin@first_company.com",
      "first_name": "Juan",
      "middle_name": null,
      "last_name": "Dela Cruz",
      "suffix": null,
      "title": null,
      "password_digest": "$2a$10$o2IBZrnngsb6gWMxNthU6OwH2Cz1yNwZr5pyGaoQFL8NPlHUogAzG",
      "user_type": null,
      "user_status": 0,
      "token": "Qt4KrDQyzMWA4AwPJ5qEXdsS",
      "status": "active",
      "created_at": "2018-05-10T13:01:11.560Z",
      "updated_at": "2018-05-10T13:01:11.560Z"
    }
  ]
}
```

`GET /api/v1/users`

### Response

Key | Type    | Description
--------- | ------- | -----------
`users`       | Array  | Collection of users
