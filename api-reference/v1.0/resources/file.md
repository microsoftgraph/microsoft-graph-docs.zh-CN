---
author: JeremyKelley
ms.date: 09/10/2017
title: File 资源类型
localization_priority: Normal
description: 文件资源将与文件相关的数据项分组到一个单一结构。
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 57266222e9cbc2778673172b3b96a40ca4d51df466a8c90ae784d170b7e25175
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146886"
---
# <a name="file-resource-type"></a>File 资源类型

命名空间：microsoft.graph

**文件** 资源将与文件相关的数据项分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有非 null **文件** Facet，则该项表示文件。
除了其他属性，文件还具有 **content** 关系，其中包含文件字节流。

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

