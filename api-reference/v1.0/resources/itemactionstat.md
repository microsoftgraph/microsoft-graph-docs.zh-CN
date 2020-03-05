---
author: daspek
ms.author: dspektor
title: itemActionStat 资源类型
description: ItemActionStat 对象提供有关一段时间内的操作的聚合详细信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4207c85185281ec9944aa08dfce088739116bb8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447680"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat 资源类型

命名空间： microsoft. graph

**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。

## <a name="properties"></a>属性

| 属性    | 类型  | 说明
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | 操作发生次数。 只读。
| actorCount  | Int32 | 执行此操作的不同参与者的数量。 只读。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->
