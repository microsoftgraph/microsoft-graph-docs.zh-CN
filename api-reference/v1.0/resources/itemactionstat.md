---
author: daspek
title: itemActionStat 资源类型
description: itemActionStat 对象提供有关一段时间的操作的聚合详细信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 595a479f98e6327f3e43c2278c646d6e570e5a290cdcae8b7151ac4162d15578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246673"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat 资源类型

命名空间：microsoft.graph

**itemActionStat** 资源提供有关一段时间的操作的聚合详细信息。

## <a name="properties"></a>属性

| 属性    | 类型  | 说明
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | 操作发生次数。 只读。
| actorCount  | Int32 | 执行该操作的不同操作者的数量。 只读。

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

