---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
localization_priority: Normal
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 182ef3239437234c74945fa37483924429f2200b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958092"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="6d530-103">assignedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d530-103">assignedPlan resource type</span></span>

<span data-ttu-id="6d530-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d530-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6d530-105">**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="6d530-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="6d530-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d530-106">Properties</span></span>

| <span data-ttu-id="6d530-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d530-107">Property</span></span>     | <span data-ttu-id="6d530-108">类型</span><span class="sxs-lookup"><span data-stu-id="6d530-108">Type</span></span>   |<span data-ttu-id="6d530-109">说明</span><span class="sxs-lookup"><span data-stu-id="6d530-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d530-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d530-110">assignedDateTime</span></span>|<span data-ttu-id="6d530-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d530-111">DateTimeOffset</span></span>|<span data-ttu-id="6d530-112">分配计划的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6d530-112">The date and time at which the plan was assigned.</span></span> <span data-ttu-id="6d530-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6d530-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d530-114">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="6d530-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="6d530-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="6d530-115">capabilityStatus</span></span>|<span data-ttu-id="6d530-116">String</span><span class="sxs-lookup"><span data-stu-id="6d530-116">String</span></span>|<span data-ttu-id="6d530-117">功能分配的条件。</span><span class="sxs-lookup"><span data-stu-id="6d530-117">Condition of the capability assignment.</span></span> <span data-ttu-id="6d530-118">可能的值为 `Enabled` `Warning` `Suspended` `Deleted` `LockedOut` 、、。</span><span class="sxs-lookup"><span data-stu-id="6d530-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> <span data-ttu-id="6d530-119">请参阅 [每个值的](#capabilitystatus-values) 详细说明。</span><span class="sxs-lookup"><span data-stu-id="6d530-119">See [a detailed description](#capabilitystatus-values) of each value.</span></span>|
|<span data-ttu-id="6d530-120">service</span><span class="sxs-lookup"><span data-stu-id="6d530-120">service</span></span>|<span data-ttu-id="6d530-121">String</span><span class="sxs-lookup"><span data-stu-id="6d530-121">String</span></span>|<span data-ttu-id="6d530-122">服务名称；例如，“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="6d530-122">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="6d530-123">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="6d530-123">servicePlanId</span></span>|<span data-ttu-id="6d530-124">Guid</span><span class="sxs-lookup"><span data-stu-id="6d530-124">Guid</span></span>|<span data-ttu-id="6d530-125">用于标识服务计划的 GUID。</span><span class="sxs-lookup"><span data-stu-id="6d530-125">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="6d530-126">capabilityStatus 值</span><span class="sxs-lookup"><span data-stu-id="6d530-126">capabilityStatus values</span></span>

| <span data-ttu-id="6d530-127">成员</span><span class="sxs-lookup"><span data-stu-id="6d530-127">Member</span></span> | <span data-ttu-id="6d530-128">说明</span><span class="sxs-lookup"><span data-stu-id="6d530-128">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="6d530-129">已启用</span><span class="sxs-lookup"><span data-stu-id="6d530-129">Enabled</span></span> | <span data-ttu-id="6d530-130">可供正常使用。</span><span class="sxs-lookup"><span data-stu-id="6d530-130">Available for normal use.</span></span> |
| <span data-ttu-id="6d530-131">警告</span><span class="sxs-lookup"><span data-stu-id="6d530-131">Warning</span></span> | <span data-ttu-id="6d530-132">可供正常使用，但位于宽限期内。</span><span class="sxs-lookup"><span data-stu-id="6d530-132">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="6d530-133">已暂停</span><span class="sxs-lookup"><span data-stu-id="6d530-133">Suspended</span></span> | <span data-ttu-id="6d530-134">不可用，但必须保留与功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="6d530-134">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="6d530-135">Deleted</span><span class="sxs-lookup"><span data-stu-id="6d530-135">Deleted</span></span> | <span data-ttu-id="6d530-136">不可用，并且可能会删除与功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="6d530-136">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="6d530-137">LockedOut</span><span class="sxs-lookup"><span data-stu-id="6d530-137">LockedOut</span></span> | <span data-ttu-id="6d530-138">所有管理员和用户都不可用，但必须保留与功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="6d530-138">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d530-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d530-139">JSON representation</span></span>

<span data-ttu-id="6d530-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d530-140">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

