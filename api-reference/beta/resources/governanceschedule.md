---
title: governanceSchedule 资源类型
description: '代表 governanceRoleAssignmentRequest 的计划。 角色分配请求，时间表控制时执行该角色分配操作，何时停止角色分配，以及如何经常角色分配操作。 '
ms.openlocfilehash: 6eff3977aa7806c975f968b8706f2e8c21e5d99e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046535"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="fac26-104">governanceSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="fac26-104">governanceSchedule resource type</span></span>

> <span data-ttu-id="fac26-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fac26-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fac26-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fac26-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fac26-107">代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的计划。</span><span class="sxs-lookup"><span data-stu-id="fac26-107">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="fac26-108">角色分配请求，时间表控制时执行该角色分配操作，何时停止角色分配，以及如何经常角色分配操作。</span><span class="sxs-lookup"><span data-stu-id="fac26-108">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="fac26-109">属性</span><span class="sxs-lookup"><span data-stu-id="fac26-109">Properties</span></span>
| <span data-ttu-id="fac26-110">属性</span><span class="sxs-lookup"><span data-stu-id="fac26-110">Property</span></span>     | <span data-ttu-id="fac26-111">类型</span><span class="sxs-lookup"><span data-stu-id="fac26-111">Type</span></span>   |<span data-ttu-id="fac26-112">说明</span><span class="sxs-lookup"><span data-stu-id="fac26-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fac26-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fac26-113">startDateTime</span></span>|<span data-ttu-id="fac26-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fac26-114">DateTimeOffset</span></span>|<span data-ttu-id="fac26-115">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="fac26-115">The start time of the role assignment.</span></span> <span data-ttu-id="fac26-116">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fac26-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fac26-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fac26-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fac26-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fac26-118">endDateTime</span></span>|<span data-ttu-id="fac26-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fac26-119">DateTimeOffset</span></span>|<span data-ttu-id="fac26-120">角色分配的结束时间。</span><span class="sxs-lookup"><span data-stu-id="fac26-120">The end time of the role assignment.</span></span> <span data-ttu-id="fac26-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fac26-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fac26-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="fac26-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fac26-123">*注意： 如果值为`null`，它指示一个永久的分配。*</span><span class="sxs-lookup"><span data-stu-id="fac26-123">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="fac26-124">type</span><span class="sxs-lookup"><span data-stu-id="fac26-124">type</span></span>|<span data-ttu-id="fac26-125">字符串</span><span class="sxs-lookup"><span data-stu-id="fac26-125">String</span></span>|<span data-ttu-id="fac26-126">角色分配安排类型。</span><span class="sxs-lookup"><span data-stu-id="fac26-126">The role assignment schedule type.</span></span> <span data-ttu-id="fac26-127">仅`Once`现在支持。</span><span class="sxs-lookup"><span data-stu-id="fac26-127">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="fac26-128">duration</span><span class="sxs-lookup"><span data-stu-id="fac26-128">duration</span></span>|<span data-ttu-id="fac26-129">Duration</span><span class="sxs-lookup"><span data-stu-id="fac26-129">Duration</span></span>|<span data-ttu-id="fac26-130">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="fac26-130">The duration of a role assignment.</span></span> <span data-ttu-id="fac26-131">处于 TimeSpan 的格式。</span><span class="sxs-lookup"><span data-stu-id="fac26-131">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fac26-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fac26-132">JSON representation</span></span>

<span data-ttu-id="fac26-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fac26-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
