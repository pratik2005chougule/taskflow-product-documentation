# Projects API

## Overview

The Projects API allows applications to create, view, update, and manage projects.

## Get All Projects

### Request

```http
GET /projects
```

### Response

```json
[
  {
    "id": 101,
    "name": "Website Launch"
  }
]
```

## Create a Project

### Request

```http
POST /projects
```

```json
{
  "name": "Website Launch",
  "description": "Marketing website redesign"
}
```

### Response

```json
{
  "id": 101,
  "name": "Website Launch"
}
```

## Update a Project

```http
PUT /projects/{id}
```

## Delete a Project

```http
DELETE /projects/{id}
```

## Response Codes

| Code | Description |
|--------|-------------|
| 200 | Success |
| 201 | Created |
| 404 | Not Found |
| 500 | Server Error |