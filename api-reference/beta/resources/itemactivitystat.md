---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041799"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**ItemActivityStat**资源提供有关发生的时间间隔内的活动信息。

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
| incompleteData   | [incompleteData][]      | 指示此间隔中的统计信息基于不完整的数据。 只读。
| isTrending       | 布尔                 | 指示是否项目"趋势。" 只读。
| startDateTime    | DateTimeOffset          | 当开始间隔。 只读。
| endDateTime      | DateTimeOffset          | 当结束间隔。 只读。
| create           | [itemActionStat][]      | 有关此间隔中的**创建**操作的统计信息。 只读。
| edit             | [itemActionStat][]      | 有关此间隔中的**编辑**操作的统计信息。 只读。
| delete           | [itemActionStat][]      | 有关此间隔中的**删除**操作的统计信息。 只读。
| move             | [itemActionStat][]      | 有关此间隔中的**移动**操作的统计信息。 只读。
| 访问           | [itemActionStat][]      | 有关此间隔中的**访问**操作的统计信息。 只读。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>关系

| 关系名称 | 类型                        | 说明
|:------------------|:----------------------------|:---------------------------
| activities        | [itemActivity][] 集合 | 公开**itemActivities**此**itemActivityStat**资源中表示。

[itemActivity]: itemactivity.md

## <a name="remarks"></a>注解

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
