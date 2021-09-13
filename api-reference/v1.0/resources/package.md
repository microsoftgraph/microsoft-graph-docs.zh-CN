---
author: JeremyKelley
ms.date: 09/10/2017
title: 程序包
ms.localizationpriority: medium
description: " 或应视为集合而不是单个项目的项目集合。"
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cf4a0ec97c328bb10aa51800c7ec18b4a8512286
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094119"
---
# <a name="package-resource-type"></a>包资源类型

命名空间：microsoft.graph

**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。

包的一个示例是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有 **包** facet，以向客户端指示这是应被特殊处理的数据集。

具有 **包** facet 的 DriveItems 不包括 **文件夹** 或 **文件** facet，但在概念上与具有 **文件夹** facet 的项类似。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a>属性

| 属性名 | 类型   | 说明                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 类型          | string | 一个指示程序包类型的字符串。 虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。 |

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

