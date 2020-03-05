---
title: licenseAssignmentState 资源类型
description: User 实体的**licenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。 它提供了对用户的许可证分配的详细信息。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: e5b9a1687209c9d8580ef3c82bece0c31733d707
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447596"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="8bf28-104">licenseAssignmentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bf28-104">licenseAssignmentState resource type</span></span>

<span data-ttu-id="8bf28-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8bf28-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="8bf28-106">[User](user.md)实体的**LicenseAssignmentStates**属性是**licenseAssignmentState**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8bf28-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="8bf28-107">它提供了对用户的许可证分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8bf28-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="8bf28-108">详细信息包括以下信息：</span><span class="sxs-lookup"><span data-stu-id="8bf28-108">The details include information such as:</span></span>  

- <span data-ttu-id="8bf28-109">为用户禁用了哪些计划</span><span class="sxs-lookup"><span data-stu-id="8bf28-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="8bf28-110">是否将许可证直接分配给用户或从组继承。</span><span class="sxs-lookup"><span data-stu-id="8bf28-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="8bf28-111">工作分配的当前状态</span><span class="sxs-lookup"><span data-stu-id="8bf28-111">The current state of the assignment</span></span>
- <span data-ttu-id="8bf28-112">如果工作分配状态为错误，则为错误详细信息</span><span class="sxs-lookup"><span data-stu-id="8bf28-112">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="8bf28-113">属性</span><span class="sxs-lookup"><span data-stu-id="8bf28-113">Properties</span></span>
| <span data-ttu-id="8bf28-114">属性</span><span class="sxs-lookup"><span data-stu-id="8bf28-114">Property</span></span>     | <span data-ttu-id="8bf28-115">类型</span><span class="sxs-lookup"><span data-stu-id="8bf28-115">Type</span></span>   |<span data-ttu-id="8bf28-116">说明</span><span class="sxs-lookup"><span data-stu-id="8bf28-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bf28-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="8bf28-117">assignedByGroup</span></span>|<span data-ttu-id="8bf28-118">string</span><span class="sxs-lookup"><span data-stu-id="8bf28-118">string</span></span>|<span data-ttu-id="8bf28-119">分配此许可证的组的 id。</span><span class="sxs-lookup"><span data-stu-id="8bf28-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="8bf28-120">如果分配是直接分配的许可证，则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="8bf28-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="8bf28-121">只读。</span><span class="sxs-lookup"><span data-stu-id="8bf28-121">Read-Only.</span></span>|
|<span data-ttu-id="8bf28-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="8bf28-122">disabledPlans</span></span>|<span data-ttu-id="8bf28-123">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="8bf28-123">Collection(String)</span></span>|<span data-ttu-id="8bf28-124">此工作分配中禁用的服务计划。</span><span class="sxs-lookup"><span data-stu-id="8bf28-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="8bf28-125">只读。</span><span class="sxs-lookup"><span data-stu-id="8bf28-125">Read-Only.</span></span>|
|<span data-ttu-id="8bf28-126">error</span><span class="sxs-lookup"><span data-stu-id="8bf28-126">error</span></span>|<span data-ttu-id="8bf28-127">String</span><span class="sxs-lookup"><span data-stu-id="8bf28-127">String</span></span>|<span data-ttu-id="8bf28-128">许可证分配失败错误。</span><span class="sxs-lookup"><span data-stu-id="8bf28-128">License assignment failure error.</span></span> <span data-ttu-id="8bf28-129">如果许可证分配成功，则此字段将为 Null。</span><span class="sxs-lookup"><span data-stu-id="8bf28-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="8bf28-130">只读。</span><span class="sxs-lookup"><span data-stu-id="8bf28-130">Read-Only.</span></span> <span data-ttu-id="8bf28-131">可能的值`CountViolation`： `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、和`Others`。</span><span class="sxs-lookup"><span data-stu-id="8bf28-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="8bf28-132">有关如何识别和解决许可证分配错误的详细信息，请参阅[此处](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="8bf28-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="8bf28-133">skuId</span><span class="sxs-lookup"><span data-stu-id="8bf28-133">skuId</span></span>|<span data-ttu-id="8bf28-134">String</span><span class="sxs-lookup"><span data-stu-id="8bf28-134">String</span></span>|<span data-ttu-id="8bf28-135">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8bf28-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="8bf28-136">只读。</span><span class="sxs-lookup"><span data-stu-id="8bf28-136">Read-Only.</span></span>|
|<span data-ttu-id="8bf28-137">state</span><span class="sxs-lookup"><span data-stu-id="8bf28-137">state</span></span>|<span data-ttu-id="8bf28-138">String</span><span class="sxs-lookup"><span data-stu-id="8bf28-138">String</span></span>|<span data-ttu-id="8bf28-139">指示此工作分配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="8bf28-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="8bf28-140">只读。</span><span class="sxs-lookup"><span data-stu-id="8bf28-140">Read-Only.</span></span> <span data-ttu-id="8bf28-141">可能的值： Active、ActiveWithError、Disabled 和 Error。</span><span class="sxs-lookup"><span data-stu-id="8bf28-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bf28-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bf28-142">JSON representation</span></span>

<span data-ttu-id="8bf28-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bf28-143">The following is a JSON representation of the resource.</span></span>

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
