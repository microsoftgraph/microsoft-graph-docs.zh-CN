---
title: chatMessage： undoSoftDelete
description: 在频道或聊天中取消删除单条消息或消息回复。
author: Ramjot Singh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.openlocfilehash: 353b41cee2ab489f88eaec8b5a6d6f3d19560722
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768356"
---
# <a name="chatmessage-undosoftdelete"></a>chatMessage： undoSoftDelete

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

撤消在[频道](../resources/channel.md)或[聊天](../resources/chat.md)中软删除单条[消息](../resources/chatmessage.md)或[邮件回复](../resources/chatmessage.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-for-channel"></a>频道权限

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
|委派（工作或学校帐户）| ChannelMessage.ReadWrite |
|委派（个人 Microsoft 帐户）| 不支持 |
|应用程序| 不支持 |

> **Note**： 仅支持使用 ** 标记的权限以实现向后兼容。 建议更新解决方案，以使用上表中列出的替代权限，并避免今后使用这些权限。

### <a name="permissions-for-chat"></a>聊天权限

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
|委派（工作或学校帐户）| ChatMessage.ReadWrite |
|委派（个人 Microsoft 帐户）| 不支持 |
|应用程序| 不支持 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/chats/{chatsId}/messages/{chatMessageId}/undoSoftDelete
POST /teams/{teamsId}/channels/{channelId}/messages/{chatMessageId}/undoSoftDelete
POST /teams/{teamId}/channels/{channelId}/messages/{messageId}/replies/{replyId}/undoSoftDelete
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

### <a name="example-1-undo-soft-deletion-of-a-message-in-a-chat"></a>示例 1：撤消聊天中邮件的软删除

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-undosoftdelete1"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/8f98f01d-1a73-401a-b9e9-9fd1e6f5e5ap/chats/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-undo-soft-deletion-of-a-message-in-a-channel"></a>示例 2：撤消频道中邮件的软删除

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chatmessagethis2undosoftdelete2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-undo-soft-deletion-of-a-message-of-a-reply-in-a-channel"></a>示例 3：撤消软删除通道中答复的消息

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-undosoftdelete3"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```
