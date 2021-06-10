---
title: 消息：答复
description: 使用 JSON 或 MIME 格式答复邮件的发件人。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5a9cab87389f41c795268a1d7964a7d8e987269
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870498"
---
# <a name="message-reply"></a>消息：答复

命名空间：microsoft.graph。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 JSON 或 MIME [格式](../resources/message.md) 答复邮件的发件人。

使用 JSON 格式时：
- 指定参数的 comment 或 **body** `message` 属性。 指定这两者将返回 HTTP 400 错误请求错误。
- 如果原始邮件在 **replyTo** 属性中指定收件人，则根据 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ，将答复发送给 **replyTo** 中的收件人，而不是 **from** 属性中的收件人。

使用 MIME 格式时：
- 提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，所有内容在请求正文中都通过 **base64** 格式进行编码。
- 向 MIME 内容添加任何附件和 S/MIME 属性。

此方法将邮件保存在 **“已发送邮件”** 文件夹中。

或者，[创建一个草稿以答复邮件，](../api/message-createreply.md)[并稍后](../api/message-send.md)发送。

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
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。 必需 |
| Content-Type | string  | 实体正文中的数据性质。 必需 <br/> 用于 `application/json` JSON 对象和 `text/plain` MIME 内容 |

## <a name="request-body"></a>请求正文
使用 JSON 格式时，请包含具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|注释|String|要包含的注释。可以为空字符串。|
|message|[message](../resources/message.md) | 回复邮件中要更新的任何可写属性。|

指定 MIME 格式的正文时，请提供 MIME 内容以及适用的 Internet 邮件头，所有邮件头在请求正文中都以 **base64** 格式进行编码。 此方法使用原始邮件的发件人作为收件人。

## <a name="response"></a>响应

如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。

如果请求正文包含错误的 MIME 内容，此方法将返回 `400 Bad request` 和以下错误消息：“无效的 base64 字符串 MIME 内容”。

## <a name="examples"></a>示例
### <a name="example-1-reply-to-a-message-in-json-format"></a>示例 1：以 JSON 格式答复邮件
以下示例包含注释，并将收件人添加到回复邮件中。
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}

```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
下面是一个响应示例。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-to-a-message-in-mime-format"></a>示例 2：以 MIME 格式答复邮件
##### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "message_reply_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: text/plain

UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIE1pY3Jvc29mdCAKU01UUCBTZXJ2ZXIgKHZlcnNpb249VExTMV8yLCAKY2lwaGVyPVRMU19FQ0RIRV9SU0FfV0lUSF9BRVNfMjU2X0NCQ19TSEEzODRfUDI1NikgaW

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

如果请求正文包含错误的 MIME 内容，此方法返回以下错误消息。

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
