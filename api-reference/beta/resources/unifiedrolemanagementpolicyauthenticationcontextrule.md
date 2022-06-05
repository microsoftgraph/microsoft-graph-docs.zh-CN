---
title: unifiedRoleManagementPolicyAuthenticationContextRule 资源类型
description: 一种派生自 unifiedRoleManagementPolicyRule 资源类型的类型，用于定义与角色管理策略关联的条件访问策略的身份验证上下文规则。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 118f24e9b449dbe2b1b8069741cea26e7f032990
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900448"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>unifiedRoleManagementPolicyAuthenticationContextRule 资源类型

命名空间：microsoft.graph

一种派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 资源类型的类型，用于定义与角色管理策略关联的条件访问策略的身份验证上下文规则。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|claimValue|字符串|身份验证上下文声明的值。|
|id|字符串|规则的标识符。 继承自 [entity](../resources/entity.md)。|
|isEnabled|Boolean| 是否启用此规则。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|定义启用规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。 支持 `$filter`（`eq`、`ne`）。|

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

