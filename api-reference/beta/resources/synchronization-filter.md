---
title: 筛选资源类型
description: 确定哪些对象应该设置到应用程序。 例如，您可能希望向只位于美国的设置用户。 存在范围筛选器时，将同步过程中跳过不满足筛选器的对象。
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894409"
---
# <a name="filter-resource-type"></a>筛选资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

确定哪些对象应该设置到应用程序。 例如，您可能希望向只位于美国的设置用户。 存在范围筛选器时，将同步过程中跳过不满足筛选器的对象。

筛选器是[对象映射](synchronization-objectmapping.md)的一部分。 它包含的筛选器组几组和每个筛选器组包含一个或多个子句。 对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。

对象被视为组集范围内 (组集中计算为`true`) 如果任何集中组计算结果为`true`。

有关详细信息，请参阅[基于属性的应用程序与范围筛选器设置](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|categoryFilterGroups|[filterGroup](synchronization-filtergroup.md)集合|`*Experimental*`用于确定是否给定对象所属的组设置筛选器，并应作为此对象映射的一部分。 对象被视为范围内*如果集合中的组的任何计算结果为`true`*。|
|组|[filterGroup](synchronization-filtergroup.md)集合|组设置用来确定给定对象是否在范围内用于设置筛选器。 **这是在大多数情况下应使用哪些筛选器**。 如果用来满足给定时刻，此筛选器对象然后对象或筛选器已更改，因此该筛选器是不满足任何更长时间，此类对象 * 获取取消设置"。 对象被视为范围内*如果集合中的组的任何计算结果为`true`*。|
|inputFilterGroups|[filterGroup](synchronization-filtergroup.md)集合|`*Experimental*`用于在从目录中读取的早期阶段筛选掉对象的筛选器组设置。 如果对象不满足此筛选器，它将不进一步处理。 一定要了解，如果一个对象用于在给定的时刻，满足此筛选器，然后对象或筛选器已更改，以便该筛选器不再满足，例如对象*不获取取消设置*。 对象被视为范围内*如果集合中的组的任何计算结果为`true`*。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
