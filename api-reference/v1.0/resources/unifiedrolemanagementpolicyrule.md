---
title: unifiedRoleManagementPolicyRule 资源类型
description: 定义与角色管理策略关联的规则或设置的抽象类型。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54444e25d6967536fa2e9a444fd05adf66467881
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461259"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>unifiedRoleManagementPolicyRule 资源类型

命名空间：microsoft.graph


定义与角色管理策略关联的规则或设置的抽象类型。 此抽象类型由以下资源继承，这些资源定义各种类型的规则及其与角色管理策略关联的设置。
+ [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](unifiedrolemanagementpolicynotificationrule.md)


继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|规则的标识符。 继承自 [entity](../resources/entity.md)。 只读。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| 定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 支持 `$filter`（`eq`、`ne`）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```

