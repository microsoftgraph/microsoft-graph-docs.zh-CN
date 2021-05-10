---
title: unifiedRoleManagementPolicyAssignment 资源类型
description: unifiedRoleManagementPolicyAssignment 将策略分配给特定作用域和角色定义。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3028655cb1b7acd88764abf64dd609147b399a07
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299237"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a><span data-ttu-id="3bfa5-103">unifiedRoleManagementPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bfa5-103">unifiedRoleManagementPolicyAssignment resource type</span></span>

<span data-ttu-id="3bfa5-104">unifiedRoleManagementPolicyAssignment 将策略分配给特定作用域和角色定义。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-104">A unifiedRoleManagementPolicyAssignment assigns the policy to a specific scope and role definition.</span></span>

## <a name="methods"></a><span data-ttu-id="3bfa5-105">方法</span><span class="sxs-lookup"><span data-stu-id="3bfa5-105">Methods</span></span>
|<span data-ttu-id="3bfa5-106">方法</span><span class="sxs-lookup"><span data-stu-id="3bfa5-106">Method</span></span>|<span data-ttu-id="3bfa5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3bfa5-107">Return type</span></span>|<span data-ttu-id="3bfa5-108">说明</span><span class="sxs-lookup"><span data-stu-id="3bfa5-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3bfa5-109">列出 unifiedRoleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="3bfa5-109">List unifiedRoleManagementPolicyAssignments</span></span>](../api/unifiedrolemanagementpolicyassignment-list.md)|<span data-ttu-id="3bfa5-110">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bfa5-110">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="3bfa5-111">获取 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-111">Get a list of the [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects and their properties.</span></span>|
|[<span data-ttu-id="3bfa5-112">获取 unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3bfa5-112">Get unifiedRoleManagementPolicyAssignment</span></span>](../api/unifiedrolemanagementpolicyassignment-get.md)|[<span data-ttu-id="3bfa5-113">unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3bfa5-113">unifiedRoleManagementPolicyAssignment</span></span>](../resources/unifiedrolemanagementpolicyassignment.md)|<span data-ttu-id="3bfa5-114">读取 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-114">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3bfa5-115">属性</span><span class="sxs-lookup"><span data-stu-id="3bfa5-115">Properties</span></span>
|<span data-ttu-id="3bfa5-116">属性</span><span class="sxs-lookup"><span data-stu-id="3bfa5-116">Property</span></span>|<span data-ttu-id="3bfa5-117">类型</span><span class="sxs-lookup"><span data-stu-id="3bfa5-117">Type</span></span>|<span data-ttu-id="3bfa5-118">说明</span><span class="sxs-lookup"><span data-stu-id="3bfa5-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bfa5-119">id</span><span class="sxs-lookup"><span data-stu-id="3bfa5-119">id</span></span>|<span data-ttu-id="3bfa5-120">String</span><span class="sxs-lookup"><span data-stu-id="3bfa5-120">String</span></span>|<span data-ttu-id="3bfa5-121">策略分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-121">Unique identifier for the policy assignment.</span></span>|
|<span data-ttu-id="3bfa5-122">policyId</span><span class="sxs-lookup"><span data-stu-id="3bfa5-122">policyId</span></span>|<span data-ttu-id="3bfa5-123">String</span><span class="sxs-lookup"><span data-stu-id="3bfa5-123">String</span></span>|<span data-ttu-id="3bfa5-124">策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-124">The id of the policy.</span></span>|
|<span data-ttu-id="3bfa5-125">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3bfa5-125">roleDefinitionId</span></span>|<span data-ttu-id="3bfa5-126">String</span><span class="sxs-lookup"><span data-stu-id="3bfa5-126">String</span></span>|<span data-ttu-id="3bfa5-127">应用策略的角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-127">The id of the role definition where the policy applies.</span></span> <span data-ttu-id="3bfa5-128">如果未指定，则策略适用于所有角色。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-128">If not specified, the policy applies to all roles.</span></span>|
|<span data-ttu-id="3bfa5-129">scopeId</span><span class="sxs-lookup"><span data-stu-id="3bfa5-129">scopeId</span></span>|<span data-ttu-id="3bfa5-130">String</span><span class="sxs-lookup"><span data-stu-id="3bfa5-130">String</span></span>|<span data-ttu-id="3bfa5-131">分配策略的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-131">The id of the scope where the policy is assigned.</span></span> <span data-ttu-id="3bfa5-132">例如，</span><span class="sxs-lookup"><span data-stu-id="3bfa5-132">E.g.</span></span> <span data-ttu-id="3bfa5-133">"/"、groupId 等。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-133">"/", groupId, etc.</span></span>|
|<span data-ttu-id="3bfa5-134">scopeType</span><span class="sxs-lookup"><span data-stu-id="3bfa5-134">scopeType</span></span>|<span data-ttu-id="3bfa5-135">String</span><span class="sxs-lookup"><span data-stu-id="3bfa5-135">String</span></span>|<span data-ttu-id="3bfa5-136">分配策略的范围类型。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-136">The type of the scope where the policy is assigned.</span></span> <span data-ttu-id="3bfa5-137">Directory、DirectoryRole、Group 之一。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-137">One of Directory, DirectoryRole, Group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bfa5-138">关系</span><span class="sxs-lookup"><span data-stu-id="3bfa5-138">Relationships</span></span>
|<span data-ttu-id="3bfa5-139">关系</span><span class="sxs-lookup"><span data-stu-id="3bfa5-139">Relationship</span></span>|<span data-ttu-id="3bfa5-140">类型</span><span class="sxs-lookup"><span data-stu-id="3bfa5-140">Type</span></span>|<span data-ttu-id="3bfa5-141">说明</span><span class="sxs-lookup"><span data-stu-id="3bfa5-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bfa5-142">策略</span><span class="sxs-lookup"><span data-stu-id="3bfa5-142">policy</span></span>|[<span data-ttu-id="3bfa5-143">unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="3bfa5-143">unifiedRoleManagementPolicy</span></span>](../resources/unifiedrolemanagementpolicy.md)|<span data-ttu-id="3bfa5-144">工作分配的策略。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-144">The policy for the assignment.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bfa5-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bfa5-145">JSON representation</span></span>
<span data-ttu-id="3bfa5-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bfa5-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "id": "String (identifier)",
  "policyId": "String",
  "scopeId": "String",
  "scopeType": "String",
  "roleDefinitionId": "String"
}
```

