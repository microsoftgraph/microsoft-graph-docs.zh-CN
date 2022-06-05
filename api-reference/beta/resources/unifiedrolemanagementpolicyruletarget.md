---
title: unifiedRoleManagementPolicyRuleTarget 资源类型
description: 定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 47989969bdce1060d01a6e4b300b5df9e16de67a
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899062"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>unifiedRoleManagementPolicyRuleTarget 资源类型

命名空间：microsoft.graph

定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|来电|字符串|作为策略规则目标的调用方的类型。 允许的值为： `None`， ， `Admin``EndUser`.|
|enforcedSettings|String collection|已强制执行且无法由子范围重写的角色设置的列表。 用于 `All` 所有设置。|
|inheritableSettings|String collection|可由子范围继承的角色设置列表。 用于 `All` 所有设置。|
|水平|字符串|作为策略规则目标的角色分配类型。 允许的值为： `Eligibility`. `Assignment`   |
|operations|String collection|作为策略规则目标的角色管理操作。 允许的值为： `All`， `Activate`， `Deactivate`， `Assign`， `Remove``Update`， `Extend`。 `Renew`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|targetObjects|[directoryObject](../resources/directoryobject.md) collection| 策略范围内的用户、组和服务主体的集合。 如果未指定，则所有对象都在策略范围内。|

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