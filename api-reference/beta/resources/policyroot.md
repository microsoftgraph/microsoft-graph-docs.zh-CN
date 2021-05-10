---
title: policyRoot 资源类型
description: unifiedRoleManagementPolicy 和 unifiedRoleManagementPolicyAssignment 的新导航属性绑定到 policyRoot。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85c334c52ab2bb196bcfce24610414a0843f898a
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299181"
---
# <a name="policyroot-resource-type"></a><span data-ttu-id="1ef6e-103">policyRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ef6e-103">policyRoot resource type</span></span>

<span data-ttu-id="1ef6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ef6e-105">unifiedRoleManagementPolicy 和 unifiedRoleManagementPolicyAssignment 的新导航属性绑定到 policyRoot。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-105">A new navigation properties binding for unifiedRoleManagementPolicy and unifiedRoleManagementPolicyAssignment to policyRoot.</span></span>

## <a name="methods"></a><span data-ttu-id="1ef6e-106">方法</span><span class="sxs-lookup"><span data-stu-id="1ef6e-106">Methods</span></span>
|<span data-ttu-id="1ef6e-107">方法</span><span class="sxs-lookup"><span data-stu-id="1ef6e-107">Method</span></span>|<span data-ttu-id="1ef6e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ef6e-108">Return type</span></span>|<span data-ttu-id="1ef6e-109">说明</span><span class="sxs-lookup"><span data-stu-id="1ef6e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ef6e-110">列出 roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="1ef6e-110">List roleManagementPolicies</span></span>](../api/policyroot-list-rolemanagementpolicies.md)|<span data-ttu-id="1ef6e-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ef6e-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="1ef6e-112">从 roleManagementPolicies 导航属性获取 unifiedRoleManagementPolicy 资源。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-112">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>|
|[<span data-ttu-id="1ef6e-113">列出 roleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="1ef6e-113">List roleManagementPolicyAssignments</span></span>](../api/policyroot-list-rolemanagementpolicyassignments.md)|<span data-ttu-id="1ef6e-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ef6e-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="1ef6e-115">从 roleManagementPolicyAssignments 导航属性获取 unifiedRoleManagementPolicyAssignment 资源。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-115">Get the unifiedRoleManagementPolicyAssignment resources from the roleManagementPolicyAssignments navigation property.</span></span>|

<!--
## Properties
|Property|Type|Description|
|:---|:---|:---|


## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleManagementPolicies|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection|Represents the role management policies.|
|roleManagementPolicyAssignments|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection|Represents the role management policy assignments.|
-->

## <a name="json-representation"></a><span data-ttu-id="1ef6e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ef6e-116">JSON representation</span></span>
<span data-ttu-id="1ef6e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

