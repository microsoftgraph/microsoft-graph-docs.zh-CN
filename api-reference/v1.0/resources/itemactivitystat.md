---
author: daspek
title: itemActivityStat 资源类型
description: ItemActivityStat 对象提供有关在项目上发生的活动的信息。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 97702f31f8b6125b06d3c34eba9eda596604422c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113663"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat 资源类型

命名空间：microsoft.graph

**itemActivityStat** 资源提供有关某个时间间隔内发生的活动的信息。

## <a name="properties"></a>属性

| 属性         | 类型                    | 说明
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | 指示此间隔中的统计信息基于不完整的数据。 只读。
| isTrending       | 布尔值                 | 指示项目是否是"趋势"。 只读。
| startDateTime    | DateTimeOffset          | 间隔开始时。 只读。
| endDateTime      | DateTimeOffset          | 间隔结束时。 只读。
| create           | [itemActionStat][]      | 有关此 **间隔中的** 创建操作统计信息。 只读。
| edit             | [itemActionStat][]      | 有关此 **间隔中的** 编辑操作统计信息。 只读。
| delete           | [itemActionStat][]      | 有关此 **间隔中的** 删除操作统计信息。 只读。
| move             | [itemActionStat][]      | 有关此 **间隔中的** 移动操作统计信息。 只读。
| access           | [itemActionStat][]      | 有关此 **间隔中的** 访问操作统计信息。 只读。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>关系

| 关系名称 | 类型                        | 说明
|:------------------|:----------------------------|:---------------------------
| activities        | [itemActivity][] 集合 | 公开此 **itemActivityStat** 资源中表示的 **itemActivities。**

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

