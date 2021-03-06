---
title: licenseAssignmentState 资源类型
description: '**user 实体的 licenseAssignmentStates** 属性是 **licenseAssignmentState 的集合**。 它提供有关向用户分配的许可证的详细信息。 详细信息包括以下信息：  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 06b469cb80e92ca09a8e1bce7a058aed1b3a570d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547076"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**user 实体的 licenseAssignmentStates** 属性是 **licenseAssignmentState 的集合**。 [](user.md) 它提供有关向用户分配的许可证的详细信息。 详细信息包括以下信息：

- 为用户禁用的计划
- 许可证是直接分配给用户还是从组继承
- 工作分配的当前状态
- 如果工作分配状态为"错误"，则失败的错误详细信息是什么？


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedByGroup|string|分配此许可证的组的 ID。 如果分配是直接分配的许可证，则此字段将为 Null。 只读。|
|disabledPlans|集合（字符串）|在此分配中禁用的服务计划。 只读。|
|error|String|许可证分配失败错误。 如果许可证分配成功，则此字段将为 Null。 只读。 可能的值 `CountViolation` `MutuallyExclusiveViolation` `DependencyViolation` ：、、、、 `ProhibitedInUsageLocationViolation` `UniquenessViolation` 和 `Others` 。 若要详细了解如何识别和解决许可证分配错误，请参阅 [此处](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|String|此 SKU 的唯一标识符。 只读。|
|state|String|指示此工作分配的当前状态。 只读。 可能的值：Active、ActiveWithError、Disabled 和 Error。|

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