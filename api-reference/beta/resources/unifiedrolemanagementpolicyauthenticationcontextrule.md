---
title: unifiedRoleManagementPolicyAuthenticationContextRule 资源类型
description: unifiedRoleManagementPolicyAuthenticationContextRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d12f3ed100179198d66fe780c9aee6dd93039012edfc105ac58001d24f6e3d77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155888"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>unifiedRoleManagementPolicyAuthenticationContextRule 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicyAuthenticationContextRule 指定与角色管理策略关联的启用规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。

继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|claimValue|字符串|身份验证上下文声明的值。|
|id|String|规则的唯一标识符。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|isEnabled|Boolean|指示设置是否已启用。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|规则的目标。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

