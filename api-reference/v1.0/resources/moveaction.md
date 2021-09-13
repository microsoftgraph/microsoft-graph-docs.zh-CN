---
author: daspek
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项目的活动的信息。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 953c932d83060ed650b0e3ad096cf1de40941e1c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067057"
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

