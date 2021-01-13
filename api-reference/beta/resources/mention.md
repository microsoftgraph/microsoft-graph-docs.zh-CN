---
title: 提及资源类型
description: 表示根据用户的电子邮件地址向用户发送的通知。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 23d4ac1d98a65e206a476768569cca89fb295a61
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844856"
---
# <a name="mention-resource-type"></a>提及资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示根据用户的电子邮件地址向用户发送的通知。 此类型的通知也称为 @-mentions。

邮件 [资源](../resources/message.md) 支持 **提及**。 它包括 **一个 mentionsPreview** 属性，该属性指示是否已在邮件实例中提及登录用户。 它还包括 **提及** 导航属性，该属性支持获取提及的详细信息，或删除该实例中的提及。

创建邮件时，应用可以通过将提及包括在提及属性中，在同一请求中 `POST` 创建 **提及** 。 通过使用查询参数的请求，应用可以返回已登录用户邮箱中提及该用户 `GET` `$filter` 的所有邮件。 通过 `GET` 查询参数 `$expand` 的请求，应用可以展开特定邮件中提及的所有内容。

这种允许应用在邮件中设置和提及的机制可启用轻型通知，其中进行提及的用户可以保留在现有上下文中 (例如，在应用设置基础提及属性时) 撰写邮件正文。  被提及人员可以轻松找出是否通过请求或查询参数提及 `GET` `$filter` 他们以及在何处 `$expand` 提及他们。  

例如，在 Outlook 邮件客户端中，当用户在编写邮件时进行输入时，Outlook 允许用户选择或输入名称以 `@` 完成 @-mention。 Outlook 在 **创建和** 发送邮件或事件之前设置 mentions 属性。 Outlook 还使用与登录用户一起的操作，并允许登录用户查找提及用户的邮件，以提醒用户操作项目或讨论，从而加快 `GET` `$filter` `$expand` 响应速度。


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
|application | String | 创建提及项的应用程序的名称。 可选。 不用于邮件，并且默认为 **null。** |
|clientReference | String | 表示资源实例的父级的唯一标识符。 可选。 不用于邮件，并且默认为 **null。** |
|createdBy  | [emailAddress](../resources/emailaddress.md) | 进行提及的用户的电子邮件信息。 |
|createdDateTime  |DateTimeOffset |在客户端上创建提及的日期和时间。 |
|deepLink | String | 指向资源实例中提及内容上下文的深层 Web 链接。 可选。 不用于邮件，并且默认为 **null。** |
|id | String| 资源实例中提及的唯一标识符。|
|提及 | [emailAddress](../resources/emailaddress.md) | 被提及人员的电子邮件信息。 必需。 |
|mentionText | String | 可选。 不用于邮件，并且默认为 **null。** 若要获取邮件中的提及，请参阅邮件的 **bodyPreview** 属性。 |
|serverCreatedDateTime | DateTimeOffset | 在服务器上创建提及的日期和时间。 可选。 不用于邮件，并且默认为 **null。** |

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[发布](../api/user-sendmail.md#request-2) 和发送 | 无 | 创建新邮件的一部分并发送提及。|
|[张贴](../api/user-post-messages.md#request-2) 到新草稿 | [包含](../resources/message.md) 一个或多个 **提及对象** 的邮件。 | 创建新邮件的草稿，并包括一个或多个 **提及** 对象。|
|[获取](../api/user-list-messages.md#request-2) 提及我的消息 | [message](../resources/message.md) 集合 | 获取已登录用户的邮箱中包含此用户提及的所有邮件。 |
|[获取](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) 邮件及其提及内容 | [message](../resources/message.md) 集合 | 获取邮件并展开邮件中每个 **提及** 的详细信息。|
|[删除](../api/message-delete.md#request-2) 提及 | 无 |删除登录用户邮箱中指定邮件中指定的提及内容。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


