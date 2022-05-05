---
title: 列出对话
description: 检索此组中的会话列表。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1489e2629b9babd01d601002f4c5a5cb2113a440
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211219"
---
# <a name="list-conversations"></a>列出对话

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索此组中的[对话](../resources/conversation.md)列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Group.Read.All、Group.ReadWrite.All         |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| Application                            | Group.Read.All、Group.ReadWrite.All         |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持`$select` 和 `$filter` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 标头        | 值                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-conversations-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-conversations-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-conversations-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/get-conversations-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f448435d-3ca7-4073-8152-a1fd73c0fd09')/conversations",
    "value": [
        {
            "id": "AAQkAGFhZDhkNGI1LTliZmEtNGEzMi04NTkzLWZjMWExZDkyMWEyZgAQAH4o7SknOTNKqAqMhqJHtUM=",
            "topic": "The new All Company group is ready",
            "hasAttachments": false,
            "lastDeliveredDateTime": "2021-08-02T10:34:00Z",
            "uniqueSenders": [
                "All Company"
            ],
            "preview": "Welcome to the All Company group.Use the group to share ideas, files, and important dates.Start a conversationRead group conversations or start your own.Share filesView, edit, and share all group files, including email attachments.Connect your"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
