---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
localization_priority: Normal
author: krbain
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 44af60c7d74f0a0d21a2312a19853a23cdcbe0ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135301"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="084f4-103">assignedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="084f4-103">assignedPlan resource type</span></span>

<span data-ttu-id="084f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="084f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="084f4-105">**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="084f4-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="084f4-106">属性</span><span class="sxs-lookup"><span data-stu-id="084f4-106">Properties</span></span>

| <span data-ttu-id="084f4-107">属性</span><span class="sxs-lookup"><span data-stu-id="084f4-107">Property</span></span>     | <span data-ttu-id="084f4-108">类型</span><span class="sxs-lookup"><span data-stu-id="084f4-108">Type</span></span>   |<span data-ttu-id="084f4-109">说明</span><span class="sxs-lookup"><span data-stu-id="084f4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="084f4-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="084f4-110">assignedDateTime</span></span>|<span data-ttu-id="084f4-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="084f4-111">DateTimeOffset</span></span>|<span data-ttu-id="084f4-p101">分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="084f4-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="084f4-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="084f4-115">capabilityStatus</span></span>|[<span data-ttu-id="084f4-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="084f4-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="084f4-117">功能分配的条件。</span><span class="sxs-lookup"><span data-stu-id="084f4-117">Condition of the capability assignment.</span></span> <span data-ttu-id="084f4-118">可能的值为 `Enabled` ， `Warning` ， ， `Suspended` `Deleted` 。 `LockedOut`</span><span class="sxs-lookup"><span data-stu-id="084f4-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="084f4-119">service</span><span class="sxs-lookup"><span data-stu-id="084f4-119">service</span></span>|<span data-ttu-id="084f4-120">String</span><span class="sxs-lookup"><span data-stu-id="084f4-120">String</span></span>|<span data-ttu-id="084f4-121">服务名称；例如，“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="084f4-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="084f4-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="084f4-122">servicePlanId</span></span>|<span data-ttu-id="084f4-123">Guid</span><span class="sxs-lookup"><span data-stu-id="084f4-123">Guid</span></span>|<span data-ttu-id="084f4-124">用于标识服务计划的 GUID。</span><span class="sxs-lookup"><span data-stu-id="084f4-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="084f4-125">capabilityStatus 值</span><span class="sxs-lookup"><span data-stu-id="084f4-125">capabilityStatus values</span></span>

| <span data-ttu-id="084f4-126">成员</span><span class="sxs-lookup"><span data-stu-id="084f4-126">Member</span></span> | <span data-ttu-id="084f4-127">说明</span><span class="sxs-lookup"><span data-stu-id="084f4-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="084f4-128">已启用</span><span class="sxs-lookup"><span data-stu-id="084f4-128">Enabled</span></span> | <span data-ttu-id="084f4-129">可供正常使用。</span><span class="sxs-lookup"><span data-stu-id="084f4-129">Available for normal use.</span></span> |
| <span data-ttu-id="084f4-130">警告</span><span class="sxs-lookup"><span data-stu-id="084f4-130">Warning</span></span> | <span data-ttu-id="084f4-131">可供正常使用，但位于宽限期内。</span><span class="sxs-lookup"><span data-stu-id="084f4-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="084f4-132">已暂停</span><span class="sxs-lookup"><span data-stu-id="084f4-132">Suspended</span></span> | <span data-ttu-id="084f4-133">不可用，但必须保留与该功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="084f4-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="084f4-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="084f4-134">Deleted</span></span> | <span data-ttu-id="084f4-135">不可用，并且可能会删除与该功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="084f4-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="084f4-136">LockedOut</span><span class="sxs-lookup"><span data-stu-id="084f4-136">LockedOut</span></span> | <span data-ttu-id="084f4-137">所有管理员和用户都不可用，但必须保留与该功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="084f4-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="084f4-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="084f4-138">JSON representation</span></span>

<span data-ttu-id="084f4-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="084f4-139">Here is a JSON representation of the resource</span></span>

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

