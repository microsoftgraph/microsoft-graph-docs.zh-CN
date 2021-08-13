---
author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Hashes 资源类型
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd04ff57aff3d276655a173d123f228520a77b7d548afb9f8d75d30fd6ba4e6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243551"
---
# <a name="hashes-resource-type"></a>Hashes 资源类型

命名空间：microsoft.graph

**哈希** 资源将可用哈希分组到项的单个结构中。

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
| **sha1Hash**     | String | 文件内容的 SHA1 哈希（如果可用）。只读。 |
| **sha256Hash**   | String | 文件内容的 SHA256 哈希 (（如果) ）。 只读。 |
| **crc32Hash**    | String | 文件的 CRC32 值以小尾数表示， (可用) 。 只读。            |
| **quickXorHash** | String | 文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。 |

**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。

## <a name="remarks"></a>注解

在 OneDrive for Business 和 SharePoint Server 2016 中 **，sha1Hash** 和 **crc32Hash** 和 **sha256Hash** 不可用。

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

