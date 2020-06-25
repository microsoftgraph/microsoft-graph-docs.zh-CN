---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Hashes 资源类型
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: da326576b148fdaee79ebfc3df2d7832bfeee4e5
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863738"
---
# <a name="hashes-resource-type"></a>Hashes 资源类型

命名空间：microsoft.graph

**哈希**资源将可用哈希分组到项的单个结构中。

**注意：** 并非所有服务均为列出的所有哈希属性提供值。

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

## <a name="properties"></a>属性

| 属性         | 类型   | 说明                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | SHA1 hash for the contents of the file (if available). Read-only. |
| **sha256Hash**   | String | 文件内容的 SHA256 哈希值（如果有）。 只读。 |
| **crc32Hash**    | String | 文件的 CRC32 值，以小字节序（如果可用）为单位。 只读。            |
| **quickXorHash** | String | A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only. |

**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.

## <a name="remarks"></a>注解

在 OneDrive for Business 和 SharePoint Server 2016 中， **sha1Hash**和**Crc32Hash**，并且**sha256Hash**不可用。

在 OneDrive 个人版中，**quickXorHash** 不可用。

若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。
有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
