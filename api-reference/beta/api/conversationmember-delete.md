---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a6ac8b72f5dea24c0f60062b91dac7648b91e85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436564"
---
# <a name="delete-conversationmember"></a>删除 conversationMember

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从[频道](../resources/channel.md)中删除[conversationMember](../resources/conversationmember.md) 。

> [!NOTE]
> 此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的`private`通道上受支持。 与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回`400 Bad Request`响应。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|---------|-------------|
|委派（工作或学校帐户）|对于**用户**或**聊天**资源：<br/>Chat.Read、Chat.ReadWrite<br/><br/>对于**频道**资源：<br/>Group.Read.All、Group.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序| 对于**用户**或**聊天**资源：<br/>Chat.Read.All、Chat.ReadWrite.All<br/><br/>对于**频道**资源：<br/>Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
