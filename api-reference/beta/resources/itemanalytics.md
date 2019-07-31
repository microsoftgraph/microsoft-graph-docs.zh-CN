---
author: daspek
description: ItemAnalytics 资源提供有关项目上发生的活动的分析。 此资源目前仅适用于 SharePoint 和 OneDrive for business。
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d2be5c7665961248e989101a1a9bd21eb805e6e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967093"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemAnalytics**资源提供有关项目上发生的活动的分析。 此资源目前仅适用于 SharePoint 和 OneDrive for business。

您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。

>**注意:****ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。

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

## <a name="properties"></a>属性

| 属性      | 类型                 | 说明
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | 对项目生命周期的分析。
| lastSevenDays | [itemActivityStat][] | 最近七天的分析。

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

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
