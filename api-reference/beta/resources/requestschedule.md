---
title: requestSchedule 资源类型
description: 请求计划可包含在访问包分配请求中，并且存在于访问包分配中。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 33abd221d22d37cc58bcf3770b4e28fa78b77064
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718462"
---
# <a name="requestschedule-resource-type"></a><span data-ttu-id="4bce9-103">requestSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bce9-103">requestSchedule resource type</span></span>

<span data-ttu-id="4bce9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bce9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bce9-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由想要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="4bce9-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="4bce9-106">此请求可以包括用户希望何时进行工作分配的计划。</span><span class="sxs-lookup"><span data-stu-id="4bce9-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="4bce9-107">来自此类请求的访问包分配也具有计划。</span><span class="sxs-lookup"><span data-stu-id="4bce9-107">An access package assignment that results from such a request also has a schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="4bce9-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bce9-108">Properties</span></span>

| <span data-ttu-id="4bce9-109">属性</span><span class="sxs-lookup"><span data-stu-id="4bce9-109">Property</span></span>     | <span data-ttu-id="4bce9-110">类型</span><span class="sxs-lookup"><span data-stu-id="4bce9-110">Type</span></span>        | <span data-ttu-id="4bce9-111">说明</span><span class="sxs-lookup"><span data-stu-id="4bce9-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4bce9-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4bce9-112">startDateTime</span></span>|<span data-ttu-id="4bce9-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bce9-113">DateTimeOffset</span></span>|<span data-ttu-id="4bce9-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4bce9-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4bce9-115">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="4bce9-115">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="4bce9-116">expiration</span><span class="sxs-lookup"><span data-stu-id="4bce9-116">expiration</span></span>|[<span data-ttu-id="4bce9-117">expirationPattern</span><span class="sxs-lookup"><span data-stu-id="4bce9-117">expirationPattern</span></span>](expirationpattern.md)|<span data-ttu-id="4bce9-118">访问应过期的时间。</span><span class="sxs-lookup"><span data-stu-id="4bce9-118">When the access should expire.</span></span>|
|<span data-ttu-id="4bce9-119">recurrence</span><span class="sxs-lookup"><span data-stu-id="4bce9-119">recurrence</span></span>|[<span data-ttu-id="4bce9-120">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4bce9-120">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="4bce9-121">对于定期访问。</span><span class="sxs-lookup"><span data-stu-id="4bce9-121">For recurring access.</span></span> <span data-ttu-id="4bce9-122">目前未使用。</span><span class="sxs-lookup"><span data-stu-id="4bce9-122">Not used at present.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bce9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bce9-123">JSON representation</span></span>

<span data-ttu-id="4bce9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bce9-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule"
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
        "endDateTime": "2020-09-10T23:06:53.307Z",
        "type": "afterDateTime"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


