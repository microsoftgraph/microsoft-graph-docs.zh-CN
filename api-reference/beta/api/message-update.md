---
title: 更新邮件
description: 更新 message 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6553365ffd31c56348c930be5562ebd65abc734d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977764"
---
# <a name="update-message"></a>更新邮件

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新消息对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Mail.ReadWrite    |
|委派（个人 Microsoft 帐户） | Mail.ReadWrite    |
|应用程序 | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | string  | 实体正文中的数据性质。必需。 |
## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，不应包括尚未更改的现有值。 以下属性可以进行更新。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|Recipient|邮件的密件抄送收件人。 |
|body|ItemBody|邮件的正文。 可更新才 isDraft = true。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|收件人集合|邮件的抄送收件人。 |
|发件人|Recipient|邮箱所有者和邮件发件人。 必须为实际的邮箱使用相对应。 |
|importance|String|邮件的重要性。可能的值是：`Low`、`Normal`、`High`。|
|inferenceClassification | String | 根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。 |
|internetMessageId |String |由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。 可更新才 isDraft = true。|
|isDeliveryReceiptRequested|布尔|指示是否需要发送邮件已读回执。|
|isRead|布尔|指示是否已阅读该邮件。|
|isReadReceiptRequested|布尔|指示是否需要发送邮件已读回执。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合| 多值为消息定义的扩展属性的集合。 可为 Null。|
|replyTo|Recipient collection|在答复时使用的电子邮件地址。 可更新才 isDraft = true。|
|sender|Recipient|实际用于生成邮件的帐户。 从[共享的邮箱](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)，或作为[委派](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送一条消息发送邮件时可更新。 在任何情况下的值必须为实际的邮箱使用对应。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| 为消息定义的单值扩展属性的集合。 可为 Null。|
|subject|String|邮件的主题。 可更新才 isDraft = true。|
|toRecipients|Recipient collection|邮件的收件人。 |

由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
