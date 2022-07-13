---
title: chatMessage： softDelete
description: 删除频道或聊天中的单条消息或消息回复。
author: Ramjot Singh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.openlocfilehash: df9262e051c59760d3890e772dbc3857afc6182b
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768352"
---
# <a name="chatmessage-softdelete"></a>chatMessage： softDelete

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除[频道](../resources/channel.md)或[聊天](../resources/chat.md)中的单[条消息](../resources/chatmessage.md)或[消息回复](../resources/chatmessage.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-for-channel"></a>频道权限

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
|委派（工作或学校帐户）| ChannelMessage.ReadWrite |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

### <a name="permissions-for-chat"></a>聊天权限

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
|委派（工作或学校帐户）| ChatMessage.ReadWrite |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/chats/{chatsId}/messages/{chatMessageId}/softDelete
POST /teams/{teamsId}/channels/{channelId}/messages/{chatMessageId}/softDelete
POST /teams/{teamId}/channels/{channelId}/messages/{messageId}/replies/{replyId}/softDelete
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-soft-delete-message-in-a-chat"></a>示例 1：聊天中的软删除消息

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-softdelete1"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/8f98f01d-1a73-401a-b9e9-9fd1e6f5e5ar/chats/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/softDelete
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-soft-delete-message-in-a-channel"></a>示例 2：通道中的软删除消息

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "chatmessagethis-softdelete2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/softDelete
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-soft-delete-message-of-a-reply"></a>示例 3：答复的软删除消息

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "chatmessagethis-softdelete3"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/replies/1649852161658/softDelete
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```
