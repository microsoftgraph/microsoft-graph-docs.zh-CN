---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561899"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemActivityStat**资源提供有关在一段时间内发生的活动的信息。

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

## <a name="properties"></a>属性

| 属性         | 类型                    | 说明
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | 指示此时间间隔中的统计信息基于不完整的数据。 只读。
| isTrending       | 布尔值                 | 指示项目是否为 "趋势"。 只读。
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

## <a name="remarks"></a>注解

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
