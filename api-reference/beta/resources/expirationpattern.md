---
title: expirationPattern 资源类型
description: 请求计划中的过期模式可包含在访问包分配请求中，并且存在于访问包分配中。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6587d8ba410ba0240c0fd75b7c8ec37105061d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721291"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="090ec-103">expirationPattern 资源类型</span><span class="sxs-lookup"><span data-stu-id="090ec-103">expirationPattern resource type</span></span>

<span data-ttu-id="090ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="090ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="090ec-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由想要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="090ec-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="090ec-106">此请求可以包括用户希望何时进行工作分配的计划。</span><span class="sxs-lookup"><span data-stu-id="090ec-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="090ec-107">来自此类请求的访问包分配也具有计划。</span><span class="sxs-lookup"><span data-stu-id="090ec-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="090ec-108">requestSchedule 的过期 [字段](requestschedule.md) 指示访问包分配应过期的时间。</span><span class="sxs-lookup"><span data-stu-id="090ec-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="090ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="090ec-109">Properties</span></span>

| <span data-ttu-id="090ec-110">属性</span><span class="sxs-lookup"><span data-stu-id="090ec-110">Property</span></span>     | <span data-ttu-id="090ec-111">类型</span><span class="sxs-lookup"><span data-stu-id="090ec-111">Type</span></span>        | <span data-ttu-id="090ec-112">说明</span><span class="sxs-lookup"><span data-stu-id="090ec-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="090ec-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="090ec-113">endDateTime</span></span>|<span data-ttu-id="090ec-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="090ec-114">DateTimeOffset</span></span>|<span data-ttu-id="090ec-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="090ec-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="090ec-116">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="090ec-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="090ec-117">duration</span><span class="sxs-lookup"><span data-stu-id="090ec-117">duration</span></span>|<span data-ttu-id="090ec-118">持续时间</span><span class="sxs-lookup"><span data-stu-id="090ec-118">Duration</span></span>|<span data-ttu-id="090ec-119">请求者所需的访问持续时间。</span><span class="sxs-lookup"><span data-stu-id="090ec-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="090ec-120">如果在请求中指定，则 endDateTime 不应存在。</span><span class="sxs-lookup"><span data-stu-id="090ec-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="090ec-121">type</span><span class="sxs-lookup"><span data-stu-id="090ec-121">type</span></span>|<span data-ttu-id="090ec-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="090ec-122">expirationPatternType</span></span>|<span data-ttu-id="090ec-123">请求者所需的过期模式类型。</span><span class="sxs-lookup"><span data-stu-id="090ec-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="090ec-124">expirationPatternType 值</span><span class="sxs-lookup"><span data-stu-id="090ec-124">expirationPatternType values</span></span>

| <span data-ttu-id="090ec-125">成员</span><span class="sxs-lookup"><span data-stu-id="090ec-125">Member</span></span> | <span data-ttu-id="090ec-126">值</span><span class="sxs-lookup"><span data-stu-id="090ec-126">Value</span></span>| <span data-ttu-id="090ec-127">说明</span><span class="sxs-lookup"><span data-stu-id="090ec-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="090ec-128">notSpecified</span><span class="sxs-lookup"><span data-stu-id="090ec-128">notSpecified</span></span>|<span data-ttu-id="090ec-129">0</span><span class="sxs-lookup"><span data-stu-id="090ec-129">0</span></span>|<span data-ttu-id="090ec-130">未指定过期计划。</span><span class="sxs-lookup"><span data-stu-id="090ec-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="090ec-131">noExpiration</span><span class="sxs-lookup"><span data-stu-id="090ec-131">noExpiration</span></span>|<span data-ttu-id="090ec-132">1</span><span class="sxs-lookup"><span data-stu-id="090ec-132">1</span></span>|<span data-ttu-id="090ec-133">请求者不希望访问过期。</span><span class="sxs-lookup"><span data-stu-id="090ec-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="090ec-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="090ec-134">afterDateTime</span></span>|<span data-ttu-id="090ec-135">2 </span><span class="sxs-lookup"><span data-stu-id="090ec-135">2</span></span>|<span data-ttu-id="090ec-136">访问将在指定的日期和时间之后过期。</span><span class="sxs-lookup"><span data-stu-id="090ec-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="090ec-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="090ec-137">afterDuration</span></span>|<span data-ttu-id="090ec-138">3 </span><span class="sxs-lookup"><span data-stu-id="090ec-138">3</span></span>|<span data-ttu-id="090ec-139">访问将在相对于授予访问权限的指定持续时间后过期。</span><span class="sxs-lookup"><span data-stu-id="090ec-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="090ec-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="090ec-140">JSON representation</span></span>

<span data-ttu-id="090ec-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="090ec-141">The following is a JSON representation of the resource.</span></span>

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


