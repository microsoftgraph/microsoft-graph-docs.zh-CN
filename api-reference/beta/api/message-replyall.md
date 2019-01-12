---
title: 消息：replyAll
description: '通过指定注释和修改任何可更新属性回复邮件的所有收件人 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1abbf271350c6bbbd10af1f17c6c7d3069c3cf22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976364"
---
# <a name="message-replyall"></a>消息：replyAll

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

通过指定注释和所有使用**replyAll**方法修改的回复，任何可更新属性回复邮件的所有收件人。 然后在已发送邮件文件夹中保存邮件。

此外，您可以第一个[创建草稿全部答复邮件](../api/message-createreplyall.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)答复。

**注意**

- 您可以指定注释或的**body**属性`message`参数。 如果同时指定将返回 HTTP 400 错误请求出错。
- 如果**回复**属性指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应发送给收件人的答复  
**回复**和**toRecipients**属性，并不**从**和**toRecipients**属性中的收件人。 


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Mail.Send    |
|委派（个人 Microsoft 帐户） | Mail.Send    |
|应用程序 | Mail.Send |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | string  | 实体正文中的数据性质。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|注释|String|要包含的注释。可以为空字符串。|
|message|[message](../resources/message.md)|若要在答复邮件更新任何可写属性。|

## <a name="response"></a>响应

如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
下面的示例包括一条注释，并将添加到全部答复邮件附件。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```


##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
