---
title: licenseAssignmentState 资源类型
description: User 实体的 **licenseAssignmentStates** 属性是 **licenseAssignmentState** 对象的集合。 它提供了对用户的许可证分配的详细信息。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b26ab4be63cbb40929dbea3f40522ee4c6b7ff70
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582182"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型

命名空间：microsoft.graph


[User](user.md)实体的**LicenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。 它提供了对用户的许可证分配的详细信息。 详细信息包括以下信息：  

- 为用户禁用了哪些计划
- 是否将许可证直接分配给用户或从组继承。
- 工作分配的当前状态
- 如果工作分配状态为错误，则为错误详细信息 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedByGroup|string|分配此许可证的组的 id。 如果分配是直接分配的许可证，则此字段将为 Null。 只读。|
|disabledPlans|集合（字符串）|此工作分配中禁用的服务计划。 只读。|
|error|字符串|许可证分配失败错误。 如果许可证分配成功，则此字段将为 Null。 只读。 可能的值： `CountViolation` 、、、、 `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` 和 `Others` 。 有关如何识别和解决许可证分配错误的详细信息，请参阅 [此处](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|字符串|此 SKU 的唯一标识符。 只读。|
|state|String|指示此工作分配的当前状态。 只读。 可能的值： Active、ActiveWithError、Disabled 和 Error。|

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