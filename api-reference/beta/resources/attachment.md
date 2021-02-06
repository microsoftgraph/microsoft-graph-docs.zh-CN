---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: d1296c40bfc434262f1911c6f9453725bc033999
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137618"
---
# <a name="attachment-resource-type"></a>attachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

可以将相关内容以附件的形式添加到用户[](../resources/event.md)事件、[邮件](../resources/message.md)[、Outlook](../resources/outlooktask.md)任务或组[](../resources/post.md)帖子中。 

组日历中的事件不支持附件。

Outlook 任务不支持引用附件。

**附件** 是以下附件派生类型的基础资源：

* 文件（[fileAttachment](../resources/fileattachment.md) 资源）
* 项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）
* 文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）

>**注意**：可添加到的文件或项目附件的大小限制为 4 MB 以下。 
>
> 但是，如果要将介于 3MB 到 150MB 之间的文件附加到邮件，可以创建上载会话并反复[](../api/attachment-createuploadsession.md)上载文件范围以附加它。 有关 [示例，请参阅将大文件附加到 Outlook](/graph/outlook-large-attachments) 邮件。

## <a name="methods"></a>方法

以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取附件](../api/attachment-get.md) | [attachment](attachment.md) |读取附加到用户事件、邮件、Outlook 任务或帖子的附件的属性、关系或原始内容。|
|[将附件添加到用户事件中](../api/event-post-attachments.md) | [附件](attachment.md) |将文件、项目或链接附件添加到用户日历中的事件中。|
|[将附件添加到邮件中](../api/message-post-attachments.md) | [附件](attachment.md) |将文件、项目或将附件链接添加到邮件中。 此操作将可添加到的附件大小限制在 4 MB 以下。|
|[创建会话以附加大文件](../api/attachment-createuploadsession.md)| [uploadSession](uploadsession.md) | 创建允许应用迭代上载文件范围的上载会话，以便将文件附加到指定的 **消息**。 文件大小必须介于 3MB 和 150MB 之间。|
|[将附件添加到已弃](../api/outlooktask-post-attachments.md) (Outlook 任务)  | [附件](attachment.md) |将文件或项目附件添加到 Outlook 任务。|
|[将附件添加到帖子中](../api/post-post-attachments.md) | [附件](attachment.md) |向组帖子添加文件、项目或链接附件。|
|[列出用户事件的附件](../api/event-list-attachments.md) | [附件](attachment.md)集合 | 获取用户日历中事件的附件列表。 |
|[列出邮件的附件](../api/message-list-attachments.md) | [附件](attachment.md) 集合 | 获取邮件的附件列表。 |
|[列出已弃](../api/outlooktask-list-attachments.md) (Outlook 任务)  | [附件](attachment.md) 集合 | 获取 Outlook 任务的附件列表。 |
|[列出帖子的附件](../api/post-list-attachments.md) | [附件](attachment.md) 集合 | 获取帖子的附件列表。 |
|[删除](../api/attachment-delete.md) | 无 |删除事件、邮件、Outlook 任务或帖子上的附件。 |

## <a name="properties"></a>属性

下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|MIME 类型。|
|id|字符串| 只读。|
|isInline|Boolean|如果附件是内嵌附件，则为 `true`；否则为 `false`。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|名称|String|附件的显示名称。 这不必是实际的文件名。|
|大小|Int32|附件大小，以字节为单位。|

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
  "suppressions": []
}
-->


