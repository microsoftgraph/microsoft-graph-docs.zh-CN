---
title: 有提及资源类型
description: 代表到个人基于此人的电子邮件地址的通知。
author: simonhult
ms.openlocfilehash: a9c00daed067ecd41f0f687687ac9bf7f86d6f2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334227"
---
# <a name="mention-resource-type"></a>有提及资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表到个人基于此人的电子邮件地址的通知。 此类通知也称为是 @ 提及。

[消息](../resources/message.md)资源支持**提及**。 它包括**mentionsPreview**属性指示是否已登录的用户提及该消息实例中。 它还包括支持的某个提及，或删除某个提及该实例中的获取详细信息的**提到**导航属性。

应用程序时创建一条消息，可以在同一个创建某个提及`POST`通过包括提及的**提到**属性中的请求。 使用`GET`请求`$filter`查询参数，应用程序可返回所有邮件提及用户的登录用户邮箱中。 A`GET`请求`$expand`参数允许展开特定的邮件中的所有提及的应用程序的查询。

此机制的应用程序时让应用程序设置和获取提及在消息中的允许轻型通知，其中进行提及的用户，可以保持 （如撰写邮件正文） 的现有上下文中设置基础**提及**属性. 提到人员可以轻松地找到如果和通过其中提到这些`GET`请求与`$filter`或`$expand`查询参数。  

例如，在 Outlook 邮件客户端，当用户键入时`@`Outlook 时写入一条消息，允许用户选择或输入要完成 @ 提及的名称。 创建和发送的邮件或事件之前，outlook 将**提到**属性设置。 Outlook 还使用`GET`操作`$filter`和`$expand`，使已登录的用户可以查找提及用户的消息，警报用户对拟办事项或讨论，从而实现更快地响应。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|application | 字符串 | 在其中创建提及的应用程序的名称。 可选。 不使用和默认设置为 null 的**消息**。 |
|clientReference | 字符串 | 表示父资源实例的唯一标识符。 可选。 不使用和默认设置为 null 的**消息**。 |
|createdBy  | [emailAddress](../resources/emailaddress.md) | 进行提及的用户的电子邮件信息。 |
|createdDateTime  |DateTimeOffset |日期和时间在客户端上创建提及的。 |
|deepLink | 字符串 | 深入 web 链接到的资源实例中提及的上下文。 可选。 不使用和默认设置为 null 的**消息**。 |
|id | 字符串| 资源实例中提及的唯一标识符。|
|提到 | [emailAddress](../resources/emailaddress.md) | 被提及人员的电子邮件的信息。 必需。 |
|mentionText | 字符串 | 可选。 不使用和默认设置为 null 的**消息**。 获取提及中一条消息，请参阅改为邮件的**bodyPreview**属性。 |
|serverCreatedDateTime | DateTimeOffset | 日期和时间是在服务器上创建提及的。 可选。 不使用和默认设置为 null 的**消息**。 |

## <a name="relationships"></a>Relationships
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Post](../api/user-sendmail.md#request-2)和发送 | 无 | 创建和发送提及作为新邮件的一部分。|
|以新草稿的[文章](../api/user-post-messages.md#request-2) | 包含一个或多个**提及**对象的[消息](../resources/message.md)。 | 创建一个新的邮件草稿并包括一个或多个**提及**的对象。|
|[获取](../api/user-list-messages.md#request-2)邮件提及我 | [邮件](../resources/message.md)集合 | 获取包含**提及**的此用户的登录用户邮箱中的所有邮件。|
|一条消息的[获取](../api/message-get.md#request-2)和其提及 | [邮件](../resources/message.md)集合 | 收到一条消息，并展开的每个**提及**消息中的详细信息。|
|[删除](../api/message-delete.md#request-2)某个提及 | 无 |删除中指定的消息已登录的用户邮箱中提及的指定。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->