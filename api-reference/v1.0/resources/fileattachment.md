---
title: fileAttachment 资源类型
description: 事件、邮件或帖子中附加的文件（例如文本文件或 Word 文档）。
ms.localizationpriority: high
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ffd35829cfafac92b2cd6707e0d653325b37993e
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160621"
---
# <a name="fileattachment-resource-type"></a>fileAttachment 资源类型

命名空间：microsoft.graph

用户[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)中附加的文件（例如文本文件或 Word 文档）。 

创建文件附件时，在请求正文中包括以下内容：

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* 必要属性 **名称** 和 **contentBytes**。

派生自 [附件](attachment.md)。

> [!NOTE]
> 确保先使用 base64 为文件内容编码，然后再将其分配到 **contentBytes**。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |读取 **fileAttachment** 对象的属性、关系或原始内容。|
|[删除](../api/attachment-delete.md) | 无 |删除 **fileAttachment** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentBytes|Edm.Binary|文件的 Base64 编码内容。|
|contentId|String|获取 Exchange 存储中的附件 ID。|
|contentLocation|String|请勿使用此属性，因为它不受支持。|
|contentType|String|附件的内容类型。|
|id|String|附件 ID。|
|isInline|Boolean|如果是内嵌附件则设置为 `true`。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。|
|name|String|表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式

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
  "size": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

