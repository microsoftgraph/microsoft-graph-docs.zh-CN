---
author: daspek
ms.author: dspektor
title: itemActivityTimeSet 资源类型
description: ItemActionSet 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4ef0b56471afe78b13edc2f6efb25941c9a749df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970656"
---
# <a name="itemactivitytimeset-resource-type"></a>itemActivityTimeSet 资源类型

**ItemActivityTimeSet**资源提供有关何时发生某个项目的[活动][ activity]的信息。

>**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称    | 类型           | 说明
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | 在观察到要发生活动时。
| recordedDateTime | DateTimeOffset | 在服务上记录观察时。

对于离线协作方案来说，**观察**和**记录**时间差异尤为重要。
如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。
稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
