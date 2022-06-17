---
title: fileAttachment 资源类型
description: 文件 (，例如附加到事件、消息、任务或帖子的文本文件或 Word 文档) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 14ae2bb7ec5e341a144fa5c00eb131853ea6b679
ms.sourcegitcommit: 2132198551c7d1f37474debab471f612a3e35a08
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2022
ms.locfileid: "66141241"
---
# <a name="fileattachment-resource-type"></a>fileAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

文件 (，例如附加到用户[事件](../resources/event.md)、[消息](../resources/message.md)、[Outlook任务](../resources/outlooktask.md)或帖子的文本文件或 Word 文[档) ](../resources/post.md)。 

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
|isInline|Boolean|设置为 `true` 如果这是内联附件。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。|
|name|String|表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无。


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
  "size": "Int32"
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


