---
author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
description: ThumbnailSet 资源是键控的 缩略图 资源集合。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aa38f89fbfe5738a37842439965690f5ce8aa86c122685d37a991e2797c2ca48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221171"
---
# <a name="thumbnailset-resource-type"></a>ThumbnailSet 资源类型

命名空间：microsoft.graph

**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a>属性

| 属性 | 类型                      | 说明                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| id       | String                    | 项目中的 id。只读。                                                |
| 大    | [缩略图](thumbnail.md) | 1920 x 1920 缩放后的缩略图。                                                     |
| 中等   | [缩略图](thumbnail.md) | 176x176 缩放后的缩略图。                                                       |
| 小    | [缩略图](thumbnail.md) | 48x48 裁剪缩略图。                                                        |
| 源   | [缩略图](thumbnail.md) | 用来生成其他缩略图的自定义缩略图图像或原始图像。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->

