---
title: unifiedRoleManagementPolicyRuleTarget 资源类型
description: unifiedRoleManagementPolicyRuleTarget 指定与角色管理策略相关联的目标。
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c4d7bfb6744c3272e9237590b4d17c5e1d79b0f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074442"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>unifiedRoleManagementPolicyRuleTarget 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicyRuleTarget 指定与角色管理策略相关联的目标。


## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|呼叫者|String|策略规则目标的调用方。 允许的值包括 `None` `Admin` `EndUser` ：、、。|
|enforcedSettings|String collection|强制且不能由子范围覆盖的设置列表。 用于 `All` 所有设置。|
|inheritableSettings|String collection|子作用域可继承的设置列表。 用于 `All` 所有设置。|
|level|String|策略规则目标的级别。 允许的值包括 `Eligibility` `Assignment` ：、。    |
|operations|String collection|策略规则目标的操作。 允许的值为 `All` `Activate` `Deactivate` ：、、、、、、、。 `Assign` `Update` `Remove` `Extend` `Renew`|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|targetObjects|[directoryObject](../resources/directoryobject.md) 集合|策略范围内用户、组和 servicePrincipals 的集合。 如果未指定，则所有对象均在策略范围内。|
-->
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

