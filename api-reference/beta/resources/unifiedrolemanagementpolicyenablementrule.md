---
title: unifiedRoleManagementPolicyEnablementRule 资源类型
description: 一种派生自 unifiedRoleManagementPolicyRule 资源类型的类型，该类型定义用于启用分配的规则，例如，启用 MFA、分配或票证信息的理由。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 512821df715da8b5b2261293ce18233741d67183
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899076"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a>unifiedRoleManagementPolicyEnablementRule 资源类型

命名空间：microsoft.graph

一种派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 资源类型的类型，该类型定义用于启用分配的规则，例如，启用 MFA、分配或票证信息的理由。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enabledRules|字符串集合|为此策略规则启用的规则的集合。 例如，`MultiFactorAuthentication``Ticketing`和 `Justification`.|
|id|字符串|规则的标识符。 继承自 [entity](../resources/entity.md)。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|定义启用规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。 支持 `$filter`（`eq`、`ne`）。|


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

