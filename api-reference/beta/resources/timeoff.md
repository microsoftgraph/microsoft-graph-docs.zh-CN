---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 848365a812053b7788db37395bee8662d69cda37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342013"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="41a20-103">timeOff 资源类型</span><span class="sxs-lookup"><span data-stu-id="41a20-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41a20-104">计划中的非工作单位。</span><span class="sxs-lookup"><span data-stu-id="41a20-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="41a20-105">方法</span><span class="sxs-lookup"><span data-stu-id="41a20-105">Methods</span></span>

| <span data-ttu-id="41a20-106">方法</span><span class="sxs-lookup"><span data-stu-id="41a20-106">Method</span></span>       | <span data-ttu-id="41a20-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="41a20-107">Return Type</span></span>  |<span data-ttu-id="41a20-108">说明</span><span class="sxs-lookup"><span data-stu-id="41a20-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41a20-109">创建 timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="41a20-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="41a20-111">创建一个新的 `timeOff` 对象。</span><span class="sxs-lookup"><span data-stu-id="41a20-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="41a20-112">列出 timeOffs</span><span class="sxs-lookup"><span data-stu-id="41a20-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="41a20-113">[timeOff](timeOff.md)集合</span><span class="sxs-lookup"><span data-stu-id="41a20-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="41a20-114">获取此计划中`timeOff`的对象列表。</span><span class="sxs-lookup"><span data-stu-id="41a20-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="41a20-115">获取 timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="41a20-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="41a20-117">按 ID 获取 `timeOff`。</span><span class="sxs-lookup"><span data-stu-id="41a20-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="41a20-118">替换 timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="41a20-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="41a20-120">更换 `timeOff`。</span><span class="sxs-lookup"><span data-stu-id="41a20-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="41a20-121">删除 timeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="41a20-122">无</span><span class="sxs-lookup"><span data-stu-id="41a20-122">None</span></span> | <span data-ttu-id="41a20-123">`timeOff`从计划中删除。</span><span class="sxs-lookup"><span data-stu-id="41a20-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="41a20-124">属性</span><span class="sxs-lookup"><span data-stu-id="41a20-124">Properties</span></span>
|<span data-ttu-id="41a20-125">名称</span><span class="sxs-lookup"><span data-stu-id="41a20-125">Name</span></span>          |<span data-ttu-id="41a20-126">类型</span><span class="sxs-lookup"><span data-stu-id="41a20-126">Type</span></span>           |<span data-ttu-id="41a20-127">说明</span><span class="sxs-lookup"><span data-stu-id="41a20-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="41a20-128">id</span><span class="sxs-lookup"><span data-stu-id="41a20-128">id</span></span>            |`string`      |<span data-ttu-id="41a20-129">`timeOff` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="41a20-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="41a20-130">userId</span><span class="sxs-lookup"><span data-stu-id="41a20-130">userId</span></span>            |`string`      |<span data-ttu-id="41a20-131">分配给的`timeOff`用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="41a20-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="41a20-132">必需。</span><span class="sxs-lookup"><span data-stu-id="41a20-132">Required.</span></span>|
| <span data-ttu-id="41a20-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-133">sharedTimeOff</span></span>     | [<span data-ttu-id="41a20-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="41a20-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="41a20-135">员工和经理可查看`timeOff`的共享版本。</span><span class="sxs-lookup"><span data-stu-id="41a20-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="41a20-136">必需。</span><span class="sxs-lookup"><span data-stu-id="41a20-136">Required.</span></span>|
| <span data-ttu-id="41a20-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="41a20-137">draftTimeOff</span></span>      | [<span data-ttu-id="41a20-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="41a20-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="41a20-139">经理可查看的草稿`timeOff`版本。</span><span class="sxs-lookup"><span data-stu-id="41a20-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="41a20-140">必需。</span><span class="sxs-lookup"><span data-stu-id="41a20-140">Required.</span></span>|
| <span data-ttu-id="41a20-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41a20-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="41a20-142">首次创建时的时间`timeOff`戳。</span><span class="sxs-lookup"><span data-stu-id="41a20-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="41a20-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="41a20-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41a20-144">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="41a20-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="41a20-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41a20-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="41a20-146">上次更新此`timeOff`时间戳的时间戳。</span><span class="sxs-lookup"><span data-stu-id="41a20-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="41a20-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="41a20-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41a20-148">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="41a20-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="41a20-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="41a20-149">lastModifiedBy</span></span>        | [<span data-ttu-id="41a20-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="41a20-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="41a20-151">上次更新 `timeOff` 的标识。</span><span class="sxs-lookup"><span data-stu-id="41a20-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41a20-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41a20-152">JSON representation</span></span>

<span data-ttu-id="41a20-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41a20-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
