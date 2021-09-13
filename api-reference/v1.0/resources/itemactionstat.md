---
author: daspek
title: itemActionStat 资源类型
description: itemActionStat 对象提供有关一段时间的操作的聚合详细信息。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 047ffe54a613cafbe953a4ff72794382ab440b7e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104122"
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

