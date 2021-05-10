---
title: unifiedRoleManagementPolicy 资源类型
description: unifiedRoleManagementPolicy 指定与作用域和角色定义关联的各种策略。 它派生自 microsoft.graph.policyBase。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 73510f928fa4a32e92ff0a50b3439ab60dfb95f8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299177"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>unifiedRoleManagementPolicy 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicy 指定与作用域和角色定义关联的各种策略。 它派生自 microsoft.graph.policyBase。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合|获取 [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象及其属性的列表。|
|[获取 unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|读取 [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象的属性和关系。|
|[列出 effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。|
|[List rules](../api/unifiedrolemanagementpolicy-list-rules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|从 rules 导航属性获取 unifiedRoleManagementPolicyRule 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略的说明。|
|displayName|String|策略的显示名称。|
|id|String|策略的唯一标识符。|
|isOrganizationDefault|Boolean|对于将适用于所有作用域和角色的单个租户范围策略，这只能设置为 true。 将 scopeId 设置为"/"，将 scopeType 设置为 Directory。|
|lastModifiedBy|[identity](../resources/identity.md)|上次修改角色设置的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改角色设置的时间。|
|scopeId|String|创建策略的范围的 ID。 例如， "/"、groupId 等。|
|scopeType|String|创建策略的范围类型。 Directory、DirectoryRole、Group 之一。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|effectiveRules|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|根据继承的引用规则评估的有效规则（如审批规则、过期规则等）的列表。 例如， 如果存在用于强制执行启用审批规则的租户范围策略，则有效规则将为启用审批，即使该 polcy 具有禁用审批的规则。|
|规则|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|审批规则、过期规则等规则的集合。|

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

