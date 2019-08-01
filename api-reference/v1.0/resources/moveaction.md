---
author: daspek
ms.author: dspektor
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 8ef93cd83c8fd020af91a9ea8c9288c1d27d5cf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036069"
---
# <a name="moveaction-resource-type"></a>moveAction 资源类型

[**ItemActivity**][activity]上的**moveAction**资源是否存在指示活动已移动项目。

>**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| from          | string | 被移动项原来位置的名称。
| to            | string | 将项移动到的位置的名称。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
