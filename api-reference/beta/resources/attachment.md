---
title: attachment 资源类型
description: 您可以向事件中添加相关内容,
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535555"
---
# <a name="attachment-resource-type"></a>attachment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以将相关内容添加到[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或以附件形式[发布](../resources/post.md)。

**附件**是以下附件派生类型的基础资源：

* 文件（[fileAttachment](../resources/fileattachment.md) 资源）
* 项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）
* 文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）

## <a name="methods"></a>方法

以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取附件](../api/attachment-get.md) | [attachment](attachment.md) |读取附加到事件、邮件、Outlook 任务或帖子的附件的属性和关系。|
|[Add attachment to an event](../api/event-post-attachments.md) | [attachment](attachment.md) |将文件、项目或链接附件添加到事件中。|
|[将附件添加到邮件中](../api/message-post-attachments.md) | [attachment](attachment.md) |将文件、项目或将附件链接添加到邮件中。|
|[将附件添加到 Outlook 任务](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |将文件、项目或链接附件添加到 Outlook 任务中。|
|[将附件添加到帖子中](../api/post-post-attachments.md) | [附件](attachment.md) |将文件、项目或将附件链接添加到帖子中。|
|[列出事件的附件](../api/event-list-attachments.md) | [附件](attachment.md)集合 | 获取事件的附件列表。 |
|[列出邮件的附件](../api/message-list-attachments.md) | [附件](attachment.md)集合 | 获取邮件的附件列表。 |
|[列出 Outlook 任务的附件](../api/outlooktask-list-attachments.md) | [附件](attachment.md)集合 | 获取 Outlook 任务的附件列表。 |
|[列出帖子的附件](../api/post-list-attachments.md) | [附件](attachment.md) 集合 | 获取帖子的附件列表。 |
|[删除](../api/attachment-delete.md) | 无 |删除事件、邮件、Outlook 任务或帖子上的附件。 |

## <a name="properties"></a>属性

下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|MIME 类型。|
|id|String| 只读。|
|isInline|Boolean|如果附件是内嵌附件，则为 `true`；否则为 `false`。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|name|String|附件的显示名称。 这不必是实际的文件名。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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
