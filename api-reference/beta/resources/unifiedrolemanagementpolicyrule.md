---
title: unifiedRoleManagementPolicyRule 资源类型
description: 定义与角色管理策略关联的规则的抽象类型。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4851f090b4e73ace7de7b86fc85db76555c918fa
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898516"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>unifiedRoleManagementPolicyRule 资源类型

命名空间：microsoft.graph

定义与角色管理策略关联的规则的抽象类型。 此抽象类型由以下资源继承，这些资源定义各种类型的规则及其与角色管理策略关联的设置。
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
|id|字符串|规则的标识符。 继承自 [entity](../resources/entity.md)。 只读。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| **未实现。** 定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 支持 `$filter`（`eq`、`ne`）。|

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