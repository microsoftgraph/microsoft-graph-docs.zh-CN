---
author: JeremyKelley
description: 已删除资源指示该项已被删除。
ms.date: 09/10/2017
title: Deleted
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: c62d3a6e0636b2e39875bef17dabe2b92cad806a
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900035"
---
# <a name="deleted-facet"></a>Deleted Facet

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**已删除的** 资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。

有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a>属性

| 属性 | 类型   | 说明                               |
|:---------|:-------|:------------------------------------------|
| state    | String | 表示已删除的项的状态。 |

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": []
}
-->


