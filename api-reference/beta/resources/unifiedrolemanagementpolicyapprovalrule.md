---
title: unifiedRoleManagementPolicyApprovalRule 资源类型
description: 一种派生自 unifiedRoleManagementPolicyRule 资源类型的类型，用于定义批准角色分配的规则。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 882961f6ca7a5caed8ca7eee52bf18de5f7a940a
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900000"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a>unifiedRoleManagementPolicyApprovalRule 资源类型

命名空间：microsoft.graph

一种派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 资源类型的类型，用于定义批准角色分配的规则。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|规则的标识符。 继承自 [entity](../resources/entity.md)。|
|setting|[approvalSettings](../resources/approvalsettings.md)|用于批准角色分配的设置。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|定义审批规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。 支持 `$filter`（`eq`、`ne`）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "setting": {
    "@odata.type": "microsoft.graph.approvalSettings"
  }
}
```

