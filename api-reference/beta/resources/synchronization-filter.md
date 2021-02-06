---
title: 筛选器资源类型
description: 确定应该向应用程序预配哪些对象。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8c461dffab9af810d20f6b866134ecc5d4238eb1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133929"
---
# <a name="filter-resource-type"></a>筛选器资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定应该向应用程序预配哪些对象。 例如，你可能希望仅预配位于美国的用户。 存在作用域筛选器时，在同步过程中将跳过不满足该筛选器的对象。

筛选器是对象 [映射的一部分](synchronization-objectmapping.md)。 它由多组筛选器组组成，每个筛选器组包含一个或多个子句。 在组范围内考虑对象 (只有在组的所有子句都计算为) 计算组时，才计算为一 `true` 个对象 `true` 。

在组集范围内考虑对象， (组集求值) 组集的任何组求值为 `true` `true` 。

有关详细信息，请参阅使用范围筛选器的基于属性 [的应用程序设置](/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|categoryFilterGroups|[filterGroup](synchronization-filtergroup.md) 集合|`*Experimental*` 用于决定给定对象是否属于且应作为此对象映射的一部分进行处理的筛选器组集。 如果将集合中的任一组求值为 ，则视为范围内 *的对象 `true`*。|
|groups|[filterGroup](synchronization-filtergroup.md) 集合|用于决定给定对象是否位于设置范围的筛选器组集。 **这是在大多数情况下应该使用的筛选器**。 如果用于满足此筛选器的对象在给定时刻，然后对象或筛选器已更改，以便不再满足筛选器，则此类对象 *将被取消设置"。 如果将集合中的任一组求值为 ，则视为范围内 *的对象 `true`*。|
|inputFilterGroups|[filterGroup](synchronization-filtergroup.md) 集合|`*Experimental*` 用于在从目录读取对象的早期阶段筛选出对象的筛选器组集。 如果对象不满足此筛选器，则将不会进一步处理该对象。 必须了解的是，如果用于满足此筛选器的对象在给定时刻，然后对象或筛选器已更改，以便不再满足筛选器，则此类对象将不会取消 *设置*。 如果将集合中的任一组求值为 ，则视为范围内 *的对象 `true`*。 |

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


