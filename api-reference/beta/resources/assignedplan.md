---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: krbain
ms.openlocfilehash: fe546f2dd25ca7f65e1ce8299bfad9b9ce5be56d
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563420"
---
# <a name="assignedplan-resource-type"></a>assignedPlan 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。


## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|capabilityStatus|[capabilityStatus](#capabilitystatus-values)|功能分配的条件。 可能的值为 `Enabled` 、、、 `Warning` `Suspended` `Deleted` `LockedOut` 。|
|service|String|服务名称；例如，“Exchange”。|
|servicePlanId|Guid|用于标识服务计划的 GUID。|


### <a name="capabilitystatus-values"></a>capabilityStatus 值

| 成员 | 说明  |
|:---------------|:--------|
| 已启用 | 可用于正常使用。 |
| 警告 | 可用于正常使用，但处于宽限期内。 |
| 已暂停 | 不可用，但必须保留与该功能关联的任何数据。 |
| Deleted | 不可用，并且与该功能关联的任何数据可能会被删除。 |
| LockedOut | 对所有管理员和用户不可用，但必须保留与该功能关联的任何数据。 |

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


