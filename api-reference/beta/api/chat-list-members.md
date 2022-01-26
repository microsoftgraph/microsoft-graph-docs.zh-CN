---
title: 列出聊天成员。
description: 检索聊天成员。
author: bhartono
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5f831e3762e61e915f65a49a4f0bdadb71f6062f
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225565"
---
# <a name="list-members-of-a-chat"></a>列出聊天成员。

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出[聊天](../resources/chat.md)中的所有[对话成员](../resources/conversationmember.md)。

> [!NOTE]
> 服务器返回的成员 ID 必须作为不透明的字符串处理。 客户端不应尝试对这些资源 ID 进行分析或做出任何假设。
>
> 未来，成员资格结果可以映射到来自不同租户的用户，如响应中所示。客户端不应假定所有成员仅来自当前租户。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|---------|-------------|
|委派（工作或学校帐户）| ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All |

> **注意**：标有 * 的权限用于 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

> [!NOTE]
> 在使用应用程序权限调用此 API 之前，必须先请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members
GET /users/{user-id | user-principal-name}/chats/{chat-id}/members
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

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
   "@odata.count":3,
   "value":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
         "roles":[
            "owner"
         ],
         "displayName":"John Doe",
         "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"2019-04-18T23:51:43.255Z"
      },
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"2de87aaf-844d-4def-9dee-2c317f0be1b3",
         "roles":[
            "owner"
         ],
         "displayName":"Bart Hogan",
         "userId":"2de87aaf-844d-4def-9dee-2c317f0be1b3",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"0001-01-01T00:00:00Z"
      },
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"07ad17ad-ada5-4f1f-a650-7a963886a8a7",
         "roles":[
            "owner"
         ],
         "displayName":"Minna Pham",
         "userId":"07ad17ad-ada5-4f1f-a650-7a963886a8a7",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"2019-04-18T23:51:43.255Z"
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
