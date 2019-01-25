---
title: governanceSchedule 资源类型
description: '代表 governanceRoleAssignmentRequest 的计划。 角色分配请求，时间表控制时执行该角色分配操作，何时停止角色分配，以及如何经常角色分配操作。 '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508025"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="b7d86-104">governanceSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7d86-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7d86-105">代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的计划。</span><span class="sxs-lookup"><span data-stu-id="b7d86-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="b7d86-106">角色分配请求，时间表控制时执行该角色分配操作，何时停止角色分配，以及如何经常角色分配操作。</span><span class="sxs-lookup"><span data-stu-id="b7d86-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="b7d86-107">属性</span><span class="sxs-lookup"><span data-stu-id="b7d86-107">Properties</span></span>
| <span data-ttu-id="b7d86-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7d86-108">Property</span></span>     | <span data-ttu-id="b7d86-109">类型</span><span class="sxs-lookup"><span data-stu-id="b7d86-109">Type</span></span>   |<span data-ttu-id="b7d86-110">说明</span><span class="sxs-lookup"><span data-stu-id="b7d86-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7d86-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b7d86-111">startDateTime</span></span>|<span data-ttu-id="b7d86-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7d86-112">DateTimeOffset</span></span>|<span data-ttu-id="b7d86-113">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="b7d86-113">The start time of the role assignment.</span></span> <span data-ttu-id="b7d86-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b7d86-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b7d86-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b7d86-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b7d86-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b7d86-116">endDateTime</span></span>|<span data-ttu-id="b7d86-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7d86-117">DateTimeOffset</span></span>|<span data-ttu-id="b7d86-118">角色分配的结束时间。</span><span class="sxs-lookup"><span data-stu-id="b7d86-118">The end time of the role assignment.</span></span> <span data-ttu-id="b7d86-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b7d86-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b7d86-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b7d86-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b7d86-121">*注意： 如果值为`null`，它指示一个永久的分配。*</span><span class="sxs-lookup"><span data-stu-id="b7d86-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="b7d86-122">type</span><span class="sxs-lookup"><span data-stu-id="b7d86-122">type</span></span>|<span data-ttu-id="b7d86-123">String</span><span class="sxs-lookup"><span data-stu-id="b7d86-123">String</span></span>|<span data-ttu-id="b7d86-124">角色分配安排类型。</span><span class="sxs-lookup"><span data-stu-id="b7d86-124">The role assignment schedule type.</span></span> <span data-ttu-id="b7d86-125">仅`Once`现在支持。</span><span class="sxs-lookup"><span data-stu-id="b7d86-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="b7d86-126">duration</span><span class="sxs-lookup"><span data-stu-id="b7d86-126">duration</span></span>|<span data-ttu-id="b7d86-127">持续时间</span><span class="sxs-lookup"><span data-stu-id="b7d86-127">Duration</span></span>|<span data-ttu-id="b7d86-128">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="b7d86-128">The duration of a role assignment.</span></span> <span data-ttu-id="b7d86-129">处于 TimeSpan 的格式。</span><span class="sxs-lookup"><span data-stu-id="b7d86-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7d86-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7d86-130">JSON representation</span></span>

<span data-ttu-id="b7d86-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7d86-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
