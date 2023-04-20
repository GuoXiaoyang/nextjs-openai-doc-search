---
title: External Business API Documentation V1
slug: external-business-api-documentation-v1
date_published: 1970-01-01T00:00:00.000Z
date_updated: 2023-01-31T23:16:07.000Z
draft: true
---

- [Notice](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Notice)
- [Basic information](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Basic-information)
- [Authentication](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Authentication)
- [Rate limits](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Rate-limits)
- [Authorization](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Authorization)
- [Login](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Login)
- [Business](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Business)
- [Get all associated businesses and accounts](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Get-all-associated-businesses-and-accounts)
- [Payments](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Payments)
- [Get all payments](https://moego.atlassian.net/wiki/spaces/ET/pages/173604865/External+Business+API+Documentation+V1#Get-all-payments)

# Notice

1. **This is not the official open API, but for internal use of MoeGo products, which may change at any time. We will launch the official open API later.**

# Basic information

1. The API domain is `https://go.moego.pet`.
2. Only HTTP protocol is supported. Includes `HTTP/2` and `HTTP/1.1`.

If there is no special statement, the data serialization protocol of all API is `JSON`, which means:

1. If the request contains a body part, you need to set the `Content-Type` in the header to `application/json`, and serialize the body using `JSON`.
2. The response body is always serialized by `JSON`, and the `Content-Type` in response is always `Content-Type: application/json`.

## Authentication

1. Get your `accountToken` and `staffToken` by calling Login API.
2. Set the `Account-Token` and `Staff-Token` in the request header to your `accountToken` and `staffToken` respectively.

## Rate limits

1. We don't have a clear rate limit rule. But your request frequency should not exceed 5 times per second (all APIs together). Otherwise, you may be banned.

# Authorization

## Login

**API Identifier**: `POST https://go.moego.pet/api/business/account/login`

**Request Body:**`1{2    "email": "xxx",    # Required, your email 3    "password": "xxx"  # Required, your password 4}`

**Response Body:**`1{2    "code": 200,3    "message": "Operation is successful !",4    "data": {5        "accountToken": "xxx", *// Your accountToken*6        "staffToken": "xxx"    *// The staffToken of the business you last visited,*7                               *// It maybe null if you have no business*8    },9    "success": true10}`

**Note:**

1. This API does not need Authentication

# Business

## Get all associated businesses and accounts

**API Identifier: **`POST https://go.moego.pet/api/business/myAccount/queryWithBusiness`

**Response Body:**`1{2    "code": 200,3    "message": "Operation is successful !",4    "data": {5        "account": {                      *// My account info*6            "accountId": 000,             *// My account id*7            "email": "xxx",               *// My email*8            "avatarPath": "xxx",          *// My avatar*9            "firstName": "xxx",           *// My first name*10            "lastName": "xxx",            *// My last name*11            "phoneNumber": "xxx",         *// My phone number*12            "token": "xxx",               *// My accountToken*13            "lastBusinessId": 000,        *// My last visited business's id*14            "status": 1,15            "createTime": 016        },17        "businessInfo": [                 *// My associated business list*18            {19                "accountId": 000,         *// My account id*20                "staffId": 000,           *// My staff id in the business*21                "staffToken": "xxx",      *// My staffToken for the business*22                "employeeCategory": 1,    *// My role type, 0 is staff, 1 is owner*23                "businessId": 000,        *// The business's id*24                "businessName": "xxx",    *// The business's name*25                "avatarPath": "xxx"       *// The business's avatar*26            }27        ],28        "relevantAccountDto": [           *// My associated account list*29            {30                "accountId": 000,         *// The associated account id*31                "staffId": 000,           *// The account last visited business's staff id*32                "staffToken": "xxx",      *// The account last visited business's staffToken*33                "employeeCategory": 1,    *// The account last visited business's staff type*34                "businessId": 000,        *// The account last visited business's id*35                "businessName": null,     *// bad field*36                "avatarPath": "xxx",      *// bad field*37                "accountToken": "xxx",    *// The account's accountToken*38                "accountEmail": "xxx",    *// The account's email*39                "accountFirstName": "xxx",*// The account's first name*40                "accountLastName": "xxx"  *// The account's last name*41            }42        ]43    },44    "success": true45}`

**Note:**

1. If you want to switch business, you can choose the business’s `staffToken` as the value of request header `Staff-Token`
2. If you want to switch account, you can use the account’s `accountToken` as the value of request header `Account-Token`(The `Staff-Token` should be replaced at the same time).
3. This API only requires `Account-Token` authentication.

# Payments

## Get all payments

**API Identifier: **`GET https://go.moego.pet/api/payment/payment/list`

**Query String Parameters:**`1order:        # Optional, set the order of the results (by create time), the value 2              #   could be 'asc', 'desc'. default is 'desc'. 3vendor:       # Optional, filter by credit card payment vendor, the value could be 4              #   'stripe', 'square'. default is empty. 5method:       # Optional, filter by the payment method, which is configured by your 6              #   business, the value is the payment method name. eg: 'credit card'. 7              #   default is empty. 8customerId:   # Optional, filter by the customer id. default is empty. 9pageNum:      # Optional, the page num, starts with 1, default is 1. 10pageSize:     # Optional, the items included per page, should in [0, 100], default 11              #   is 20.`

**Response Body:**`1{2    "code": 200,3    "message": "Operation is successful !",4    "data": {5        "paymentCount": 50,                   *// The total payment items*6        "paymentList": [                      *// The payment list*7            {8                "id": 000,                    *// The payment id*9                "businessId": 000,            *// Your business id*10                "module": "grooming",         *// The payment source, could be 'grooming' or 'retail'*11                "invoiceId": 000,             *// The order id*12                "customerId": 000,            *// The customer id*13                "staffId": 000,               *// The staff id*14                "method": "xxx",              *// The payment method name*15                "amount": 00.00,              *// The amount*16                "processingFee": 00.00,       *// The processing fee, only avaiable for 'Credit card' method*17                "status": 2,                  *// The status, value means: 0 created, 1 processing, 2 paid, 3 completed, -1 failed*18                "checkNumber": "000",         *// The check number, only available for 'Check' method*19                "cardType": "xxx",            *// The credit card's type, eg: 'visa'.*20                "cardNumber": "000",          *// The credit card's last 4 digit*21                "expMonth": "00",             *// The credit card's expire month*22                "expYear": "0000",            *// The credit card's expire year*23                "signature": "xxx",           *// The customer submitted signature, maybe base64 string or uploaded file url*24                "paidBy": "xxx",              *// The paied by*25                "description": "xxx",         *// The description*26                "methodId": 000,              *// The payment method id*27                "squarePaymentMethod": 000,   *// The square payment method id, only avaiable for 'square' vendor, value means: 1 - card, 2 - card on file, 3- terminal, 4 - reader sdk*28                "stripePaymentMethod": 000,   *// The stripe payment method id, only avaiable for 'stripe' vendor, value means: 1 - card, 2 - card on file, 3- bluetooth, 4 - smart reader  5 - apple pay, 6 - google pay*29                "isOnline": true,             *// Bad field*30                "createTime": 000,            *// The create time in unix seconds*31                "updateTime": 000,            *// The update time in unix seconds*32                "cancelReason": "xxx",        *// The square cancel reason*33                "locationId": "xxx",          *// The square location id*34                "customerName": "xxx",        *// The customer's name*35                "refunds": [],                *// The refunds history*36                "groomingId": 000,            *// The grooming id, only avaiable for 'grooming' module*37                "isPrepay": true,             *// Is prepay or not*38                "refundedAmount": 0           *// The total refunded amount*39            }40        ]41    },42    "success": true43}`

**Examples:**

Get the latest 50 stripe payments of your business by `curl`:`1curl 'https://go.moego.pet/api/payment/payment/list?order=desc&vendor=stripe&method=credit%20card&pageNum=1&pageSize=50' \ 2    -H 'Account-Token: YOUR_ACCOUNT_TOKEN' \ 3    -H 'Staff-Token: YOUR_STAFF_TOKEN'`
