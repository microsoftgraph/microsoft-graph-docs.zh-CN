---
title: 消息： 取消订阅
description: 提交代表登录用户的电子邮件请求取消订阅电子邮件通讯组列表。 使用中的信息`List-Unsubscribe`标头。
author: angelgolfer-ms
ms.openlocfilehash: e516a8aa68bde02f056e503da9c85d4e7a6f62fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357223"
---
# <a name="message-unsubscribe"></a>消息： 取消订阅

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

提交代表登录用户的电子邮件请求取消订阅电子邮件通讯组列表。 使用中的信息`List-Unsubscribe`标头。

邮件发件人可以使用邮件列表以用户友好的方式通过包括一个选项以收件人退出。他们可以通过指定实现`List-Unsubscribe`关注[RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)每个邮件中的页眉。

**注释**具体而言，以**取消**操作，发件人必须指定`mailto:`和不基于 URL 的取消信息。

设置该标题将对[邮件](../resources/message.md)实例与**unsubscribeEnabled**属性还设置`true`，并**unsubscribeData**属性设为标题数据。

如果一条消息的**unsubscribeEnabled**属性是`true`，您可以使用**取消**操作取消类似今后的邮件用户管理邮件发件人。

成功，则**取消**操作会将邮件移到**已删除邮件**文件夹中。 发件人管理将来邮件通讯组从实际的用户的排除。

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
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a>请求标头
| Name       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
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
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
