---
title: licenseAssignmentState 资源类型
description: 用户实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。 为用户提供有关许可证分配的详细信息。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649383"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型


[用户](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。 为用户提供有关许可证分配的详细信息。 详细信息包括以下信息：  

 - 哪些计划将被禁用的用户
 - 是否许可证已直接分配给用户或从组继承
 - 当前状态的工作分配
 - 如果工作分配状态错误的错误详细信息 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedByGroup|string|分配此许可证的组 id。 如果工作分配为直接分配许可证，此字段为 Null。 只读。|
|disabledPlans|集合（字符串）|此工作分配中禁用服务计划。 只读。|
|error|String|许可证分配失败错误。 如果已成功分配许可证，此字段为 Null。 只读。 可能的值： `CountViolation`， `MutuallyExclusiveViolation`， `DependencyViolation`， `ProhibitedInUsageLocationViolation`， `UniquenessViolation`，和`Others`。 有关详细信息如何确定和解决许可证分配错误请参见[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|String|此 SKU 的唯一标识符。 只读。|
|state|String|指示此工作分配的当前状态。 只读。 可能的值： 活动、 ActiveWithError、 已禁用和错误。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
