---
title: licenseAssignmentState 资源类型
description: '**用户实体的 licenseAssignmentStates** 属性是 **licenseAssignmentState 的集合**。 它提供有关向用户分配许可证的详细信息。 详细信息包括以下信息：  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jpettere
ms.openlocfilehash: 6362737397d8f5b5c1643557bc7c834392b520ef
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720527"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="96253-105">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="96253-105">licenseAssignmentState resource type</span></span>

<span data-ttu-id="96253-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96253-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96253-107">**用户实体的 licenseAssignmentStates** 属性是 **licenseAssignmentState 的集合**。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="96253-107">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="96253-108">它提供有关向用户分配许可证的详细信息。</span><span class="sxs-lookup"><span data-stu-id="96253-108">It provides details about license assignments to a user.</span></span> <span data-ttu-id="96253-109">详细信息包括以下信息：</span><span class="sxs-lookup"><span data-stu-id="96253-109">The details includes information like:</span></span>

- <span data-ttu-id="96253-110">为用户禁用哪些计划</span><span class="sxs-lookup"><span data-stu-id="96253-110">What plans are disabled for a user</span></span>
- <span data-ttu-id="96253-111">许可证是直接分配给用户还是从组继承</span><span class="sxs-lookup"><span data-stu-id="96253-111">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="96253-112">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="96253-112">Current state of the assignment</span></span>
- <span data-ttu-id="96253-113">如果工作分配状态为 Error，则失败的错误详细信息是什么？</span><span class="sxs-lookup"><span data-stu-id="96253-113">If the assignment state is Error, what is the error detail for the failure?</span></span>


## <a name="properties"></a><span data-ttu-id="96253-114">属性</span><span class="sxs-lookup"><span data-stu-id="96253-114">Properties</span></span>
| <span data-ttu-id="96253-115">属性</span><span class="sxs-lookup"><span data-stu-id="96253-115">Property</span></span>     | <span data-ttu-id="96253-116">类型</span><span class="sxs-lookup"><span data-stu-id="96253-116">Type</span></span>   |<span data-ttu-id="96253-117">说明</span><span class="sxs-lookup"><span data-stu-id="96253-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96253-118">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="96253-118">assignedByGroup</span></span>|<span data-ttu-id="96253-119">string</span><span class="sxs-lookup"><span data-stu-id="96253-119">string</span></span>|<span data-ttu-id="96253-120">分配此许可证的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="96253-120">The id of the group that assigns this license.</span></span> <span data-ttu-id="96253-121">如果分配是直接分配的许可证，则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="96253-121">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="96253-122">只读。</span><span class="sxs-lookup"><span data-stu-id="96253-122">Read-Only.</span></span>|
|<span data-ttu-id="96253-123">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="96253-123">disabledPlans</span></span>|<span data-ttu-id="96253-124">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="96253-124">Collection(String)</span></span>|<span data-ttu-id="96253-125">在此分配中禁用的服务计划。</span><span class="sxs-lookup"><span data-stu-id="96253-125">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="96253-126">只读。</span><span class="sxs-lookup"><span data-stu-id="96253-126">Read-Only.</span></span>|
|<span data-ttu-id="96253-127">error</span><span class="sxs-lookup"><span data-stu-id="96253-127">error</span></span>|<span data-ttu-id="96253-128">String</span><span class="sxs-lookup"><span data-stu-id="96253-128">String</span></span>|<span data-ttu-id="96253-129">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="96253-129">License assignment failure error.</span></span> <span data-ttu-id="96253-130">如果许可证分配成功，则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="96253-130">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="96253-131">只读。</span><span class="sxs-lookup"><span data-stu-id="96253-131">Read-Only.</span></span> <span data-ttu-id="96253-132">可能的值 `CountViolation` `MutuallyExclusiveViolation` `DependencyViolation` ：、、、 `ProhibitedInUsageLocationViolation` `UniquenessViolation` 和 `Others` 。</span><span class="sxs-lookup"><span data-stu-id="96253-132">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="96253-133">若要详细了解如何识别和解决许可证分配错误，请参阅 [此处](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="96253-133">For more information on how to identify and resolve license assignment errors see [here](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="96253-134">skuId</span><span class="sxs-lookup"><span data-stu-id="96253-134">skuId</span></span>|<span data-ttu-id="96253-135">String</span><span class="sxs-lookup"><span data-stu-id="96253-135">String</span></span>|<span data-ttu-id="96253-136">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96253-136">The unique identifier for the SKU.</span></span> <span data-ttu-id="96253-137">只读。</span><span class="sxs-lookup"><span data-stu-id="96253-137">Read-Only.</span></span>|
|<span data-ttu-id="96253-138">state</span><span class="sxs-lookup"><span data-stu-id="96253-138">state</span></span>|<span data-ttu-id="96253-139">String</span><span class="sxs-lookup"><span data-stu-id="96253-139">String</span></span>|<span data-ttu-id="96253-140">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="96253-140">Indicate the current state of this assignment.</span></span> <span data-ttu-id="96253-141">只读。</span><span class="sxs-lookup"><span data-stu-id="96253-141">Read-Only.</span></span> <span data-ttu-id="96253-142">可能的值：Active、ActiveWithError、Disabled 和 Error。</span><span class="sxs-lookup"><span data-stu-id="96253-142">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96253-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96253-143">JSON representation</span></span>

<span data-ttu-id="96253-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96253-144">Here is a JSON representation of the resource</span></span>

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