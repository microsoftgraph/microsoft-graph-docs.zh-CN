---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: jpettere
ms.openlocfilehash: ddb13f656eda6e17e037a7bcae06b33b41260f8f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721829"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="cc20b-103">assignedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc20b-103">assignedPlan resource type</span></span>

<span data-ttu-id="cc20b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc20b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc20b-105">**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="cc20b-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="cc20b-106">属性</span><span class="sxs-lookup"><span data-stu-id="cc20b-106">Properties</span></span>

| <span data-ttu-id="cc20b-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc20b-107">Property</span></span>     | <span data-ttu-id="cc20b-108">类型</span><span class="sxs-lookup"><span data-stu-id="cc20b-108">Type</span></span>   |<span data-ttu-id="cc20b-109">说明</span><span class="sxs-lookup"><span data-stu-id="cc20b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc20b-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc20b-110">assignedDateTime</span></span>|<span data-ttu-id="cc20b-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc20b-111">DateTimeOffset</span></span>|<span data-ttu-id="cc20b-112">分配计划的日期和时间；例如：2013-01-02T19:32:30Z。</span><span class="sxs-lookup"><span data-stu-id="cc20b-112">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z.</span></span> <span data-ttu-id="cc20b-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="cc20b-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc20b-114">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="cc20b-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="cc20b-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="cc20b-115">capabilityStatus</span></span>|[<span data-ttu-id="cc20b-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="cc20b-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="cc20b-117">功能分配的条件。</span><span class="sxs-lookup"><span data-stu-id="cc20b-117">Condition of the capability assignment.</span></span> <span data-ttu-id="cc20b-118">可能的值是 `Enabled` ， `Warning` ， ， `Suspended` `Deleted` `LockedOut` 。</span><span class="sxs-lookup"><span data-stu-id="cc20b-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="cc20b-119">service</span><span class="sxs-lookup"><span data-stu-id="cc20b-119">service</span></span>|<span data-ttu-id="cc20b-120">String</span><span class="sxs-lookup"><span data-stu-id="cc20b-120">String</span></span>|<span data-ttu-id="cc20b-121">服务名称；例如，“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="cc20b-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="cc20b-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="cc20b-122">servicePlanId</span></span>|<span data-ttu-id="cc20b-123">Guid</span><span class="sxs-lookup"><span data-stu-id="cc20b-123">Guid</span></span>|<span data-ttu-id="cc20b-124">用于标识服务计划的 GUID。</span><span class="sxs-lookup"><span data-stu-id="cc20b-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="cc20b-125">capabilityStatus 值</span><span class="sxs-lookup"><span data-stu-id="cc20b-125">capabilityStatus values</span></span>

| <span data-ttu-id="cc20b-126">成员</span><span class="sxs-lookup"><span data-stu-id="cc20b-126">Member</span></span> | <span data-ttu-id="cc20b-127">说明</span><span class="sxs-lookup"><span data-stu-id="cc20b-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="cc20b-128">已启用</span><span class="sxs-lookup"><span data-stu-id="cc20b-128">Enabled</span></span> | <span data-ttu-id="cc20b-129">可供正常使用。</span><span class="sxs-lookup"><span data-stu-id="cc20b-129">Available for normal use.</span></span> |
| <span data-ttu-id="cc20b-130">警告</span><span class="sxs-lookup"><span data-stu-id="cc20b-130">Warning</span></span> | <span data-ttu-id="cc20b-131">可供正常使用，但位于宽限期内。</span><span class="sxs-lookup"><span data-stu-id="cc20b-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="cc20b-132">已暂停</span><span class="sxs-lookup"><span data-stu-id="cc20b-132">Suspended</span></span> | <span data-ttu-id="cc20b-133">不可用，但必须保留与该功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="cc20b-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="cc20b-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="cc20b-134">Deleted</span></span> | <span data-ttu-id="cc20b-135">不可用，并且可能会删除与该功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="cc20b-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="cc20b-136">LockedOut</span><span class="sxs-lookup"><span data-stu-id="cc20b-136">LockedOut</span></span> | <span data-ttu-id="cc20b-137">所有管理员和用户均不可用，但必须保留与该功能关联的任何数据。</span><span class="sxs-lookup"><span data-stu-id="cc20b-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc20b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc20b-138">JSON representation</span></span>

<span data-ttu-id="cc20b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc20b-139">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


