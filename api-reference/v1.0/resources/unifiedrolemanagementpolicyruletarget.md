---
title: unifiedRoleManagementPolicyRuleTarget 资源类型
description: 定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1ae571305de5d7f20635467e65d38090761b21ce
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134020"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>unifiedRoleManagementPolicyRuleTarget 资源类型

命名空间：microsoft.graph

定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|来电|String|作为策略规则目标的调用方的类型。 允许的值为： `None`， ， `Admin``EndUser`.|
|enforcedSettings|String 集合|已强制执行且无法由子范围重写的角色设置的列表。 用于 `All` 所有设置。|
|inheritableSettings|字符串集合|可由子范围继承的角色设置列表。 用于 `All` 所有设置。|
|水平|String|作为策略规则目标的角色分配类型。 允许的值为： `Eligibility`. `Assignment`   |
|operations|String 集合|作为策略规则目标的角色管理操作。 允许的值为： `All`， `Activate`， `Deactivate`， `Assign`， `Remove``Update`， `Extend`。 `Renew`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|targetObjects|[directoryObject](../resources/directoryobject.md) 集合| 策略范围内的用户、组和服务主体的集合。 如果未指定，则所有对象都在策略范围内。|

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

