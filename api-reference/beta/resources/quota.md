---
author: JeremyKelley
description: 配额资源提供有关驱动器资源上的空间限制的详细信息。
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9477662c1ffa8419d7be293c31b8f50b06bd74d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993052"
---
# <a name="quota-resource-type"></a>配额资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**配额**资源提供有关[驱动器](drive.md)资源上的空间限制的详细信息。

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
| total         | Int64  | 允许的总存储空间，以字节为单位。只读。                           |
| used          | Int64  | 已使用的总空间，以字节为单位。只读。                                      |
| remaining     | Int64  | 达到配额限制之前剩余的总空间，以字节为单位。只读。 |
| deleted       | Int64  | 回收站中的文件占用的总空间，以字节为单位。只读。      |
| state         | string | 指示存储空间状态的枚举值。只读。 |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | 有关驱动器的存储配额计划的信息。 仅在个人 OneDrive 中。|

### <a name="state-enumeration-values"></a>状态枚举值

| 值      | 说明                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | 驱动器具有充足的剩余配额。                                                                                                                               |
| `nearing`  | 剩余配额少于总配额空间的 10%。                                                                                                                      |
| `critical` | 剩余配额少于总配额空间的 1%。                                                                                                                       |
| `exceeded` | 使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。 |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->


