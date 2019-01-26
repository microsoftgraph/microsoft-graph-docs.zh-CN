---
title: licenseAssignmentState 资源类型
description: '用户实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 为用户提供有关许可证分配的详细信息。 详细信息包括类似的信息：  '
localization_priority: Normal
ms.openlocfilehash: f2f905baaba4dddd65266ffafab44febe7a61139
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575179"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="6fc25-105">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fc25-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc25-106">[用户](user.md)实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。</span><span class="sxs-lookup"><span data-stu-id="6fc25-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="6fc25-107">为用户提供有关许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fc25-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="6fc25-108">详细信息包括类似的信息：</span><span class="sxs-lookup"><span data-stu-id="6fc25-108">The details includes information like:</span></span>  

 - <span data-ttu-id="6fc25-109">哪些计划将被禁用的用户</span><span class="sxs-lookup"><span data-stu-id="6fc25-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="6fc25-110">是否许可证已直接分配给用户或从组继承</span><span class="sxs-lookup"><span data-stu-id="6fc25-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="6fc25-111">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="6fc25-111">Current state of the assignment</span></span>
 - <span data-ttu-id="6fc25-112">如果工作分配状态错误，什么是失败的错误详细信息？</span><span class="sxs-lookup"><span data-stu-id="6fc25-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="6fc25-113">属性</span><span class="sxs-lookup"><span data-stu-id="6fc25-113">Properties</span></span>
| <span data-ttu-id="6fc25-114">属性</span><span class="sxs-lookup"><span data-stu-id="6fc25-114">Property</span></span>     | <span data-ttu-id="6fc25-115">类型</span><span class="sxs-lookup"><span data-stu-id="6fc25-115">Type</span></span>   |<span data-ttu-id="6fc25-116">说明</span><span class="sxs-lookup"><span data-stu-id="6fc25-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fc25-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="6fc25-117">assignedByGroup</span></span>|<span data-ttu-id="6fc25-118">string</span><span class="sxs-lookup"><span data-stu-id="6fc25-118">string</span></span>|<span data-ttu-id="6fc25-119">分配此许可证的组 id。</span><span class="sxs-lookup"><span data-stu-id="6fc25-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="6fc25-120">如果工作分配为直接分配许可证，此字段为 Null。</span><span class="sxs-lookup"><span data-stu-id="6fc25-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="6fc25-121">只读。</span><span class="sxs-lookup"><span data-stu-id="6fc25-121">Read-Only.</span></span>|
|<span data-ttu-id="6fc25-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="6fc25-122">disabledPlans</span></span>| <span data-ttu-id="6fc25-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="6fc25-123">String collection</span></span> |<span data-ttu-id="6fc25-124">此工作分配中禁用服务计划。</span><span class="sxs-lookup"><span data-stu-id="6fc25-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="6fc25-125">只读。</span><span class="sxs-lookup"><span data-stu-id="6fc25-125">Read-Only.</span></span>|
|<span data-ttu-id="6fc25-126">error</span><span class="sxs-lookup"><span data-stu-id="6fc25-126">error</span></span>|<span data-ttu-id="6fc25-127">String</span><span class="sxs-lookup"><span data-stu-id="6fc25-127">String</span></span>|<span data-ttu-id="6fc25-128">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="6fc25-128">License assignment failure error.</span></span> <span data-ttu-id="6fc25-129">如果已成功分配许可证，此字段为 Null。</span><span class="sxs-lookup"><span data-stu-id="6fc25-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="6fc25-130">只读。</span><span class="sxs-lookup"><span data-stu-id="6fc25-130">Read-Only.</span></span> <span data-ttu-id="6fc25-131">可能的值： `CountViolation`， `MutuallyExclusiveViolation`， `DependencyViolation`， `ProhibitedInUsageLocationViolation`， `UniquenessViolation`，和`Others`。</span><span class="sxs-lookup"><span data-stu-id="6fc25-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="6fc25-132">有关详细信息如何确定和解决许可证分配错误请参见[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="6fc25-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="6fc25-133">skuId</span><span class="sxs-lookup"><span data-stu-id="6fc25-133">skuId</span></span>|<span data-ttu-id="6fc25-134">String</span><span class="sxs-lookup"><span data-stu-id="6fc25-134">String</span></span>|<span data-ttu-id="6fc25-135">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6fc25-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="6fc25-136">只读。</span><span class="sxs-lookup"><span data-stu-id="6fc25-136">Read-Only.</span></span>|
|<span data-ttu-id="6fc25-137">state</span><span class="sxs-lookup"><span data-stu-id="6fc25-137">state</span></span>|<span data-ttu-id="6fc25-138">String</span><span class="sxs-lookup"><span data-stu-id="6fc25-138">String</span></span>|<span data-ttu-id="6fc25-139">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="6fc25-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="6fc25-140">只读。</span><span class="sxs-lookup"><span data-stu-id="6fc25-140">Read-Only.</span></span> <span data-ttu-id="6fc25-141">可能的值： 活动、 ActiveWithError、 已禁用和错误。</span><span class="sxs-lookup"><span data-stu-id="6fc25-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc25-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fc25-142">JSON representation</span></span>

<span data-ttu-id="6fc25-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc25-143">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
