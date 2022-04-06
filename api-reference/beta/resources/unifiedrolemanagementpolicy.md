---
title: unifiedRoleManagementPolicy 资源类型
description: unifiedRoleManagementPolicy 指定与作用域和角色定义关联的各种策略。 它派生自 microsoft.graph.policyBase。
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d458ab00c772040380adcb9aae800205fe82dc8e
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510174"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>unifiedRoleManagementPolicy 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicy 指定与作用域和角色Azure AD相关联的各种策略。 它派生自 [实体](entity.md)。 对于适用于 Azure RBAC 的策略，将 [Azure REST PIM API 用于角色管理策略](/rest/api/authorization/role-management-policies)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合|获取 [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象及其属性的列表。|
|[获取 unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|读取给定作用域 [的 unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象的属性和关系。|
|[List rules](../api/unifiedrolemanagementpolicy-list-rules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|从 rules 导航属性获取 unifiedRoleManagementPolicyRule 资源。|
|[获取规则](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|获取 unifiedRoleManagementPolicyRule 对象的规则。|
|[更新规则](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|更新 unifiedRoleManagementPolicyRule 对象的规则。|
<!--unsurface effectiveRules because it hasn't been implemented
|[List effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection|Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.|
-->

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略的说明。|
|displayName|字符串|策略的显示名称。|
|id|String|策略的唯一标识符。|
|isOrganizationDefault|Boolean|对于将适用于所有作用域和角色的单个租户范围策略，这只能设置为 true。 将 scopeId 设置为"/"，将 scopeType 设置为 Directory。|
|lastModifiedBy|[identity](../resources/identity.md)|上次修改角色设置的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改角色设置的时间。|
|scopeId|String|创建策略的范围的 ID。 适用于 `/` 租户或组 ID。 必需项。|
|scopeType|字符串|创建策略的范围类型。 其中一`Directory`个。 `DirectoryRole` 必填。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|effectiveRules|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|**未实现。** 根据继承的引用规则评估的有效规则（如审批规则和过期规则）的列表。 例如，如果有租户范围的策略强制启用审批规则，则有效规则将为启用审批，即使该策略具有禁用审批的规则。|
|规则|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|审批规则和过期规则等规则的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
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

