---
author: daspek
ms.author: dspektor
title: renameAction 资源类型
description: RenameAction 对象提供有关重命名项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 693c5d8586a7ceef2c30f1e6dae17ac47d8e2d1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967315"
---
# <a name="renameaction-resource-type"></a>renameAction 资源类型

命名空间：microsoft.graph

[**ItemActivity**][activity]上的**renameAction**资源是否存在指示活动重命名了项目。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | 项的原名称。
| newName       | 字符串 | 项的新名称。

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

