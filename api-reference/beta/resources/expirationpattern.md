---
title: expirationPattern 资源类型
description: 请求计划中的过期模式可包含在访问包分配请求中，并且存在于访问包分配中。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 250c01172e44d8ea5f3cdea94a9ac61a89a11c1b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761407"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="d8865-103">expirationPattern 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8865-103">expirationPattern resource type</span></span>

<span data-ttu-id="d8865-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8865-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8865-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由想要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="d8865-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="d8865-106">此请求可包括用户希望何时进行工作分配的计划。</span><span class="sxs-lookup"><span data-stu-id="d8865-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="d8865-107">由此类请求导致的访问包分配也具有计划。</span><span class="sxs-lookup"><span data-stu-id="d8865-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="d8865-108">[requestSchedule 的过期字段](requestschedule.md)指示访问包分配应过期的时间。</span><span class="sxs-lookup"><span data-stu-id="d8865-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="d8865-109">属性</span><span class="sxs-lookup"><span data-stu-id="d8865-109">Properties</span></span>

| <span data-ttu-id="d8865-110">属性</span><span class="sxs-lookup"><span data-stu-id="d8865-110">Property</span></span>     | <span data-ttu-id="d8865-111">类型</span><span class="sxs-lookup"><span data-stu-id="d8865-111">Type</span></span>        | <span data-ttu-id="d8865-112">说明</span><span class="sxs-lookup"><span data-stu-id="d8865-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d8865-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d8865-113">endDateTime</span></span>|<span data-ttu-id="d8865-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8865-114">DateTimeOffset</span></span>|<span data-ttu-id="d8865-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d8865-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8865-116">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d8865-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="d8865-117">duration</span><span class="sxs-lookup"><span data-stu-id="d8865-117">duration</span></span>|<span data-ttu-id="d8865-118">持续时间</span><span class="sxs-lookup"><span data-stu-id="d8865-118">Duration</span></span>|<span data-ttu-id="d8865-119">请求者所需的访问持续时间。</span><span class="sxs-lookup"><span data-stu-id="d8865-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="d8865-120">如果在请求中指定，endDateTime 不应存在。</span><span class="sxs-lookup"><span data-stu-id="d8865-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="d8865-121">type</span><span class="sxs-lookup"><span data-stu-id="d8865-121">type</span></span>|<span data-ttu-id="d8865-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="d8865-122">expirationPatternType</span></span>|<span data-ttu-id="d8865-123">请求者所需的过期模式类型。</span><span class="sxs-lookup"><span data-stu-id="d8865-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="d8865-124">expirationPatternType 值</span><span class="sxs-lookup"><span data-stu-id="d8865-124">expirationPatternType values</span></span>

| <span data-ttu-id="d8865-125">成员</span><span class="sxs-lookup"><span data-stu-id="d8865-125">Member</span></span> | <span data-ttu-id="d8865-126">值</span><span class="sxs-lookup"><span data-stu-id="d8865-126">Value</span></span>| <span data-ttu-id="d8865-127">说明</span><span class="sxs-lookup"><span data-stu-id="d8865-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d8865-128">notSpecified</span><span class="sxs-lookup"><span data-stu-id="d8865-128">notSpecified</span></span>|<span data-ttu-id="d8865-129">0</span><span class="sxs-lookup"><span data-stu-id="d8865-129">0</span></span>|<span data-ttu-id="d8865-130">未指定过期计划。</span><span class="sxs-lookup"><span data-stu-id="d8865-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="d8865-131">noExpiration</span><span class="sxs-lookup"><span data-stu-id="d8865-131">noExpiration</span></span>|<span data-ttu-id="d8865-132">1</span><span class="sxs-lookup"><span data-stu-id="d8865-132">1</span></span>|<span data-ttu-id="d8865-133">请求者不希望访问过期。</span><span class="sxs-lookup"><span data-stu-id="d8865-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="d8865-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="d8865-134">afterDateTime</span></span>|<span data-ttu-id="d8865-135">2 </span><span class="sxs-lookup"><span data-stu-id="d8865-135">2</span></span>|<span data-ttu-id="d8865-136">访问将在指定的日期和时间后过期。</span><span class="sxs-lookup"><span data-stu-id="d8865-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="d8865-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="d8865-137">afterDuration</span></span>|<span data-ttu-id="d8865-138">3 </span><span class="sxs-lookup"><span data-stu-id="d8865-138">3</span></span>|<span data-ttu-id="d8865-139">访问将在相对于授予访问权限的指定持续时间后过期。</span><span class="sxs-lookup"><span data-stu-id="d8865-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8865-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8865-140">JSON representation</span></span>

<span data-ttu-id="d8865-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8865-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern"
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


