# Authentication

## Overview

TaskFlow APIs require authenticated requests.

Authentication is performed using bearer access tokens.

## Obtain an Access Token

Example request:

```http
POST /auth/token
```

Request Body:

```json
{
  "username": "user@example.com",
  "password": "password"
}
```

## Example Response

```json
{
  "access_token": "eyJhbGc...",
  "token_type": "Bearer",
  "expires_in": 3600
}
```

## Use the Token

Example:

```http
Authorization: Bearer eyJhbGc...
```

## Authentication Errors

| Code | Description |
|--------|-------------|
| 401 | Invalid Token |
| 403 | Access Denied |

## Security Recommendations

- Store tokens securely.
- Rotate credentials regularly.
- Use HTTPS.
- Avoid exposing tokens in logs.