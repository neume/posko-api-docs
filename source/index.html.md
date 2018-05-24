---
title: POSko API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - sh
toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - users
  - access_keys
  - customers
  - orders

search: true
---

# Introduction

Welcome to POSko API documentation. POSko is under active development. Expect
breaking changes on each commit. We encourage you to reset your database before
running migrations.

This API contains basic functionalities and exposes unfiltered data. Requests may
return sensitive information like ```password_digest``` and other keys but those
are intentional. Those keys will be removed when the core functionalities are ready.

# Authentication

## Sign In

> This request will return a JSON similar to this

```json
{
  "user": {
    "email": "admin@first_company.com",
    "token": "t4s7yrtGqKKfwvQik9WgKFyN",
    "auth_token": "8CWo9VBGV7WEUxhgvuKRrhv4",
    "created_at": "2018-05-10T13:01:11.560Z"
  }
}
```
Use using Basic authentication

### HTTP Request


`POST /api/v1/sign_in`

### Paramaters


Parameter | Type    | Description
--------- | ------- | -----------
`account_name` | String  | The account name of the user. ex: ```the_green_store```
`email`        | String  | The email address of the user
`password`     | String  | Password of the user


### Response

Parameter | Type    | Description
--------- | ------- | -----------
`token`       | String  | A unique token that will serve as the `username` in Basic Auth
`auth_token`  | String  | The password



This endpoint returns the necessary tokens to be used in your future requests
