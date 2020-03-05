---
author: daspek
description: ItemActionStat 资源提供有关一段时间内的操作的聚合详细信息。
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6ab31d8a155e0b9fd54b3f2185e7d05969291ec1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523126"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemActionStat**资源提供有关一段时间内的操作的聚合详细信息。

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

## <a name="properties"></a>属性

| 属性    | 类型  | 说明
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | 操作发生次数。 只读。
| actorCount  | Int32 | 执行此操作的不同参与者的数量。 只读。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->
