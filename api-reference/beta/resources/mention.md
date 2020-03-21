---
title: 提及资源类型
description: 表示基于人员的电子邮件地址的人员通知。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 70005abbe8eaf0e9680f106f59caf091aa2495d2
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892581"
---
# <a name="mention-resource-type"></a>提及资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示基于人员的电子邮件地址的人员通知。 这种类型的通知也称为 @ 提到。

[邮件](../resources/message.md)资源支持**提到**。 它包含一个**mentionsPreview**属性，该属性指示该邮件实例中是否提到已登录用户。 它还包括**提及**导航属性，该属性支持获取提及的详细信息，或删除该实例中的提及。

创建邮件时，应用程序可以通过在**提及**属性中添加提及`POST`的内容，在同一请求中创建记录。 使用`$filter`查询`GET`参数的请求，应用程序可以返回登录用户的邮箱中提及用户的所有邮件。 使用`GET` `$expand`查询参数的请求可让应用展开特定邮件中的所有提及。

允许在邮件中使用应用程序集和获取提及的机制启用轻量通知，其中提出提及的用户可以保留在现有上下文中（例如，撰写邮件正文），而应用会设置基础**提及**属性。 提到的`GET` `$filter`人员可以通过或`$expand`查询参数轻松了解是否以及在请求中提及的情况。  

例如，在 Outlook 邮件客户端中，当用户在撰写`@`邮件时键入时，Outlook 允许用户选择或输入名称来完成 @-提及。 Outlook 在创建和发送邮件或事件之前设置**提及**属性。 Outlook 还使用`GET`与`$filter`和`$expand`的操作，以让登录用户查找提及用户的邮件，提醒用户执行操作项目或讨论，这样可以更快地响应。


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
|application | String | 在其中创建提及的应用程序的名称。 可选。 不会对**邮件**使用和默认为 null。 |
|clientReference | String | 代表资源实例的父项的唯一标识符。 可选。 不会对**邮件**使用和默认为 null。 |
|createdBy  | [emailAddress](../resources/emailaddress.md) | 提出提及的用户的电子邮件信息。 |
|createdDateTime  |DateTimeOffset |在客户端上创建提及的日期和时间。 |
|deepLink | String | 指向资源实例中提及的上下文的深层 web 链接。 可选。 不会对**邮件**使用和默认为 null。 |
|id | String| 资源实例中提及的唯一标识符。|
|所 | [emailAddress](../resources/emailaddress.md) | 提到的人员的电子邮件信息。 必需。 |
|mentionText | String | 可选。 不会对**邮件**使用和默认为 null。 若要获取邮件中提及的内容，请改为查看邮件的**bodyPreview**属性。 |
|serverCreatedDateTime | DateTimeOffset | 在服务器上创建提及的日期和时间。 可选。 不会对**邮件**使用和默认为 null。 |

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Post](../api/user-sendmail.md#request-2)和 send | 无 | 创建并将提及作为新邮件的一部分发送。|
|[发布](../api/user-post-messages.md#request-2)到新草稿 | 包含一个或多个**提及**对象的[邮件](../resources/message.md)。 | 创建新邮件的草稿并包含一个或多个**提及**的对象。|
|[获取](../api/user-list-messages.md#request-2)涉及我的邮件 | [邮件](../resources/message.md)集合 | 获取已登录用户邮箱中的所有邮件，其中包含此用户的**提及**。|
|[获取](../api/message-get.md#example-2)邮件及其提及内容 | [邮件](../resources/message.md)集合 | 获取邮件并展开邮件中每个**提及**的详细信息。|
|[删除](../api/message-delete.md#request-2)提及 | 无 |在已登录用户的邮箱中删除指定邮件中指定的提及项。 |

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
