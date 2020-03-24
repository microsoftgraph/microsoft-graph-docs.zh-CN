---
title: fileAttachment 资源类型
description: 附加到事件的文件（如文本文件或 Word 文档）
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: e14b98c5ee3302d5b19bc7ad92187112b6d8c80b
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926797"
---
# <a name="fileattachment-resource-type"></a>fileAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

附加到用户[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[公告](../resources/post.md)的文件（如文本文件或 Word 文档）。 

创建文件附件时，在请求正文中包括以下内容：

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* 必要属性**名称**和 **contentBytes**。

派生自 [附件](attachment.md)。

> [!NOTE]
> 在将文件内容分配给**contentBytes**之前，请务必在 base64 中对文件内容进行编码。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |读取 fileAttachment 对象的属性、关系或原始内容。|
|[删除](../api/attachment-delete.md) | 无 |删除 fileAttachment 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|contentBytes|Edm.Binary|文件的 Base64 编码内容。|
|contentId|String|获取 Exchange 存储中的附件 ID。|
|contentLocation|String|请勿使用此属性，因为它不受支持。|
|contentType|String|附件的内容类型。|
|id|String|附件 ID。|
|isInline|Boolean|如果是内嵌附件则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。|
|name|String|表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
