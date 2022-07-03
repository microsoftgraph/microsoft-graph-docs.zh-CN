---
author: JeremyKelley
title: package
ms.localizationpriority: medium
description: 指示 driveItem 是包或项目集合中的顶级项，应将其视为集合而不是单个项。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 5188ae56a1e5527f76a581544a8968579d1a423e
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609610"
---
# <a name="package-resource-type"></a>包资源类型

命名空间：microsoft.graph

**包** 资源指示 **driveItem** 是“包”或应视为集合而不是单个项的项集合中的顶级项。

包的一个示例是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有 **包** facet，以向客户端指示这是应被特殊处理的数据集。

**具有包** 方面化的 **driveItems** 不包括 **文件夹** 或 **文件** 方面，但在概念上类似于具有 **文件夹** 方面的项目。

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
| 类型          | string | 一个字符串，指示包的类型。 虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。 |

## <a name="remarks"></a>注解 

有关 DriveItem 上的分面的详细信息，请参阅 [driveItem](driveitem.md)。


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

