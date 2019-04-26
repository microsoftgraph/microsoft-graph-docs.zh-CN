---
title: licenseAssignmentState 资源类型
description: 'user 实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 它提供了对用户的许可证分配的详细信息。 详细信息包括如下信息:  '
localization_priority: Normal
ms.openlocfilehash: 1aa91dcb841c8f3219ba0ea00ad615777da89aa9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345337"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[user](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 它提供了对用户的许可证分配的详细信息。 详细信息包括如下信息:  

 - 为用户禁用了哪些计划
 - 是否将许可证直接分配给用户或从组继承。
 - 工作分配的当前状态
 - 如果工作分配状态为 "错误", 则失败的错误详细信息是什么？ 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedByGroup|string|分配此许可证的组的 id。 如果分配是直接分配的许可证, 则此字段将为 Null。 只读。|
|disabledPlans|集合（字符串）|此工作分配中禁用的服务计划。 只读。|
|error|String|许可证分配失败错误。 如果许可证分配成功, 则此字段将为 Null。 只读。 可能的值`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、和`Others`。 有关如何识别和解决许可证分配错误的详细信息, 请参阅[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|String|此 SKU 的唯一标识符。 只读。|
|state|String|指示此工作分配的当前状态。 只读。 可能的值: Active、ActiveWithError、Disabled 和 Error。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
