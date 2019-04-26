---
title: licenseAssignmentState 资源类型
description: 'user 实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 它提供了对用户的许可证分配的详细信息。 详细信息包括如下信息:  '
localization_priority: Normal
ms.openlocfilehash: 1aa91dcb841c8f3219ba0ea00ad615777da89aa9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345337"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="bad05-105">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="bad05-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bad05-106">[user](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。</span><span class="sxs-lookup"><span data-stu-id="bad05-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="bad05-107">它提供了对用户的许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bad05-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="bad05-108">详细信息包括如下信息:</span><span class="sxs-lookup"><span data-stu-id="bad05-108">The details includes information like:</span></span>  

 - <span data-ttu-id="bad05-109">为用户禁用了哪些计划</span><span class="sxs-lookup"><span data-stu-id="bad05-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="bad05-110">是否将许可证直接分配给用户或从组继承。</span><span class="sxs-lookup"><span data-stu-id="bad05-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="bad05-111">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="bad05-111">Current state of the assignment</span></span>
 - <span data-ttu-id="bad05-112">如果工作分配状态为 "错误", 则失败的错误详细信息是什么？</span><span class="sxs-lookup"><span data-stu-id="bad05-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="bad05-113">属性</span><span class="sxs-lookup"><span data-stu-id="bad05-113">Properties</span></span>
| <span data-ttu-id="bad05-114">属性</span><span class="sxs-lookup"><span data-stu-id="bad05-114">Property</span></span>     | <span data-ttu-id="bad05-115">类型</span><span class="sxs-lookup"><span data-stu-id="bad05-115">Type</span></span>   |<span data-ttu-id="bad05-116">说明</span><span class="sxs-lookup"><span data-stu-id="bad05-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bad05-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="bad05-117">assignedByGroup</span></span>|<span data-ttu-id="bad05-118">string</span><span class="sxs-lookup"><span data-stu-id="bad05-118">string</span></span>|<span data-ttu-id="bad05-119">分配此许可证的组的 id。</span><span class="sxs-lookup"><span data-stu-id="bad05-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="bad05-120">如果分配是直接分配的许可证, 则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="bad05-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="bad05-121">只读。</span><span class="sxs-lookup"><span data-stu-id="bad05-121">Read-Only.</span></span>|
|<span data-ttu-id="bad05-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="bad05-122">disabledPlans</span></span>|<span data-ttu-id="bad05-123">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="bad05-123">Collection(String)</span></span>|<span data-ttu-id="bad05-124">此工作分配中禁用的服务计划。</span><span class="sxs-lookup"><span data-stu-id="bad05-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="bad05-125">只读。</span><span class="sxs-lookup"><span data-stu-id="bad05-125">Read-Only.</span></span>|
|<span data-ttu-id="bad05-126">error</span><span class="sxs-lookup"><span data-stu-id="bad05-126">error</span></span>|<span data-ttu-id="bad05-127">String</span><span class="sxs-lookup"><span data-stu-id="bad05-127">String</span></span>|<span data-ttu-id="bad05-128">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="bad05-128">License assignment failure error.</span></span> <span data-ttu-id="bad05-129">如果许可证分配成功, 则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="bad05-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="bad05-130">只读。</span><span class="sxs-lookup"><span data-stu-id="bad05-130">Read-Only.</span></span> <span data-ttu-id="bad05-131">可能的值`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、和`Others`。</span><span class="sxs-lookup"><span data-stu-id="bad05-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="bad05-132">有关如何识别和解决许可证分配错误的详细信息, 请参阅[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="bad05-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="bad05-133">skuId</span><span class="sxs-lookup"><span data-stu-id="bad05-133">skuId</span></span>|<span data-ttu-id="bad05-134">String</span><span class="sxs-lookup"><span data-stu-id="bad05-134">String</span></span>|<span data-ttu-id="bad05-135">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bad05-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="bad05-136">只读。</span><span class="sxs-lookup"><span data-stu-id="bad05-136">Read-Only.</span></span>|
|<span data-ttu-id="bad05-137">state</span><span class="sxs-lookup"><span data-stu-id="bad05-137">state</span></span>|<span data-ttu-id="bad05-138">String</span><span class="sxs-lookup"><span data-stu-id="bad05-138">String</span></span>|<span data-ttu-id="bad05-139">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="bad05-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="bad05-140">只读。</span><span class="sxs-lookup"><span data-stu-id="bad05-140">Read-Only.</span></span> <span data-ttu-id="bad05-141">可能的值: Active、ActiveWithError、Disabled 和 Error。</span><span class="sxs-lookup"><span data-stu-id="bad05-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bad05-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bad05-142">JSON representation</span></span>

<span data-ttu-id="bad05-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bad05-143">Here is a JSON representation of the resource</span></span>

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
