---
title: 列出 contentSharingSessions
description: 检索调用中 contentSharingSession 对象的列表。
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b0136bb6942e523e218f72232d635a8c159989f3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211602"
---
# <a name="list-contentsharingsessions"></a>列出 contentSharingSessions

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索调用中 [contentSharingSession](../resources/contentsharingsession.md) 对象的列表。

## <a name="permissions"></a>权限

| 权限类型 | 权限（从最低特权到最高特权） |
| :-------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持。       |
| 委派（个人 Microsoft 帐户） | 不支持。       |
| Application     | Calls.JoinGroupCallAsGuest.All、Calls.JoinGroupCall.All、Calls.Initiate.All、Calls.InitiateGroupCall.All                                        |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /communications/calls/{id}/contentSharingSessions
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contentSharingSession](../resources/contentsharingsession.md) 对象的集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

请求示例如下所示。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-contentsharingsessions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/contentSharingSessions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contentsharingsessions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contentsharingsessions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contentsharingsessions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contentsharingsessions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-contentsharingsessions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-contentsharingsessions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.contentSharingSession",
  "isCollection": true,
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.type":"#microsoft.graph.contentSharingSession",
         "id":"a7ebfb2d-871e-419c-87af-27290b22e8db"
      },
      {
         "@odata.type":"#microsoft.graph.contentSharingSession",
         "id":"278405a3-f568-4b3e-b684-009193463064"
      }
   ],
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/contentSharingSessions"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contentSharingSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
