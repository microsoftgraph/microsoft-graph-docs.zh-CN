---
title: licenseAssignmentState 资源类型
description: 用户实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。 为用户提供有关许可证分配的详细信息。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649383"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="c3038-104">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3038-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="c3038-105">[用户](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c3038-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="c3038-106">为用户提供有关许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c3038-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="c3038-107">详细信息包括以下信息：</span><span class="sxs-lookup"><span data-stu-id="c3038-107">The details include information such as:</span></span>  

 - <span data-ttu-id="c3038-108">哪些计划将被禁用的用户</span><span class="sxs-lookup"><span data-stu-id="c3038-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="c3038-109">是否许可证已直接分配给用户或从组继承</span><span class="sxs-lookup"><span data-stu-id="c3038-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="c3038-110">当前状态的工作分配</span><span class="sxs-lookup"><span data-stu-id="c3038-110">The current state of the assignment</span></span>
 - <span data-ttu-id="c3038-111">如果工作分配状态错误的错误详细信息</span><span class="sxs-lookup"><span data-stu-id="c3038-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="c3038-112">属性</span><span class="sxs-lookup"><span data-stu-id="c3038-112">Properties</span></span>
| <span data-ttu-id="c3038-113">属性</span><span class="sxs-lookup"><span data-stu-id="c3038-113">Property</span></span>     | <span data-ttu-id="c3038-114">类型</span><span class="sxs-lookup"><span data-stu-id="c3038-114">Type</span></span>   |<span data-ttu-id="c3038-115">说明</span><span class="sxs-lookup"><span data-stu-id="c3038-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3038-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="c3038-116">assignedByGroup</span></span>|<span data-ttu-id="c3038-117">string</span><span class="sxs-lookup"><span data-stu-id="c3038-117">string</span></span>|<span data-ttu-id="c3038-118">分配此许可证的组 id。</span><span class="sxs-lookup"><span data-stu-id="c3038-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="c3038-119">如果工作分配为直接分配许可证，此字段为 Null。</span><span class="sxs-lookup"><span data-stu-id="c3038-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="c3038-120">只读。</span><span class="sxs-lookup"><span data-stu-id="c3038-120">Read-Only.</span></span>|
|<span data-ttu-id="c3038-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="c3038-121">disabledPlans</span></span>|<span data-ttu-id="c3038-122">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="c3038-122">Collection(String)</span></span>|<span data-ttu-id="c3038-123">此工作分配中禁用服务计划。</span><span class="sxs-lookup"><span data-stu-id="c3038-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="c3038-124">只读。</span><span class="sxs-lookup"><span data-stu-id="c3038-124">Read-Only.</span></span>|
|<span data-ttu-id="c3038-125">error</span><span class="sxs-lookup"><span data-stu-id="c3038-125">error</span></span>|<span data-ttu-id="c3038-126">String</span><span class="sxs-lookup"><span data-stu-id="c3038-126">String</span></span>|<span data-ttu-id="c3038-127">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="c3038-127">License assignment failure error.</span></span> <span data-ttu-id="c3038-128">如果已成功分配许可证，此字段为 Null。</span><span class="sxs-lookup"><span data-stu-id="c3038-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="c3038-129">只读。</span><span class="sxs-lookup"><span data-stu-id="c3038-129">Read-Only.</span></span> <span data-ttu-id="c3038-130">可能的值： `CountViolation`， `MutuallyExclusiveViolation`， `DependencyViolation`， `ProhibitedInUsageLocationViolation`， `UniquenessViolation`，和`Others`。</span><span class="sxs-lookup"><span data-stu-id="c3038-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="c3038-131">有关详细信息如何确定和解决许可证分配错误请参见[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="c3038-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="c3038-132">skuId</span><span class="sxs-lookup"><span data-stu-id="c3038-132">skuId</span></span>|<span data-ttu-id="c3038-133">String</span><span class="sxs-lookup"><span data-stu-id="c3038-133">String</span></span>|<span data-ttu-id="c3038-134">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c3038-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="c3038-135">只读。</span><span class="sxs-lookup"><span data-stu-id="c3038-135">Read-Only.</span></span>|
|<span data-ttu-id="c3038-136">state</span><span class="sxs-lookup"><span data-stu-id="c3038-136">state</span></span>|<span data-ttu-id="c3038-137">String</span><span class="sxs-lookup"><span data-stu-id="c3038-137">String</span></span>|<span data-ttu-id="c3038-138">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c3038-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="c3038-139">只读。</span><span class="sxs-lookup"><span data-stu-id="c3038-139">Read-Only.</span></span> <span data-ttu-id="c3038-140">可能的值： 活动、 ActiveWithError、 已禁用和错误。</span><span class="sxs-lookup"><span data-stu-id="c3038-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3038-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3038-141">JSON representation</span></span>

<span data-ttu-id="c3038-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3038-142">The following is a JSON representation of the resource.</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
