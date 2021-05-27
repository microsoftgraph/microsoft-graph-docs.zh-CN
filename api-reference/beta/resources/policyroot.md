---
title: policyRoot 资源类型
description: unifiedRoleManagementPolicy 和 unifiedRoleManagementPolicyAssignment 的新导航属性绑定到 policyRoot。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3827440befd26fb584addd0d6af520a6498c11dd
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680723"
---
# <a name="policyroot-resource-type"></a><span data-ttu-id="4eceb-103">policyRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="4eceb-103">policyRoot resource type</span></span>

<span data-ttu-id="4eceb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eceb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4eceb-105">unifiedRoleManagementPolicy 和 unifiedRoleManagementPolicyAssignment 的新导航属性绑定到 policyRoot。</span><span class="sxs-lookup"><span data-stu-id="4eceb-105">A new navigation properties binding for unifiedRoleManagementPolicy and unifiedRoleManagementPolicyAssignment to policyRoot.</span></span>

## <a name="methods"></a><span data-ttu-id="4eceb-106">方法</span><span class="sxs-lookup"><span data-stu-id="4eceb-106">Methods</span></span>
|<span data-ttu-id="4eceb-107">方法</span><span class="sxs-lookup"><span data-stu-id="4eceb-107">Method</span></span>|<span data-ttu-id="4eceb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4eceb-108">Return type</span></span>|<span data-ttu-id="4eceb-109">说明</span><span class="sxs-lookup"><span data-stu-id="4eceb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4eceb-110">列出 roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="4eceb-110">List roleManagementPolicies</span></span>](../api/policyroot-list-rolemanagementpolicies.md)|<span data-ttu-id="4eceb-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4eceb-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="4eceb-112">从 roleManagementPolicies 导航属性获取 unifiedRoleManagementPolicy 资源。</span><span class="sxs-lookup"><span data-stu-id="4eceb-112">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>|
|[<span data-ttu-id="4eceb-113">列出 roleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="4eceb-113">List roleManagementPolicyAssignments</span></span>](../api/policyroot-list-rolemanagementpolicyassignments.md)|<span data-ttu-id="4eceb-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4eceb-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="4eceb-115">从 roleManagementPolicyAssignments 导航属性获取 unifiedRoleManagementPolicyAssignment 资源。</span><span class="sxs-lookup"><span data-stu-id="4eceb-115">Get the unifiedRoleManagementPolicyAssignment resources from the roleManagementPolicyAssignments navigation property.</span></span>|

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

## <a name="json-representation"></a><span data-ttu-id="4eceb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4eceb-116">JSON representation</span></span>
<span data-ttu-id="4eceb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eceb-117">The following is a JSON representation of the resource.</span></span>
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

