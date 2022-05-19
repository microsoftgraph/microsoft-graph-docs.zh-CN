---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
ms.localizationpriority: medium
author: jconley76
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e1ac85a836ce9b46c908b33cc5d9577c40188ebc
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549454"
---
# <a name="assignedplan-resource-type"></a>assignedPlan 资源类型

命名空间：microsoft.graph

**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。


## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|分配计划的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|capabilityStatus|String|功能分配的条件。 可能的值是`Enabled`， ， `Suspended``Warning`， ， `Deleted`。 `LockedOut` 请参阅每个值的 [详细说明](#capabilitystatus-values) 。|
|service|String|服务的名称;例如， `exchange`.|
|servicePlanId|Guid|用于标识服务计划的 GUID。 有关 GUID 及其等效友好服务名称的完整列表，请参阅 [产品名称和服务计划标识符以获取许可](/azure/active-directory/enterprise-users/licensing-service-plan-reference)。|


### <a name="capabilitystatus-values"></a>capabilityStatus 值

| 成员 | 说明  |
|:---------------|:--------|
| 已启用 | 可用于正常使用。 |
| 警告 | 可用于正常使用，但处于宽限期。 |
| 已暂停 | 不可用，但必须保留与该功能关联的任何数据。 |
| Deleted | 不可用，可能删除与该功能关联的任何数据。 |
| LockedOut | 所有管理员和用户都不可用，但必须保留与该功能关联的任何数据。 |

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

