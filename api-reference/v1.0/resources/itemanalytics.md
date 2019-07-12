---
author: daspek
ms.author: dspektor
title: itemAnalytics 资源类型
description: ItemAnalytics 对象提供有关项目上发生的活动的分析。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a18d12bd2b431d147f2d23ea2c958cd75078c9a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620414"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics 资源类型

**ItemAnalytics**资源提供有关项目上发生的活动的分析。 此资源目前仅适用于 SharePoint 和 OneDrive for business。

您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。

>**注意:****ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。

## <a name="properties"></a>属性

| 属性      | 类型                 | 说明
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | 对项目生命周期的分析。
| lastSevenDays | [itemActivityStat][] | 最近七天的分析。

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```
<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": []
}
-->
