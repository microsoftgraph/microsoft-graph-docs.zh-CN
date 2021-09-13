---
title: referenceAttachment 资源类型
description: 到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。
ms.localizationpriority: medium
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: 3b82f7e166aa1ed681fb0a62a74c12df052f93be
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044284"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment 资源类型

命名空间：microsoft.graph

到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。

派生自 [附件](attachment.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |读取 referenceAttachment 对象的属性和关系。|
|[删除](../api/attachment-delete.md) | 无 |删除 referenceAttachment 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|附件的内容类型。|
|id|String|附件 ID。只读。|
|isInline|Boolean|如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|name|String|显示在用于表示嵌入附件的图标下方的文本。这不必是实际的文件名。|
|大小|Int32|存储在邮件附件中的元数据大小（以字节为单位）。 此值不表示实际文件的大小。|

## <a name="relationships"></a>关系
无



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.referenceAttachment"
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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

