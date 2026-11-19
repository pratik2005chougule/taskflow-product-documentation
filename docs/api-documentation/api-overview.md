# API Overview

## Introduction

The TaskFlow API allows developers to integrate external applications with TaskFlow.

The API follows REST principles and uses JSON for request and response payloads.

## Base URL

```text
https://api.taskflow.example.com/v1
```

## Supported Operations

The API supports:

- Project management
- Task management
- User management
- Reporting
- Integrations

## Request Format

Example:

```http
GET /projects
```

## Response Format

```json
{
  "id": 101,
  "name": "Marketing Website Launch"
}
```

## Authentication

All API requests require authentication using access tokens.

## HTTP Status Codes

| Code | Description |
|--------|-------------|
| 200 | Success |
| 201 | Created |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Server Error |

## Related Documentation

- Authentication
- Projects API
- Tasks API