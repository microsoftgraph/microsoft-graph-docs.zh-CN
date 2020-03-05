---
title: governanceSchedule 资源类型
description: '代表 governanceRoleAssignmentRequest 的日程安排。 对于角色分配请求，日程安排控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d52df62d0bed004d2126a775c44b92b5f285607f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497214"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="40656-104">governanceSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="40656-104">governanceSchedule resource type</span></span>

<span data-ttu-id="40656-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="40656-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40656-106">代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的日程安排。</span><span class="sxs-lookup"><span data-stu-id="40656-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="40656-107">对于角色分配请求，日程安排控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。</span><span class="sxs-lookup"><span data-stu-id="40656-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="40656-108">属性</span><span class="sxs-lookup"><span data-stu-id="40656-108">Properties</span></span>
| <span data-ttu-id="40656-109">属性</span><span class="sxs-lookup"><span data-stu-id="40656-109">Property</span></span>     | <span data-ttu-id="40656-110">类型</span><span class="sxs-lookup"><span data-stu-id="40656-110">Type</span></span>   |<span data-ttu-id="40656-111">说明</span><span class="sxs-lookup"><span data-stu-id="40656-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40656-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="40656-112">startDateTime</span></span>|<span data-ttu-id="40656-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40656-113">DateTimeOffset</span></span>|<span data-ttu-id="40656-114">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="40656-114">The start time of the role assignment.</span></span> <span data-ttu-id="40656-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="40656-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40656-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="40656-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="40656-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="40656-117">endDateTime</span></span>|<span data-ttu-id="40656-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40656-118">DateTimeOffset</span></span>|<span data-ttu-id="40656-119">角色分配的结束时间。</span><span class="sxs-lookup"><span data-stu-id="40656-119">The end time of the role assignment.</span></span> <span data-ttu-id="40656-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="40656-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40656-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="40656-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="40656-122">*注意：如果值为`null`，则表示永久分配。*</span><span class="sxs-lookup"><span data-stu-id="40656-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="40656-123">type</span><span class="sxs-lookup"><span data-stu-id="40656-123">type</span></span>|<span data-ttu-id="40656-124">String</span><span class="sxs-lookup"><span data-stu-id="40656-124">String</span></span>|<span data-ttu-id="40656-125">角色分配计划类型。</span><span class="sxs-lookup"><span data-stu-id="40656-125">The role assignment schedule type.</span></span> <span data-ttu-id="40656-126">目前`Once`仅支持。</span><span class="sxs-lookup"><span data-stu-id="40656-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="40656-127">duration</span><span class="sxs-lookup"><span data-stu-id="40656-127">duration</span></span>|<span data-ttu-id="40656-128">持续时间</span><span class="sxs-lookup"><span data-stu-id="40656-128">Duration</span></span>|<span data-ttu-id="40656-129">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="40656-129">The duration of a role assignment.</span></span> <span data-ttu-id="40656-130">它的格式为 TimeSpan。</span><span class="sxs-lookup"><span data-stu-id="40656-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40656-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40656-131">JSON representation</span></span>

<span data-ttu-id="40656-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40656-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
