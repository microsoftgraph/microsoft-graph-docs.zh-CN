---
title: unifiedRoleManagementPolicyRuleTarget 资源类型
description: unifiedRoleManagementPolicyRuleTarget 指定与角色管理策略关联的目标。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9681efd333a4ea8db98d7a99f481c473dae3c6fb
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399115"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>unifiedRoleManagementPolicyRuleTarget 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicyRuleTarget 指定与角色管理策略关联的目标。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|来电|String|策略规则目标的调用方。 允许的值为： `None`， ， `Admin``EndUser`.|
|enforcedSettings|String collection|子范围强制执行且无法重写的设置列表。 用于 `All` 所有设置。|
|inheritableSettings|String collection|可由子范围继承的设置列表。 用于 `All` 所有设置。|
|水平|字符串|策略规则目标的级别。 允许的值为： `Eligibility`. `Assignment`    |
|operations|String collection|策略规则目标的操作。 允许的值为： `All`， `Activate`， `Deactivate`， `Assign`， `Remove``Update`， `Extend`。 `Renew`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|targetObjects|[directoryObject](../resources/directoryobject.md) collection|策略范围内的用户、组和 servicePrincipal 的集合。 如果未指定，则所有对象都在策略范围内。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
  "caller": "String",
  "operations": [
    "String"
  ],
  "level": "String",
  "inheritableSettings": [
    "String"
  ],
  "enforcedSettings": [
    "String"
  ]
}
```

