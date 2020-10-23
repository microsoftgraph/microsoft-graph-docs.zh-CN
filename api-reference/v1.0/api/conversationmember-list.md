---
title: 列出 conversationMembers
description: 检索聊天或频道成员的列表。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8efb0b6c6647f48bf64de04a25a564ae0b3a00e8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700877"
---
# <a name="list-conversationmembers"></a>列出 conversationMembers

命名空间：microsoft.graph

列出[聊天](../resources/chatmessage.md)或[频道](../resources/channel.md)中的所有[对话成员](../resources/conversationmember.md)。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|---------|-------------|
|委派（工作或学校帐户）| Chat.ReadBasic, Chat.Read, Chat.ReadWrite |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

> [!NOTE]
> 在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a>可选的查询参数

此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/chats/{id}/members
```

### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
