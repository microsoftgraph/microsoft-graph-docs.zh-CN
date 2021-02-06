---
title: governanceSchedule 资源类型
description: '表示 governanceRoleAssignmentRequest 的计划。 对于角色分配，计划控制何时执行 角色分配 操作、何时停止 角色分配 以及执行 角色分配 操作的频率。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e7b444b1daa45daf3228476fb48a38be4e7bb2b2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132669"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="fd556-104">governanceSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd556-104">governanceSchedule resource type</span></span>

<span data-ttu-id="fd556-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd556-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd556-106">表示 [governanceRoleAssignmentRequest 的计划](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="fd556-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="fd556-107">对于角色分配，计划控制何时执行 角色分配 操作、何时停止 角色分配 以及执行 角色分配 操作的频率。</span><span class="sxs-lookup"><span data-stu-id="fd556-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span>



## <a name="properties"></a><span data-ttu-id="fd556-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd556-108">Properties</span></span>
| <span data-ttu-id="fd556-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd556-109">Property</span></span>     | <span data-ttu-id="fd556-110">类型</span><span class="sxs-lookup"><span data-stu-id="fd556-110">Type</span></span>   |<span data-ttu-id="fd556-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd556-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd556-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fd556-112">startDateTime</span></span>|<span data-ttu-id="fd556-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd556-113">DateTimeOffset</span></span>|<span data-ttu-id="fd556-114">开始时间的角色分配。</span><span class="sxs-lookup"><span data-stu-id="fd556-114">The start time of the role assignment.</span></span> <span data-ttu-id="fd556-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fd556-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd556-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fd556-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fd556-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fd556-117">endDateTime</span></span>|<span data-ttu-id="fd556-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd556-118">DateTimeOffset</span></span>|<span data-ttu-id="fd556-119">结束时间角色分配。</span><span class="sxs-lookup"><span data-stu-id="fd556-119">The end time of the role assignment.</span></span> <span data-ttu-id="fd556-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fd556-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd556-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="fd556-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fd556-122">*注意：如果值为 `null` ，则指示永久分配。*</span><span class="sxs-lookup"><span data-stu-id="fd556-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="fd556-123">type</span><span class="sxs-lookup"><span data-stu-id="fd556-123">type</span></span>|<span data-ttu-id="fd556-124">字符串</span><span class="sxs-lookup"><span data-stu-id="fd556-124">String</span></span>|<span data-ttu-id="fd556-125">计划角色分配类型。</span><span class="sxs-lookup"><span data-stu-id="fd556-125">The role assignment schedule type.</span></span> <span data-ttu-id="fd556-126">目前 `Once` 仅受支持。</span><span class="sxs-lookup"><span data-stu-id="fd556-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="fd556-127">duration</span><span class="sxs-lookup"><span data-stu-id="fd556-127">duration</span></span>|<span data-ttu-id="fd556-128">持续时间</span><span class="sxs-lookup"><span data-stu-id="fd556-128">Duration</span></span>|<span data-ttu-id="fd556-129">一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="fd556-129">The duration of a role assignment.</span></span> <span data-ttu-id="fd556-130">它采用 TimeSpan 格式。</span><span class="sxs-lookup"><span data-stu-id="fd556-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd556-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd556-131">JSON representation</span></span>

<span data-ttu-id="fd556-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd556-132">Here is a JSON representation of the resource.</span></span>

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


