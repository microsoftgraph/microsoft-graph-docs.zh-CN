---
author: daspek
description: itemActionStat 资源提供有关一段时间内操作的聚合详细信息。
ms.date: 09/14/2017
title: ItemActionStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: b1fb726904c3b97ead34162410025a82f410231d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176297"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemActionStat** 资源提供有关一段时间内操作的聚合详细信息。

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

| 属性    | 类型  | Description
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | 执行操作的次数。 只读。
| actorCount  | Int32 | 执行该操作的非重复执行组件的数目。 只读。

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


