---
title: licenseAssignmentState 资源类型
description: '用户实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 为用户提供有关许可证分配的详细信息。 详细信息包括类似的信息：  '
ms.openlocfilehash: 4e7101acc756a845913a081368b79242834ef3bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047225"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="0909b-105">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0909b-105">licenseAssignmentState resource type</span></span>

> <span data-ttu-id="0909b-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0909b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0909b-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0909b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0909b-108">[用户](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。</span><span class="sxs-lookup"><span data-stu-id="0909b-108">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="0909b-109">为用户提供有关许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0909b-109">It provides details about license assignments to a user.</span></span> <span data-ttu-id="0909b-110">详细信息包括类似的信息：</span><span class="sxs-lookup"><span data-stu-id="0909b-110">The details includes information like:</span></span>  

 - <span data-ttu-id="0909b-111">哪些计划将被禁用的用户</span><span class="sxs-lookup"><span data-stu-id="0909b-111">What plans are disabled for a user</span></span>
 - <span data-ttu-id="0909b-112">是否许可证已直接分配给用户或从组继承</span><span class="sxs-lookup"><span data-stu-id="0909b-112">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="0909b-113">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="0909b-113">Current state of the assignment</span></span>
 - <span data-ttu-id="0909b-114">如果工作分配状态错误，什么是失败的错误详细信息？</span><span class="sxs-lookup"><span data-stu-id="0909b-114">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="0909b-115">属性</span><span class="sxs-lookup"><span data-stu-id="0909b-115">Properties</span></span>
| <span data-ttu-id="0909b-116">属性</span><span class="sxs-lookup"><span data-stu-id="0909b-116">Property</span></span>     | <span data-ttu-id="0909b-117">类型</span><span class="sxs-lookup"><span data-stu-id="0909b-117">Type</span></span>   |<span data-ttu-id="0909b-118">说明</span><span class="sxs-lookup"><span data-stu-id="0909b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0909b-119">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="0909b-119">assignedByGroup</span></span>|<span data-ttu-id="0909b-120">string</span><span class="sxs-lookup"><span data-stu-id="0909b-120">string</span></span>|<span data-ttu-id="0909b-121">分配此许可证的组 id。</span><span class="sxs-lookup"><span data-stu-id="0909b-121">The id of the group that assigns this license.</span></span> <span data-ttu-id="0909b-122">如果工作分配为直接分配许可证，此字段为 Null。</span><span class="sxs-lookup"><span data-stu-id="0909b-122">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="0909b-123">只读。</span><span class="sxs-lookup"><span data-stu-id="0909b-123">Read-Only.</span></span>|
|<span data-ttu-id="0909b-124">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="0909b-124">disabledPlans</span></span>|<span data-ttu-id="0909b-125">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="0909b-125">Collection(String)</span></span>|<span data-ttu-id="0909b-126">此工作分配中禁用服务计划。</span><span class="sxs-lookup"><span data-stu-id="0909b-126">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="0909b-127">只读。</span><span class="sxs-lookup"><span data-stu-id="0909b-127">Read-Only.</span></span>|
|<span data-ttu-id="0909b-128">error</span><span class="sxs-lookup"><span data-stu-id="0909b-128">error</span></span>|<span data-ttu-id="0909b-129">字符串</span><span class="sxs-lookup"><span data-stu-id="0909b-129">String</span></span>|<span data-ttu-id="0909b-130">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="0909b-130">License assignment failure error.</span></span> <span data-ttu-id="0909b-131">如果已成功分配许可证，此字段为 Null。</span><span class="sxs-lookup"><span data-stu-id="0909b-131">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="0909b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="0909b-132">Read-Only.</span></span> <span data-ttu-id="0909b-133">可能的值： `CountViolation`， `MutuallyExclusiveViolation`， `DependencyViolation`， `ProhibitedInUsageLocationViolation`， `UniquenessViolation`，和`Others`。</span><span class="sxs-lookup"><span data-stu-id="0909b-133">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="0909b-134">有关详细信息如何确定和解决许可证分配错误请参见[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="0909b-134">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="0909b-135">skuId</span><span class="sxs-lookup"><span data-stu-id="0909b-135">skuId</span></span>|<span data-ttu-id="0909b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="0909b-136">String</span></span>|<span data-ttu-id="0909b-137">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0909b-137">The unique identifier for the SKU.</span></span> <span data-ttu-id="0909b-138">只读。</span><span class="sxs-lookup"><span data-stu-id="0909b-138">Read-Only.</span></span>|
|<span data-ttu-id="0909b-139">状态</span><span class="sxs-lookup"><span data-stu-id="0909b-139">state</span></span>|<span data-ttu-id="0909b-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0909b-140">String</span></span>|<span data-ttu-id="0909b-141">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0909b-141">Indicate the current state of this assignment.</span></span> <span data-ttu-id="0909b-142">只读。</span><span class="sxs-lookup"><span data-stu-id="0909b-142">Read-Only.</span></span> <span data-ttu-id="0909b-143">可能的值： 活动、 ActiveWithError、 已禁用和错误。</span><span class="sxs-lookup"><span data-stu-id="0909b-143">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0909b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0909b-144">JSON representation</span></span>

<span data-ttu-id="0909b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0909b-145">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```