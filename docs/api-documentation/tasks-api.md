# Tasks API

## Overview

The Tasks API enables applications to create, update, retrieve, and delete tasks within TaskFlow projects.

## Get All Tasks

### Request

```http
GET /tasks
```

### Response

```json
[
  {
    "id": 501,
    "title": "Design Homepage",
    "status": "In Progress"
  }
]
```

## Create a Task

### Request

```http
POST /tasks
```

```json
{
  "title": "Design Homepage",
  "description": "Create homepage wireframes",
  "assignee": "user123"
}
```

### Response

```json
{
  "id": 501,
  "title": "Design Homepage"
}
```

## Update a Task

```http
PUT /tasks/{id}
```

## Delete a Task

```http
DELETE /tasks/{id}
```

## Status Codes

| Code | Description |
|--------|-------------|
| 200 | Success |
| 201 | Created |
| 400 | Bad Request |
| 404 | Not Found |
| 500 | Internal Server Error |