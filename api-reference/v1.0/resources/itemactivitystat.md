---
author: daspek
ms.author: dspektor
title: itemActivityStat 资源类型
description: ItemActivityStat 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 11b19e4b953d4353382aec15071c6589b5bb23c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447666"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat 资源类型

命名空间： microsoft. graph

**ItemActivityStat**资源提供有关在一段时间内发生的活动的信息。

## <a name="properties"></a>属性

| 属性         | 类型                    | 说明
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | 指示此时间间隔中的统计信息基于不完整的数据。 只读。
| isTrending       | 布尔                 | 指示项目是否为 "趋势"。 只读。
| startDateTime    | DateTimeOffset          | 时间间隔开始时。 只读。
| endDateTime      | DateTimeOffset          | 时间间隔结束时。 只读。
| create           | [itemActionStat][]      | 有关此间隔中的**创建**操作的统计信息。 只读。
| edit             | [itemActionStat][]      | 有关此间隔中的**编辑**操作的统计信息。 只读。
| delete           | [itemActionStat][]      | 有关此间隔中的**删除**操作的统计信息。 只读。
| move             | [itemActionStat][]      | 有关此间隔中**移动**操作的统计信息。 只读。
| 访问           | [itemActionStat][]      | 有关此间隔中的**访问**操作的统计信息。 只读。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>关系

| 关系名称 | 类型                        | 说明
|:------------------|:----------------------------|:---------------------------
| activities        | [itemActivity][] 集合 | 公开此**itemActivityStat**资源中表示的**itemActivities** 。

[itemActivity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
