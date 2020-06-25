---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
description: 配额资源提供有关 驱动器 资源上的空间限制的详细信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 293daf950beb5cdf3cbd791a1e8bf0d4b92a220b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864208"
---
# <a name="quota-resource-type"></a>Quota 资源类型

命名空间：microsoft.graph

**配额**资源提供有关 [驱动器](drive.md) 资源上的空间限制的详细信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | Total allowed storage space, in bytes. Read-only.                           |
| used          | Int64  | Total space used, in bytes. Read-only.                                      |
| remaining     | Int64  | Total space remaining before reaching the quota limit, in bytes. Read-only. |
| deleted       | Int64  | Total space consumed by files in the recycle bin, in bytes. Read-only.      |
| state         | string | Enumeration value that indicates the state of the storage space. Read-only. |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | 有关驱动器的存储配额计划的信息。 仅在个人 OneDrive 中。|

## <a name="state-enumeration"></a>状态枚举

| 值      | 说明                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | 驱动器具有充足的剩余配额。                                                                                                                               |
| `nearing`  | 剩余配额少于总配额空间的 10%。                                                                                                                      |
| `critical` | 剩余配额少于总配额空间的 1%。                                                                                                                       |
| `exceeded` | The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased. |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
