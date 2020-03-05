---
title: licenseAssignmentState 资源类型
description: 'User 实体的**licenseAssignmentStates**属性是**licenseAssignmentState**的集合。 它提供了对用户的许可证分配的详细信息。 详细信息包括如下信息：  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a9b98e9bc4fc86754982bb3711dd05240b158eef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522979"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="8b0d7-105">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b0d7-105">licenseAssignmentState resource type</span></span>

<span data-ttu-id="8b0d7-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8b0d7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b0d7-107">[User](user.md)实体的**LicenseAssignmentStates**属性是**licenseAssignmentState**的集合。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-107">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="8b0d7-108">它提供了对用户的许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-108">It provides details about license assignments to a user.</span></span> <span data-ttu-id="8b0d7-109">详细信息包括如下信息：</span><span class="sxs-lookup"><span data-stu-id="8b0d7-109">The details includes information like:</span></span>  

- <span data-ttu-id="8b0d7-110">为用户禁用了哪些计划</span><span class="sxs-lookup"><span data-stu-id="8b0d7-110">What plans are disabled for a user</span></span>
- <span data-ttu-id="8b0d7-111">是否将许可证直接分配给用户或从组继承。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-111">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="8b0d7-112">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="8b0d7-112">Current state of the assignment</span></span>
- <span data-ttu-id="8b0d7-113">如果工作分配状态为 "错误"，则失败的错误详细信息是什么？</span><span class="sxs-lookup"><span data-stu-id="8b0d7-113">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="8b0d7-114">属性</span><span class="sxs-lookup"><span data-stu-id="8b0d7-114">Properties</span></span>
| <span data-ttu-id="8b0d7-115">属性</span><span class="sxs-lookup"><span data-stu-id="8b0d7-115">Property</span></span>     | <span data-ttu-id="8b0d7-116">类型</span><span class="sxs-lookup"><span data-stu-id="8b0d7-116">Type</span></span>   |<span data-ttu-id="8b0d7-117">说明</span><span class="sxs-lookup"><span data-stu-id="8b0d7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b0d7-118">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="8b0d7-118">assignedByGroup</span></span>|<span data-ttu-id="8b0d7-119">string</span><span class="sxs-lookup"><span data-stu-id="8b0d7-119">string</span></span>|<span data-ttu-id="8b0d7-120">分配此许可证的组的 id。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-120">The id of the group that assigns this license.</span></span> <span data-ttu-id="8b0d7-121">如果分配是直接分配的许可证，则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-121">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="8b0d7-122">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-122">Read-Only.</span></span>|
|<span data-ttu-id="8b0d7-123">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="8b0d7-123">disabledPlans</span></span>|<span data-ttu-id="8b0d7-124">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="8b0d7-124">Collection(String)</span></span>|<span data-ttu-id="8b0d7-125">此工作分配中禁用的服务计划。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-125">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="8b0d7-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-126">Read-Only.</span></span>|
|<span data-ttu-id="8b0d7-127">error</span><span class="sxs-lookup"><span data-stu-id="8b0d7-127">error</span></span>|<span data-ttu-id="8b0d7-128">String</span><span class="sxs-lookup"><span data-stu-id="8b0d7-128">String</span></span>|<span data-ttu-id="8b0d7-129">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-129">License assignment failure error.</span></span> <span data-ttu-id="8b0d7-130">如果许可证分配成功，则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-130">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="8b0d7-131">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-131">Read-Only.</span></span> <span data-ttu-id="8b0d7-132">可能的值`CountViolation`： `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、和`Others`。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-132">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="8b0d7-133">有关如何识别和解决许可证分配错误的详细信息，请参阅[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-133">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="8b0d7-134">skuId</span><span class="sxs-lookup"><span data-stu-id="8b0d7-134">skuId</span></span>|<span data-ttu-id="8b0d7-135">String</span><span class="sxs-lookup"><span data-stu-id="8b0d7-135">String</span></span>|<span data-ttu-id="8b0d7-136">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-136">The unique identifier for the SKU.</span></span> <span data-ttu-id="8b0d7-137">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-137">Read-Only.</span></span>|
|<span data-ttu-id="8b0d7-138">state</span><span class="sxs-lookup"><span data-stu-id="8b0d7-138">state</span></span>|<span data-ttu-id="8b0d7-139">String</span><span class="sxs-lookup"><span data-stu-id="8b0d7-139">String</span></span>|<span data-ttu-id="8b0d7-140">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-140">Indicate the current state of this assignment.</span></span> <span data-ttu-id="8b0d7-141">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-141">Read-Only.</span></span> <span data-ttu-id="8b0d7-142">可能的值： Active、ActiveWithError、Disabled 和 Error。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-142">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b0d7-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b0d7-143">JSON representation</span></span>

<span data-ttu-id="8b0d7-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b0d7-144">Here is a JSON representation of the resource</span></span>

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
