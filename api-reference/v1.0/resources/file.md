---
author: JeremyKelley
ms.date: 09/10/2017
title: 文件资源 thype
localization_priority: Normal
description: 文件资源将与文件相关的数据项分组到一个单一结构。
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0b8fc90a54dcb4a052994b4848aeb297b914d9ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018408"
---
# <a name="file-resource-type"></a>File 资源类型

命名空间：microsoft.graph

**文件**资源将与文件相关的数据项分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有非 null **文件** facet，则该项目表示一个文件。
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

