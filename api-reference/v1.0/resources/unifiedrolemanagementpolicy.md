---
title: unifiedRoleManagementPolicy 资源类型
description: 指定与范围和角色关联的各种策略。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3e9ce46b44b5e21d326c6c751ae7f6553a2c2199
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246921"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>unifiedRoleManagementPolicy 资源类型

命名空间：microsoft.graph

指定与范围和角色关联的各种策略。 对于适用于 Azure RBAC 的策略，请将 [Azure REST PIM API 用于角色管理策略](/rest/api/authorization/role-management-policies)。

目前，所有策略和关联的规则都是只读的。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合|获取角色管理策略及其详细信息。|
|[获取 unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|检索角色管理策略的详细信息。|
|[List rules](../api/unifiedrolemanagementpolicy-list-rules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|获取为角色管理策略定义的规则。|
|[获取 unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|检索为角色管理策略定义的规则。|
|[更新 unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|更新为角色管理策略定义的规则。|


## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略的说明。|
|displayName|String|策略的显示名称。|
|id|String|策略的唯一标识符。|
|isOrganizationDefault|Boolean|这只能设置 `true` 为单个租户范围的策略，该策略将应用于所有范围和角色。 将 scopeId 设置为 `/` scopeId，并将 scopeType 设置为 `Directory`. 支持 `$filter`（`eq`、`ne`）。|
|lastModifiedBy|[identity](../resources/identity.md)|上次修改角色设置的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改角色设置的时间。|
|scopeId|String|创建策略的范围的标识符。 可以 `/` 用于租户或组 ID。 必填。|
|scopeType|String|创建策略的范围的类型。 其中一 `Directory`个 ， `DirectoryRole`. 必填。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|effectiveRules|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合| 根据继承的引用规则评估的有效规则列表，例如审批规则和过期规则。 例如，如果有租户范围的策略来强制启用审批规则，则有效的规则是启用审批，即使策略有禁用审批的规则。 支持 `$expand`。|
|规则|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|审批规则和过期规则等规则的集合。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isOrganizationDefault": "Boolean",
  "scopeId": "String",
  "scopeType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

