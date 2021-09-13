---
title: shiftPreferences 资源类型
description: 表示在日程安排中向用户分配班次的可用性。
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9bebb27005d18e6fa94673a449a47f8d40f23d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032158"
---
# <a name="shiftpreferences-resource-type"></a>shiftPreferences 资源类型

命名空间：microsoft.graph

表示在日程安排中分配班次的用户 [的可用性](schedule.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Get](../api/shiftpreferences-get.md) | [shiftPreferences](shiftpreferences.md) | 读取 **shiftPreferences 对象的属性和** 关系。 |
| [更新](../api/shiftpreferences-put.md) | [shiftPreferences](shiftpreferences.md) | 更新 **shiftPreferences** 对象。 |

## <a name="properties"></a>属性

|属性          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id | `Edm.String` | 实体的标识符。 |
| @odata.etag | `Edm.String` | 实体更改键。 |
| availability | [shiftAvailability](shiftavailability.md) 集合 | 计划工作的用户的可用性及其定期模式。 |
| createdDateTime | `Edm.DateTimeOffset` | 与实体创建时间相对应的时间戳。 |
| lastModifiedDateTime | `Edm.DateTimeOffset` | 与实体上次修改时间相对应的时间戳。 |
| lastModifiedBy | [identitySet](identityset.md) | 上次修改实体的人的标识。 |

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

