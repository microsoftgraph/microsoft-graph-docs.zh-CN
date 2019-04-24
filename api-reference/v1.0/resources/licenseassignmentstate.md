---
title: licenseAssignmentState 资源类型
description: user 实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。 它提供了对用户的许可证分配的详细信息。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585144"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="50de8-104">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="50de8-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="50de8-105">[user](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="50de8-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="50de8-106">它提供了对用户的许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="50de8-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="50de8-107">详细信息包括以下信息:</span><span class="sxs-lookup"><span data-stu-id="50de8-107">The details include information such as:</span></span>  

 - <span data-ttu-id="50de8-108">为用户禁用了哪些计划</span><span class="sxs-lookup"><span data-stu-id="50de8-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="50de8-109">是否将许可证直接分配给用户或从组继承。</span><span class="sxs-lookup"><span data-stu-id="50de8-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="50de8-110">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="50de8-110">The current state of the assignment</span></span>
 - <span data-ttu-id="50de8-111">如果工作分配状态为错误, 则为错误详细信息</span><span class="sxs-lookup"><span data-stu-id="50de8-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="50de8-112">属性</span><span class="sxs-lookup"><span data-stu-id="50de8-112">Properties</span></span>
| <span data-ttu-id="50de8-113">属性</span><span class="sxs-lookup"><span data-stu-id="50de8-113">Property</span></span>     | <span data-ttu-id="50de8-114">类型</span><span class="sxs-lookup"><span data-stu-id="50de8-114">Type</span></span>   |<span data-ttu-id="50de8-115">说明</span><span class="sxs-lookup"><span data-stu-id="50de8-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50de8-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="50de8-116">assignedByGroup</span></span>|<span data-ttu-id="50de8-117">字符串</span><span class="sxs-lookup"><span data-stu-id="50de8-117">string</span></span>|<span data-ttu-id="50de8-118">分配此许可证的组的 id。</span><span class="sxs-lookup"><span data-stu-id="50de8-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="50de8-119">如果分配是直接分配的许可证, 则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="50de8-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="50de8-120">只读。</span><span class="sxs-lookup"><span data-stu-id="50de8-120">Read-Only.</span></span>|
|<span data-ttu-id="50de8-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="50de8-121">disabledPlans</span></span>|<span data-ttu-id="50de8-122">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="50de8-122">Collection(String)</span></span>|<span data-ttu-id="50de8-123">此工作分配中禁用的服务计划。</span><span class="sxs-lookup"><span data-stu-id="50de8-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="50de8-124">只读。</span><span class="sxs-lookup"><span data-stu-id="50de8-124">Read-Only.</span></span>|
|<span data-ttu-id="50de8-125">error</span><span class="sxs-lookup"><span data-stu-id="50de8-125">error</span></span>|<span data-ttu-id="50de8-126">字符串</span><span class="sxs-lookup"><span data-stu-id="50de8-126">String</span></span>|<span data-ttu-id="50de8-127">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="50de8-127">License assignment failure error.</span></span> <span data-ttu-id="50de8-128">如果许可证分配成功, 则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="50de8-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="50de8-129">只读。</span><span class="sxs-lookup"><span data-stu-id="50de8-129">Read-Only.</span></span> <span data-ttu-id="50de8-130">可能的值`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、和`Others`。</span><span class="sxs-lookup"><span data-stu-id="50de8-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="50de8-131">有关如何识别和解决许可证分配错误的详细信息, 请参阅[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="50de8-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="50de8-132">skuId</span><span class="sxs-lookup"><span data-stu-id="50de8-132">skuId</span></span>|<span data-ttu-id="50de8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="50de8-133">String</span></span>|<span data-ttu-id="50de8-134">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="50de8-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="50de8-135">只读。</span><span class="sxs-lookup"><span data-stu-id="50de8-135">Read-Only.</span></span>|
|<span data-ttu-id="50de8-136">state</span><span class="sxs-lookup"><span data-stu-id="50de8-136">state</span></span>|<span data-ttu-id="50de8-137">String</span><span class="sxs-lookup"><span data-stu-id="50de8-137">String</span></span>|<span data-ttu-id="50de8-138">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="50de8-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="50de8-139">只读。</span><span class="sxs-lookup"><span data-stu-id="50de8-139">Read-Only.</span></span> <span data-ttu-id="50de8-140">可能的值: Active、ActiveWithError、Disabled 和 Error。</span><span class="sxs-lookup"><span data-stu-id="50de8-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50de8-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50de8-141">JSON representation</span></span>

<span data-ttu-id="50de8-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50de8-142">The following is a JSON representation of the resource.</span></span>

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
