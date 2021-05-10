---
title: unifiedRoleManagementPolicyRuleTarget 资源类型
description: unifiedRoleManagementPolicyRuleTarget 指定与角色管理策略相关联的目标。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad612355fdcb5089277541ae898ba3429fda7fc9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299185"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a><span data-ttu-id="d2c9b-103">unifiedRoleManagementPolicyRuleTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2c9b-103">unifiedRoleManagementPolicyRuleTarget resource type</span></span>

<span data-ttu-id="d2c9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2c9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2c9b-105">unifiedRoleManagementPolicyRuleTarget 指定与角色管理策略相关联的目标。</span><span class="sxs-lookup"><span data-stu-id="d2c9b-105">A unifiedRoleManagementPolicyRuleTarget specifies the target associated with the role management policy.</span></span>
<!--
## Properties
|Property|Type|Description|
|:---|:---|:---|
|caller|String|The caller for the policy rule target. One of None, Admin, EndUser.  |
|enforcedSettings|String collection|The list of settings which are enforced and cannot be overridden by child scopes. Use All for all settings.|
|inheritableSettings|String collection|The list of settings which can be inherited by child scopes. Use All for all settings.|
|level|String|The level for the policy rule target. One of Eligibility, Assignment. |
|operations|String collection|The operations for policy rule target. One of All, Activate, Deactivate, Assign, Update, Remove, Extend, Renew.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|targetObjects|[directoryObject](../resources/directoryobject.md) collection|The collection of users, groups and servicePrincipals which are in scope of the policy. If not specified, all objects are in scope of the policy.|
-->
## <a name="json-representation"></a><span data-ttu-id="d2c9b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2c9b-106">JSON representation</span></span>
<span data-ttu-id="d2c9b-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2c9b-107">The following is a JSON representation of the resource.</span></span>
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

