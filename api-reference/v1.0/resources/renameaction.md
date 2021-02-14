---
author: daspek
title: renameAction 资源类型
description: renameAction 对象提供有关重命名项目的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 35e0aa9929b8e152265a5540625f5981a587edb7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238650"
---
# <a name="renameaction-resource-type"></a>renameAction 资源类型

命名空间：microsoft.graph

itemActivity 上 **存在 renameAction** [][activity]资源表示活动重命名了项目。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | 项的原名称。
| newName       | string | 项目的新名称。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->

