---
author: daspek
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项目的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 160afbc51196c60473dc40bec7b79daab6dc39eb3f302c1a1b9689c9c25929fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189462"
---
# <a name="moveaction-resource-type"></a>moveAction 资源类型

命名空间：microsoft.graph

[**itemActivity**][activity]上 **存在 moveAction** 资源指示活动移动了项目。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

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
  "@type&quot;: &quot;microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to&quot;: &quot;string"
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

