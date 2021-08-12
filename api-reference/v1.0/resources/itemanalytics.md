---
author: daspek
title: itemAnalytics 资源类型
description: ItemAnalytics 对象提供有关在项目上发生的活动的分析。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3ffedd01287f66a5640fa1a1868b05c42a6750ee223bc59546241b47733f1fc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196969"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics 资源类型

命名空间：microsoft.graph

**itemAnalytics** 资源提供有关在项目上发生的活动的分析。 此资源当前仅适用于 SharePoint 和 OneDrive for Business。

您还可以使用 [getActivitiesByInterval][] API 检索自定义时间范围或时间间隔的分析。

>**注意：****itemAnalytics** 资源尚未在所有的国家部署 [中可用](/graph/deployments)。

## <a name="properties"></a>属性

| 属性      | 类型                 | 说明
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | 项目生命周期的分析。
| lastSevenDays | [itemActivityStat][] | 过去七天的分析。

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka&quot;: &quot;oneDrive.analytics"
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

