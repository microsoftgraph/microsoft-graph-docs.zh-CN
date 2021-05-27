---
title: 创建对话
description: '通过包括线程和帖子创建新对话。 '
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a5e191e5cfb99b9ebad18af1ba7d530d79fa6e69
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681403"
---
# <a name="create-conversation"></a>创建对话

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过添加线程和帖子来新建[对话](../resources/conversation.md)。 

使用[回复线程](conversationthread-reply.md)或[回复帖子](post-reply.md)进一步发布到该对话。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供包括 [conversationThread](../resources/conversationthread.md) 和 [帖子](../resources/post.md) 的 [conversation](../resources/conversation.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversation](../resources/conversation.md) 对象。 

响应包括新对话和线程的 ID，这些 ID 也可用于[列出帖子](conversationthread-list-posts.md)操作，从而获取新帖子。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
  "topic":"New head count",
  "threads":[
    {
      "posts":[
        {
          "body":{
            "contentType":"html",
            "content":"The confirmation will come by the end of the week."
          },
          "newParticipants":[
            {
              "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
              }
            }
          ]
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
  "id":"AAQkADPxBgqECsrFDTuM=",
  "threads@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADPxBgqECsrFDTuM%3D')/threads",
  "threads":[
    {
      "id":"AAQkADUNO4xAAMbGA93Sw-EGCoQKysUNO4w=="
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


