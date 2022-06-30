---
title: unifiedRoleManagementPolicyAssignment 资源类型
description: unifiedRoleManagementPolicyAssignment 将策略分配给特定范围和角色定义。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8dfbe842f6e60abec9c0f15881695062e901d5ba
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446313"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>unifiedRoleManagementPolicyAssignment 资源类型

命名空间：microsoft.graph

将角色管理策略分配给 [角色定义](../resources/unifiedroledefinition.md) 对象。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleManagementPolicyAssignments](../api/policyroot-list-rolemanagementpolicyassignments.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合|获取所有角色管理策略分配的详细信息，包括与 Azure AD 角色关联的策略和规则。|
|[获取 unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|读取 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略分配的唯一标识符。 ID 通常是 unifiedRoleManagementPolicy ID 的串联，roleDefinitionId 由下划线分隔。|
|policyId|String|策略的 ID。 继承自 [entity](../resources/entity.md)。|
|roleDefinitionId|String|应用策略 [的角色定义](unifiedroledefinition.md) 对象的标识符。 如果未指定，则策略将应用于所有角色。 支持$filter (`eq`) 。|
|scopeId|String|分配策略的范围的标识符。  可以 `/` 用于租户或组 ID。 必需项。|
|scopeType|String|分配策略的范围的类型。 其中一 `Directory`个 ， `DirectoryRole`. 必填。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|策略|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|与策略分配关联的策略。 支持$expand和策略的规则和有效Rules 关系的嵌套$expand。|

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

