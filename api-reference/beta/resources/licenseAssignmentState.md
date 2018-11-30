---
title: licenseAssignmentState 资源类型
description: '用户实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 为用户提供有关许可证分配的详细信息。 详细信息包括类似的信息：  '
ms.openlocfilehash: 4e7101acc756a845913a081368b79242834ef3bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047225"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
|error|字符串|许可证分配失败错误。 如果已成功分配许可证，此字段为 Null。 只读。 可能的值： `CountViolation`， `MutuallyExclusiveViolation`， `DependencyViolation`， `ProhibitedInUsageLocationViolation`， `UniquenessViolation`，和`Others`。 有关详细信息如何确定和解决许可证分配错误请参见[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|字符串|此 SKU 的唯一标识符。 只读。|
|状态|字符串|指示此工作分配的当前状态。 只读。 可能的值： 活动、 ActiveWithError、 已禁用和错误。|

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