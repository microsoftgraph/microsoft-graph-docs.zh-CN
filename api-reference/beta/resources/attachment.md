---
title: attachment 资源类型
description: 您可以将相关的内容添加到事件，
localization_priority: Normal
ms.openlocfilehash: 8f7a6f9392d376995a53d9a4c06083780b0437b9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573422"
---
# <a name="attachment-resource-type"></a>attachment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以将相关的内容添加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或附件的形式[发布](../resources/post.md)。

**附件**是以下附件派生类型的基础资源：

* 文件（[fileAttachment](../resources/fileattachment.md) 资源）
* 项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）
* 文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）

## <a name="methods"></a>方法

以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取附件](../api/attachment-get.md) | [attachment](attachment.md) |读取的属性和附件，附加到事件、 邮件、 Outlook 任务或公告的关系。|
|[Add attachment to an event](../api/event-post-attachments.md) | [附件](attachment.md) |将文件、项目或链接附件添加到事件中。|
|[将附件添加到邮件中](../api/message-post-attachments.md) | [附件](attachment.md) |将文件、项目或将附件链接添加到邮件中。|
|[将附件添加到 Outlook 任务](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |添加文件、 项或 Outlook 任务链接附件。|
|[将附件添加到帖子中](../api/post-post-attachments.md) | [附件](attachment.md) |将文件、项目或将附件链接添加到帖子中。|
|[列出事件的附件](../api/event-list-attachments.md) | [附件](attachment.md) 集合 | 获取事件的附件列表。 |
|[列出邮件的附件](../api/message-list-attachments.md) | [附件](attachment.md) 集合 | 获取邮件的附件列表。 |
|[Outlook 任务的列出附件](../api/outlooktask-list-attachments.md) | [附件](attachment.md)集合 | 获取附件 Outlook 任务的列表。 |
|[列出帖子的附件](../api/post-list-attachments.md) | [附件](attachment.md) 集合 | 获取帖子的附件列表。 |
|[删除](../api/attachment-delete.md) | 无 |删除事件、 邮件、 Outlook 任务或公告上的附件。 |

## <a name="properties"></a>属性

下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|MIME 类型。|
|id|String| 只读。|
|isInline|Boolean|如果附件是内嵌附件，则为 `true`；否则为 `false`。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|名称|String|附件的显示名称。 这不需要是实际的文件名称。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
