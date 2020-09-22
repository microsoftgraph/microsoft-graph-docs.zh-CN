---
title: shiftPreferences 资源类型
description: 表示计划中用户的已分配班次的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d35f77e7d048adb0b0bb49604423bbe2ff53031c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058028"
---
# <a name="shiftpreferences-resource-type"></a>shiftPreferences 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [计划](schedule.md)中用户的已分配班次的可用性。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Get](../api/shiftpreferences-get.md) | [shiftPreferences](shiftpreferences.md) | 读取 **shiftPreferences** 对象的属性和关系。 |
| [更新](../api/shiftpreferences-put.md) | [shiftPreferences](shiftpreferences.md) | 更新 **shiftPreferences** 对象。 |

## <a name="properties"></a>属性

|属性          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id | `Edm.String` | 实体的标识符。 |
| @odata.etag | `Edm.String` | 实体的更改键。 |
| availability | [shiftAvailability](shiftavailability.md) 集合 | 用户计划的工作及其定期模式的可用性。 |
| createdDateTime | `Edm.DateTimeOffset` | 创建实体时对应的时间戳。 |
| lastModifiedDateTime | `Edm.DateTimeOffset` | 上次修改实体时对应的时间戳。 |
| lastModifiedBy | [identitySet](identityset.md) | 上次修改实体的人员的标识。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "availability": [{"@odata.type": "microsoft.graph.shiftAvailability"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


