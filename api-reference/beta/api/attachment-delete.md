---
title: 删除附件
description: 从日历事件、 邮件、 Outlook 任务或公告中删除附件。
ms.openlocfilehash: dbabde6b1783e477e3a15db3ea4d138be6e41b12
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771784"
---
# <a name="delete-attachment"></a>删除附件

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

从日历[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)删除附件。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

* 如果访问邮件中的附件： Mail.ReadWrite
* 如果访问事件中的附件： Calendars.ReadWrite
* 如果访问 Outlook 任务中的附件： Tasks.ReadWrite
* 如果访问组文章中的附件： Group.ReadWrite.All

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a>HTTP 请求

[事件](../resources/event.md)的附件。

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

用户邮箱中的 [邮件](../resources/message.md) 附件。
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

[邮件](../resources/message.md)的用户的邮箱中[mailFolder](../resources/mailfolder.md)子文件夹中包含的附件。  下面的示例演示一个级别的嵌套，但一条消息可以位于子级的子级，依此类推。
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

为[Outlook 任务](../resources/outlooktask.md)的附件。
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面的示例展示了用于删除事件的附件的请求。
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a>响应

下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
