---
title: "Search Calendar Events"
description: "You are able to search in user’s own calendar."
author: "knightsu"
localization_priority: Normal
ms.prod: "search"
---

# Search Calendar Events

You are able to search in user’s own calendar.

## Search calendar events

Request

```HTTP
POST /search/query
Content-Type: application/json
Authorization: Bearer AAD_TOKEN
```

Response

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.event"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## Known limitations

- You can only access user’s own calendar. Shared or delegated access is not supported.

## Next steps

Find out more about:

- The [search API](/graph/api/search-query?view=graph-rest-beta)