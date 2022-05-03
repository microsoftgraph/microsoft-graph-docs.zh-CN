---
author: daspek
description: itemAnalytics 资源提供有关在项上发生的活动的分析。 此资源目前仅在SharePoint和OneDrive for Business上可用。
ms.date: 09/14/2017
title: ItemAnalytics
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 15bd59f04384f2b18329f581f568ee465a86c040
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176931"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemAnalytics** 资源提供有关在项上发生的活动的分析。 此资源目前仅在SharePoint和OneDrive for Business上可用。

还可以使用 [getActivitiesByInterval][] API 在自定义时间范围或间隔内检索分析。

>**注意：****itemAnalytics** 资源在所有 [国家部署](/graph/deployments)中尚不可用。

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

| 属性      | 类型                 | Description
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | 有关项目生存期的分析。
| lastSevenDays | [itemActivityStat][] | 过去七天的分析。

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


