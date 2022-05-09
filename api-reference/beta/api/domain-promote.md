---
title: "domain: promote"
description: "Promotes subdomain to root domain."
author: "franqq"
ms.localizationpriority: medium
ms.prod: "directory-management"
doc_type: apiPageType
---

# domain: promote

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Promotes subdomain to root domain.

> **Important:**
> Only applies to an verified domain. For a verified domain, the isVerified property of the [domain](../resources/domain.md) is true.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).


|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Domain.ReadWrite.All   |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Domain.ReadWrite.All |

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/promote
```

> For {id}, specify the domain with its fully qualified domain name.

## Request headers

| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {token}. Required.|
| Content-Type  | application/json |

## Request body

## Response

If successful, this method returns `204 No Content` response code.

## Example
##### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_promote"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/promote
```
# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-promote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-promote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-promote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-promote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/domain-promote-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/domain-promote-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### Response
Note: The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
Content-type: application/json
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: promote",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

