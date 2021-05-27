---
title: unifiedRoleManagementPolicyAssignment 资源类型
description: unifiedRoleManagementPolicyAssignment 将策略分配给特定作用域和角色定义。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0b51d9c088a9d6da4e1a3a671dd578e07ed22691
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682619"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>unifiedRoleManagementPolicyAssignment 资源类型

unifiedRoleManagementPolicyAssignment 将策略分配给特定作用域和角色定义。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleManagementPolicyAssignments](../api/unifiedrolemanagementpolicyassignment-list.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合|获取 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象及其属性的列表。|
|[获取 unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|读取 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略分配的唯一标识符。|
|policyId|String|策略的 ID。|
|roleDefinitionId|String|应用策略的角色定义的 ID。 如果未指定，则策略适用于所有角色。|
|scopeId|String|分配策略的范围的 ID。 例如， "/"、groupId 等。|
|scopeType|String|分配策略的范围类型。 Directory、DirectoryRole、Group 之一。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|策略|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|工作分配的策略。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "id": "String (identifier)",
  "policyId": "String",
  "scopeId": "String",
  "scopeType": "String",
  "roleDefinitionId": "String"
}
```

