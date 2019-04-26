---
title: 筛选器资源类型
description: 确定应将哪些对象设置为应用程序。 例如, 您可能希望仅预配位于美国的用户。 当存在范围筛选器时, 将在同步过程中跳过不满足筛选器的对象。
localization_priority: Normal
ms.openlocfilehash: 0aa75f3b3116991696e9456d7cdfc7b0f72ea86e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345549"
---
# <a name="filter-resource-type"></a>筛选器资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定应将哪些对象设置为应用程序。 例如, 您可能希望仅预配位于美国的用户。 当存在范围筛选器时, 将在同步过程中跳过不满足筛选器的对象。

筛选器是[对象映射](synchronization-objectmapping.md)的一部分。 它由多个筛选器组集组成, 每个筛选器组包含一个或多个子句。 仅当组的所有子句都计算为`true` `true`时, 才会在组的作用域中考虑对象 (组的计算结果为)。

如果将集合中的任意组评估为, `true` `true`则在组集的范围内考虑对象 (组集的计算结果为)。

有关详细信息, 请参阅[基于属性的应用程序预配和作用域筛选器](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|categoryFilterGroups|[filterGroup](synchronization-filtergroup.md)集合|`*Experimental*`用于确定给定对象是否属于的筛选器组集, 以及应作为此对象映射的一部分进行处理的筛选器组集。 *如果集合中的任何组的计算结果为, `true`* 则在范围内考虑对象。|
|groups|[filterGroup](synchronization-filtergroup.md)集合|用于确定给定对象是否在设置范围内的筛选器组集。 **这是在大多数情况下应使用的筛选器**。 如果某个对象在给定时刻满足此筛选器的需要, 然后对象或筛选器发生了更改, 因此不能再满足筛选器的要求, 则此类对象 * 将被取消设置。 *如果集合中的任何组的计算结果为, `true`* 则在范围内考虑对象。|
|inputFilterGroups|[filterGroup](synchronization-filtergroup.md)集合|`*Experimental*`用于在从目录读取对象的早期阶段筛选出对象的筛选器组集。 如果对象不满足此筛选器, 则不会对其进行进一步处理。 需要了解的重要一点是, 如果某个对象在给定时刻满足此筛选器, 然后对象或筛选器已更改, 因此筛选器不再满足要求, 则此类对象*将不会被取消预配*。 *如果集合中的任何组的计算结果为, `true`* 则在范围内考虑对象。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
