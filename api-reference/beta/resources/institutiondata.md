---
title: "institutionData resource type"
description: "PROVIDE DESCRIPTION HERE"
localization_priority: Normal
author: "kevinbellinger"
ms.prod: "People"
doc_type: "resourcePageType"
---

# institutionData resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The 'institutionData' resource type provides detailed information about the institute a user undertook an undergraduate, graduate, postgraduate degree or other program at.

## Properties

| Property     | Type                                 | Description                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|description   |String                                |Short description of the institution the user studied at. |
|displayName   |String                                |Name of the institution the user studied at.              |
|location      |[physicalAddress](physicaladdress.md) |Address or location of the institute.                     |
|webUrl        |String                                |Link to the institution or department homepage.           |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->