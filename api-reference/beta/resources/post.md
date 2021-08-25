---
title: 帖子资源类型
description: 表示 conversationThread 实体中的单个帖子项。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f68b773417393c10630b0e24e6325f5080c99f6e
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514593"
---
# <a name="post-resource-type"></a>帖子资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [conversationThread](conversationthread.md) 实体中的单个帖子项。

即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：

* [答复现有帖子](../api/post-reply.md) 
* [答复现有线程](../api/conversationthread-reply.md) 
* [在新对话中创建线程](../api/group-post-threads.md)
* [创建新对话](../api/group-post-conversations.md)

使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出帖子](../api/conversationthread-list-posts.md) | [帖子](post.md) |获取指定线程的帖子。 |
|[获取帖子](../api/post-get.md) | [帖子](post.md) |获取指定的线程中帖子的属性和关系。|
|[答复](../api/post-reply.md)|无|在组对话中答复帖子，并向指定线程中添加新帖子。|
|[转发](../api/post-forward.md)|无|将帖子转发给收件人。|
|**附件**| | |
|[列出附件](../api/post-list-attachments.md) |[attachment](attachment.md) 集合| 获取帖子的所有附件。|
|[Add attachment](../api/post-post-attachments.md) |[attachment](attachment.md)| 将附件添加到帖子中。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[帖子](post.md)  |在新建或现有帖子中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的帖子](../api/singlevaluelegacyextendedproperty-get.md)  | [帖子](post.md) | 通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [帖子](post.md) | 在新建或现有的帖子中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的帖子](../api/multivaluelegacyextendedproperty-get.md)  | [帖子](post.md) | 使用 `$expand` 获取包含一个多值扩展属性的帖子。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|帖子的内容。这是默认属性。此属性可为 NULL。|
|categories|String collection|与帖子关联的类别。 每个类别对应于为用户定义的 [outlookCategory](outlookcategory.md)的 **displayName** 属性。|
|changeKey|String|标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|conversationId|String|对话的唯一 ID。只读。|
|conversationThreadId|字符串|对话线程的唯一 ID。只读。|
|createdDateTime|DateTimeOffset|创建帖子时指定。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|发件人|[recipient](recipient.md)|在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。|
|hasAttachments|Boolean|指示帖子是否具有至少一个附件。这是默认属性。|
|id|String| 只读。|
|importance | importance| 组帖子的重要性 `low` `normal` ：、、。 `high` |
|lastModifiedDateTime|DateTimeOffset|帖子上次修改时指定。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|newParticipants|[recipient](recipient.md) collection|添加到此线程作为帖子一部分的对话参与者。|
|receivedDateTime|DateTimeOffset|接收到帖子时指定。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|sender|[recipient](recipient.md)|包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合|文章的[fileAttachment、itemAttachment](fileattachment.md)和[referenceAttachment](referenceattachment.md)附件的集合。 [](itemattachment.md) 只读。 可为 NULL。 支持 `$expand`。|
|extensions|[扩展](extension.md)集合|为帖子定义的开放扩展集合。 只读。 可为 NULL。 支持 `$expand`。|
|inReplyTo|[Post](post.md)|此文章在 [conversationThread](conversationthread.md)中回复的上一个帖子。 只读。 支持 `$expand`。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为帖子定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为帖子定义的单值扩展属性的集合。只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


