---
author: daspek
description: itemActivityStat 资源提供有关某个时间间隔内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivityStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 27089dcb5e9223710edb60bbdafe88fa0b3f8099
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723903"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemActivityStat** 资源提供有关某个时间间隔内发生的活动的信息。

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

| 属性       | 类型               | 说明                                                                             |
| :------------- | :----------------- | :-------------------------------------------------------------------------------------- |
| incompleteData | [incompleteData][] | 指示此间隔中的统计信息基于不完整的数据。 只读。 |
| isTrending     | Boolean            | 指示项目是否是"趋势"。 只读。                                    |
| startDateTime  | DateTimeOffset     | 间隔开始时。 只读。                                                    |
| endDateTime    | DateTimeOffset     | 间隔结束时。 只读。                                                      |
| create         | [itemActionStat][] | 有关此 **间隔中的** 创建操作统计信息。 只读。                    |
| edit           | [itemActionStat][] | 有关此 **间隔中的** 编辑操作统计信息。 只读。                      |
| delete         | [itemActionStat][] | 有关此 **间隔中的** 删除操作统计信息。 只读。                    |
| move           | [itemActionStat][] | 有关此 **间隔中的** 移动操作统计信息。 只读。                      |
| access         | [itemActionStat][] | 有关此 **间隔中的** 访问操作统计信息。 只读。                    |

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>关系

| 关系 | 类型                        | 说明                                                                       |
| :----------- | :-------------------------- | :-------------------------------------------------------------------------------- |
| activities   | [itemActivity][] 集合 | 公开 **此 itemActivityStat** 资源中表示的 **itemActivities** 。 |

[itemActivity]: itemactivity.md

## <a name="remarks"></a>注解

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
