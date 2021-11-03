---
title: unifiedRoleManagementPolicyRule 资源类型
description: unifiedRoleManagementPolicyRule 指定与角色管理策略关联的规则。 它是抽象的。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cc8f6e135c8dd569040f7d738b7a29fb54fdf98e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688140"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>unifiedRoleManagementPolicyRule 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicyRule 指定与角色管理策略关联的规则。 它是抽象的。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleManagementPolicyRules](../api/unifiedrolemanagementpolicyrule-list.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合|获取 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象及其属性的列表。|
|[获取 unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|读取 [unifiedRoleManagementPolicyRule 对象的属性和](../resources/unifiedrolemanagementpolicyrule.md) 关系。|
|[更新 unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|更新 [unifiedRoleManagementPolicyRule 对象](../resources/unifiedrolemanagementpolicyrule.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|规则的唯一标识符。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|策略规则的目标。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
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

