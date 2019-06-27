---
title: 获取 identityRiskEvent
description: 检索 identityriskevent 对象的属性和关系。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 278ab64417b4da7db2aa736e1be934aa25d6f1bb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262634"
---
# <a name="get-identityriskevent"></a>获取 identityRiskEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 identityriskevent 对象的属性和关系。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | IdentityRiskEvent.Read.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | IdentityRiskEvent.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_identityriskevent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_identityriskevent-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_identityriskevent-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
