---
title: policyRoot 资源类型
description: unifiedRoleManagementPolicy 和 unifiedRoleManagementPolicyAssignment 的新导航属性绑定到 policyRoot。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3827440befd26fb584addd0d6af520a6498c11dd
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680723"
---
# <a name="policyroot-resource-type"></a>policyRoot 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicy 和 unifiedRoleManagementPolicyAssignment 的新导航属性绑定到 policyRoot。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 roleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合|从 roleManagementPolicies 导航属性获取 unifiedRoleManagementPolicy 资源。|
|[列出 roleManagementPolicyAssignments](../api/policyroot-list-rolemanagementpolicyassignments.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合|从 roleManagementPolicyAssignments 导航属性获取 unifiedRoleManagementPolicyAssignment 资源。|

<!--
## Properties
|Property|Type|Description|
|:---|:---|:---|


## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleManagementPolicies|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection|Represents the role management policies.|
|roleManagementPolicyAssignments|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection|Represents the role management policy assignments.|
-->

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

