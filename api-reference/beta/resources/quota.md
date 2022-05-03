---
author: JeremyKelley
description: 配额资源提供有关驱动器资源的空间约束的详细信息。
ms.date: 09/10/2017
title: 配额
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: fb27c29c70c0775ad59bf23c33348aaf490ebaed
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176736"
---
# <a name="quota-resource-type"></a>配额资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**配额** 资源提供有关 [驱动器](drive.md)资源的空间约束的详细信息。

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

| 属性               | 类型                                                | Description                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------- |
| total                  | Int64                                               | 允许的总存储空间，以字节为单位。只读。                             |
| used                   | Int64                                               | 已使用的总空间，以字节为单位。只读。                                        |
| remaining              | Int64                                               | 达到配额限制之前剩余的总空间，以字节为单位。只读。   |
| deleted                | Int64                                               | 回收站中的文件占用的总空间，以字节为单位。只读。        |
| state                  | string                                              | 指示存储空间状态的枚举值。只读。   |
| storagePlanInformation | [storagePlanInformation](storageplaninformation.md) | 有关驱动器的存储配额计划的信息。 仅在个人OneDrive中。 |

### <a name="state-enumeration-values"></a>状态枚举值

| 值      | Description                                                                                                                                                                 |
| :--------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
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
