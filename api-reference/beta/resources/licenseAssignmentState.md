---
title: licenseAssignmentState 资源类型
description: 'User 实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 它提供了对用户的许可证分配的详细信息。 详细信息包括如下信息:  '
localization_priority: Normal
ms.openlocfilehash: e720070c4c97c58fd3c99e49656d7ca33f5fb9d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778423"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="3c7c9-105">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c7c9-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c7c9-106">[User](user.md)实体的**LicenseAssignmentStates**属性是**licenseAssignmentState**的集合。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="3c7c9-107">它提供了对用户的许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="3c7c9-108">详细信息包括如下信息:</span><span class="sxs-lookup"><span data-stu-id="3c7c9-108">The details includes information like:</span></span>  

- <span data-ttu-id="3c7c9-109">为用户禁用了哪些计划</span><span class="sxs-lookup"><span data-stu-id="3c7c9-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="3c7c9-110">是否将许可证直接分配给用户或从组继承。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="3c7c9-111">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="3c7c9-111">Current state of the assignment</span></span>
- <span data-ttu-id="3c7c9-112">如果工作分配状态为 "错误", 则失败的错误详细信息是什么？</span><span class="sxs-lookup"><span data-stu-id="3c7c9-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="3c7c9-113">属性</span><span class="sxs-lookup"><span data-stu-id="3c7c9-113">Properties</span></span>
| <span data-ttu-id="3c7c9-114">属性</span><span class="sxs-lookup"><span data-stu-id="3c7c9-114">Property</span></span>     | <span data-ttu-id="3c7c9-115">类型</span><span class="sxs-lookup"><span data-stu-id="3c7c9-115">Type</span></span>   |<span data-ttu-id="3c7c9-116">说明</span><span class="sxs-lookup"><span data-stu-id="3c7c9-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c7c9-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="3c7c9-117">assignedByGroup</span></span>|<span data-ttu-id="3c7c9-118">string</span><span class="sxs-lookup"><span data-stu-id="3c7c9-118">string</span></span>|<span data-ttu-id="3c7c9-119">分配此许可证的组的 id。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="3c7c9-120">如果分配是直接分配的许可证, 则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="3c7c9-121">只读。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-121">Read-Only.</span></span>|
|<span data-ttu-id="3c7c9-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="3c7c9-122">disabledPlans</span></span>|<span data-ttu-id="3c7c9-123">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="3c7c9-123">Collection(String)</span></span>|<span data-ttu-id="3c7c9-124">此工作分配中禁用的服务计划。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="3c7c9-125">只读。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-125">Read-Only.</span></span>|
|<span data-ttu-id="3c7c9-126">error</span><span class="sxs-lookup"><span data-stu-id="3c7c9-126">error</span></span>|<span data-ttu-id="3c7c9-127">String</span><span class="sxs-lookup"><span data-stu-id="3c7c9-127">String</span></span>|<span data-ttu-id="3c7c9-128">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-128">License assignment failure error.</span></span> <span data-ttu-id="3c7c9-129">如果许可证分配成功, 则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="3c7c9-130">只读。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-130">Read-Only.</span></span> <span data-ttu-id="3c7c9-131">可能的值`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、和`Others`。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="3c7c9-132">有关如何识别和解决许可证分配错误的详细信息, 请参阅[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="3c7c9-133">skuId</span><span class="sxs-lookup"><span data-stu-id="3c7c9-133">skuId</span></span>|<span data-ttu-id="3c7c9-134">String</span><span class="sxs-lookup"><span data-stu-id="3c7c9-134">String</span></span>|<span data-ttu-id="3c7c9-135">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="3c7c9-136">只读。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-136">Read-Only.</span></span>|
|<span data-ttu-id="3c7c9-137">state</span><span class="sxs-lookup"><span data-stu-id="3c7c9-137">state</span></span>|<span data-ttu-id="3c7c9-138">String</span><span class="sxs-lookup"><span data-stu-id="3c7c9-138">String</span></span>|<span data-ttu-id="3c7c9-139">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="3c7c9-140">只读。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-140">Read-Only.</span></span> <span data-ttu-id="3c7c9-141">可能的值: Active、ActiveWithError、Disabled 和 Error。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c7c9-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c7c9-142">JSON representation</span></span>

<span data-ttu-id="3c7c9-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c7c9-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
