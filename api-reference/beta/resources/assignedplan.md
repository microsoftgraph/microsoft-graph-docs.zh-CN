---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
localization_priority: Normal
ms.openlocfilehash: 0f44e96e5591d46d6a22b0cdd951b4dfb1e05e75
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339052"
---
# <a name="assignedplan-resource-type"></a>assignedPlan 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|capabilityStatus|String|例如，“Enabled”。|
|服务|String|服务名称；例如，“Exchange”。|
|servicePlanId|Guid|用于标识服务计划的 GUID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
