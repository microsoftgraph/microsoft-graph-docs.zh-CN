---
title: licenseAssignmentState 资源类型
description: '用户实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 为用户提供有关许可证分配的详细信息。 详细信息包括类似的信息：  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515277"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[用户](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 为用户提供有关许可证分配的详细信息。 详细信息包括类似的信息：  

 - 哪些计划将被禁用的用户
 - 是否许可证已直接分配给用户或从组继承
 - 工作分配的当前状态
 - 如果工作分配状态错误，什么是失败的错误详细信息？ 


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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
