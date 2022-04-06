---
title: educationMediaResource 资源类型
description: 表示 educationAssignment 的媒体文件资源。 继承自 educationResource
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2daa0b185ced9dd7400be6c54674f6e72a89dfe4
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684863"
---
# <a name="educationmediaresource-resource-type"></a>educationMediaResource 资源类型

命名空间：microsoft.graph

表示 [educationAssignment](educationassignment.md) 的媒体文件资源。 继承自 [educationResource](educationresource.md)。

将这些文件Upload到与分配或提交关联 **的文件Resource** 目录。

以下文件类型为媒体资源：`webm`、、`mkv`、`avi`、`wmv`、`mp4`、`m4v`、`mpg`、`mpeg``m2v`、`png``jpg``gif`、`bmp`、`jpeg``psd``heic``mp3`和。`m4a`

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|共享点文件夹上的文件的位置。 必需|
|createdBy|String|创建此资源的用户的显示名称。|
|createdDateTime|DateTimeOffset|添加重索的日期时间。|
|displayName|string|添加资源的用户的显示名称。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationMediaResource"
}-->

```json
{
  "fileUrl": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationMediaResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


