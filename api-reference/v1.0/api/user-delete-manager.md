---
title: "Remove manager"
description: "Remove a user's manager."
ms.localizationpriority: medium
author: "yyuank"
ms.prod: "users"
doc_type: apiPageType
---

# Remove manager

Namespace: microsoft.graph

Remove a user's manager.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadWrite.All, Directory.ReadWrite.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.ReadWrite.All, Directory.ReadWrite.All |

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/manager/$ref
```

## Request headers

| Header       | Value |
|:---------------|:----------|
| Authorization  | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns `204 No Content` response code. It does not return anything in the response body.

## Example

##### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "remove_manager"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
```

##### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 7ac5b390-b3bf-11ed-afa1-0242ac120002
2023-02-23 22:41:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove a user's manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
