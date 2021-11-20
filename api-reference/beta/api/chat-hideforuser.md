---
title: chat： hideForUser
description: 隐藏用户的聊天。
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.openlocfilehash: 88cef270a068b84541c3782da4aa782040d80264
ms.sourcegitcommit: 70b3caded085ba8ef15e389f81fa005506f1e2fb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2021
ms.locfileid: "61131960"
---
# <a name="chat-hideforuser"></a>chat： hideForUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

隐藏 [用户的](../resources/chat.md) 聊天。

> **注意：** 如果在聊天级别执行诸如发送消息等操作，则用户会自动取消聊天。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Chat.ReadWrite|
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatsId}/hideForUser
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|Description|
|:---|:---|:---|
|用户|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|要隐藏聊天的用户。 **在委派模式下，用户只能为自己隐藏聊天**。|
|tenantId|String|用户的租户 ID。|

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chat_hideforuser"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces/hideForUser
Content-Type: application/json

{
  "user": {
    "id" : "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
  },
  "tenantId": "2a690434-97d9-4eed-83a6-f5f13600199a"
}
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

