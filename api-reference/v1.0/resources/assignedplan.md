---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
ms.localizationpriority: medium
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 599a462e49822c6b69fe75ac7104a101e986db6c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333188"
---
# <a name="assignedplan-resource-type"></a>assignedPlan 资源类型

命名空间：microsoft.graph

**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。


## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|分配计划的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|capabilityStatus|String|功能分配的条件。 可能的值为 、`Enabled``Deleted``Warning``Suspended`、。 `LockedOut` 请参阅 [每个值的](#capabilitystatus-values) 详细说明。|
|service|String|服务的名称;例如， `exchange`。|
|servicePlanId|Guid|用于标识服务计划的 GUID。 有关 GUID 及其等效友好服务名称的完整列表，请参阅许可的产品名称和服务 [计划标识符](/azure/active-directory/enterprise-users/licensing-service-plan-reference)。|


### <a name="capabilitystatus-values"></a>capabilityStatus 值

| 成员 | 说明  |
|:---------------|:--------|
| 已启用 | 可供正常使用。 |
| 警告 | 可供正常使用，但位于宽限期内。 |
| 已暂停 | 不可用，但必须保留与功能关联的任何数据。 |
| Deleted | 不可用，并且可能会删除与功能关联的任何数据。 |
| LockedOut | 所有管理员和用户都不可用，但必须保留与功能关联的任何数据。 |

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
  "capabilityStatus": "String",
  "service": "String",
  "servicePlanId": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

