---
title: fileAttachment 资源类型
description: 附加到事件，文件 （如文本文件或 Word 文档中）
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045671"
---
# <a name="fileattachment-resource-type"></a>fileAttachment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)（如文本文件或 Word 文档） 的文件。 **ContentBytes**属性将包含 base64 编码的文件的内容。  

创建文件附件时，在请求正文中包括以下内容：

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* 必要属性**名称**和 **contentBytes**。

派生自 [附件](attachment.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |读取 fileattachment 对象的属性和关系。|
|[删除](../api/attachment-delete.md) | 无 |删除 fileAttachment 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentBytes|Binary|文件的 Base64 编码内容。|
|contentId|String|获取 Exchange 存储中的附件 ID。|
|contentLocation|String|对应于附件内容所在位置的统一资源标识符 (URI)。|
|contentType|String|附件的内容类型。|
|id|String|附件 ID。|
|isInline|布尔|如果是内嵌附件则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。|
|name|String|表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
