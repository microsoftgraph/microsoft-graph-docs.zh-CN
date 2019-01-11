---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
localization_priority: Normal
ms.openlocfilehash: 8a247987447dcd97ac0f42a6a4e743a0c80f6bd5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862305"
---
# <a name="file-resource-type"></a>File 资源类型

**文件**资源将与文件相关的数据项分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有一个非 null **文件**方面，则该项表示一个文件。除了其他属性，文件还具有**内容**关系，其中包含文件字节流。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a>属性

| 属性 | 类型                    | 说明                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| 哈希   | [哈希](hashes.md) | 文件二进制内容的哈希值（如果可用）。只读。                                                                                    |
| mimeType | string                  | 文件的 MIME 类型。这由服务器上的逻辑决定，不能是在上载文件时提供的值。只读。 |

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
