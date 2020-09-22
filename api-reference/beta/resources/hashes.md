---
author: JeremyKelley
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.date: 09/10/2017
title: 哈希
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: df3629be679b714805ea6618b7aa963214f32793
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013606"
---
# <a name="hashes-resource-type"></a>哈希资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将可用哈希分组到一个项的单个结构中。

> [!NOTE]
> 并非所有服务都为列出的所有哈希属性提供值。 在 OneDrive for Business 和 SharePoint Server 2016 中， **sha1Hash**、 **crc32Hash**和 **sha256Hash** 不可用。 在 OneDrive 个人版中，**quickXorHash** 不可用。

## <a name="properties"></a>属性

| 属性         | 类型   | 说明                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | 文件内容的 SHA1 哈希（如果可用）。只读。 |
| **sha256Hash**   | String | 如果可用) ，则为文件的内容 (SHA256 哈希。 只读。 |
| **crc32Hash**    | String | 文件的 CRC32 值（如果可用）。只读。            |
| **quickXorHash** | String | 文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。 |

> **注意：** 在哈希值不可用的情况下，项目的哈希值将在项目下载后进行更新。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="see-also"></a>另请参阅

- 有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。
- 若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->


