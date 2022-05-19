---
title: licenseAssignmentState 资源类型
description: 用户实体的 **licenseAssignmentStates** 属性是 **licenseAssignmentState** 对象的集合。 它向用户提供有关许可证分配的详细信息。
author: jconley76
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 2608cb593908380ea3812ce5a1360a015b757050
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549545"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型

命名空间：microsoft.graph


[用户](user.md)实体的 **licenseAssignmentStates** 属性是 **licenseAssignmentState** 对象的集合。 它向用户提供有关许可证分配的详细信息。 详细信息包括以下信息：  

- 为用户禁用了哪些计划
- 许可证是直接分配给用户还是从组继承
- 分配的当前状态
- 如果分配状态为“错误”，则错误详细信息 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedByGroup|string|分配此许可证的组的 ID。 如果分配是直接分配的许可证，则此字段将为 Null。 只读。|
|disabledPlans|集合（字符串）|在此分配中禁用的服务计划。 只读。|
|error|字符串|许可证分配失败错误。 如果成功分配许可证，则此字段将为 Null。 只读。 可能的值是`CountViolation`， ， `DependencyViolation``MutuallyExclusiveViolation`， `ProhibitedInUsageLocationViolation`， `UniquenessViolation`和 `Other`. 有关如何识别和解决许可证分配错误的详细信息，请参阅 [此处](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|lastUpdatedDateTime|DateTimeOffset|上次更新许可证分配状态的时间戳。|
|skuId|字符串|此 SKU 的唯一标识符。 只读。|
|state|String|指示此分配的当前状态。 只读。 可取值为：`Active`、`ActiveWithError`、`Disabled` 和 `Error`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "lastUpdatedDateTime": "String (timestamp)",
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
