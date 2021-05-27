---
title: unifiedRoleManagementPolicyEnablementRule 资源类型
description: unifiedRoleManagementPolicyEnablementRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf3ef8e25026c72aab36a9c2fb6241f5bef950da
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680680"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a>unifiedRoleManagementPolicyEnablementRule 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicyEnablementRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。

继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enabledRules|String collection|启用的规则。 允许的值包括 MultifactorAuthentication、Justification、Ticketing。|
|id|String|规则的唯一标识符。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|规则的目标。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

