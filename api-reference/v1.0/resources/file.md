---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
ms.openlocfilehash: 2201533457863c3cac6b7a9463f80e37bd5a569a
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267463"
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
| hashes   | [Hashes](hashes.md) | 文件二进制内容的哈希值（如果可用）。只读。                                                                                    |
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
