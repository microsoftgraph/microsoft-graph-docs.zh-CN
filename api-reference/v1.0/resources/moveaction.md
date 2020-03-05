---
author: daspek
ms.author: dspektor
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 04c9ddad00b5705d84af6e72ac194a0d32fd015c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447379"
---
# <a name="moveaction-resource-type"></a>moveAction 资源类型

命名空间： microsoft. graph

[**ItemActivity**][activity]上的**moveAction**资源是否存在指示活动已移动项目。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

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
