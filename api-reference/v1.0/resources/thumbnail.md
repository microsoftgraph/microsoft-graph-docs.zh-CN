---
author: JeremyKelley
ms.date: 09/10/2017
title: 缩略图
localization_priority: Normal
description: 缩略图资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 76d71cc8cbebc987eea6bbf057945dc41b55f0ee
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239266"
---
# <a name="thumbnail-resource-type"></a>Thumbnail 资源类型

命名空间：microsoft.graph

**缩略图** 资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。

## <a name="json-representation"></a>JSON 表示形式

下面是 **缩略图** 资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a>属性

| 属性     | 类型   | 说明
| :----------- | :----- | :----------------------------------------------------
| height       | Int32  | 缩略图高度，以像素为单位。
| sourceItemId | 字符串 | 提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。
| url          | String | 用于提取缩略图内容的 URL。
| width        | Int32  | 缩略图宽度，以像素为单位。
| content      | 流 | 缩略图的内容流。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->

