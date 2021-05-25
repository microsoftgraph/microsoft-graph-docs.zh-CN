---
title: 更新邮件
description: 更新 message 对象的属性。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c9c3e9f13a592738ebd4245015a9458a0856dda8
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645337"
---
# <a name="update-message"></a>更新邮件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 message 对象的属性。
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
在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可进行以下属性的更新。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|收件人|邮件的密件抄送收件人。 |
|body|ItemBody|邮件的正文。仅当 isDraft = true 时可以更新。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|收件人集合|邮件的抄送收件人。 |
|flag|[followupFlag](../resources/followupflag.md)|指示邮件的状态、开始日期、截止日期或完成日期的标志值。|
|发件人|收件人|邮箱所有者和邮件发件人。 必须对应于使用的实际邮箱。 |
|importance|String|邮件的重要性。可能的值是：`Low`、`Normal`、`High`。|
|inferenceClassification | String | 根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。 |
|internetMessageId |String |由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。仅当 isDraft = true 时可以更新。|
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合| 为邮件定义的多值扩展属性的集合。只读。可为空。|
|replyTo|收件人集合|在答复时使用的电子邮件地址。仅当 isDraft = true 时可以更新。|
|sender|收件人|实际用于生成邮件的帐户。 从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件或将邮件作为[委托](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送时可更新。 在任何情况下，此值必须对应于使用的实际邮箱。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| 为邮件定义的单值扩展属性的集合。可为空。|
|subject|String|邮件的主题。仅当 isDraft = true 时可以更新。|
|toRecipients|收件人集合|邮件的收件人。 |

由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有 **邮件** 实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
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
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


