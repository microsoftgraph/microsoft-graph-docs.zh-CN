---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 64ef8a07d3190ad2a54e9e3e5c68f3ffb0335acc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866523"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="2ca8c-103">timeOff 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ca8c-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ca8c-104">计划中非工作的单位。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-104">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="2ca8c-105">方法</span><span class="sxs-lookup"><span data-stu-id="2ca8c-105">Methods</span></span>

| <span data-ttu-id="2ca8c-106">方法</span><span class="sxs-lookup"><span data-stu-id="2ca8c-106">Method</span></span>       | <span data-ttu-id="2ca8c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ca8c-107">Return Type</span></span>  |<span data-ttu-id="2ca8c-108">说明</span><span class="sxs-lookup"><span data-stu-id="2ca8c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ca8c-109">Create</span><span class="sxs-lookup"><span data-stu-id="2ca8c-109">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="2ca8c-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="2ca8c-110">timeOff</span></span>](timeoff.md) | <span data-ttu-id="2ca8c-111">创建新的**timeOff**对象。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-111">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="2ca8c-112">List</span><span class="sxs-lookup"><span data-stu-id="2ca8c-112">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="2ca8c-113">[timeOff](timeoff.md)集合</span><span class="sxs-lookup"><span data-stu-id="2ca8c-113">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="2ca8c-114">获取此计划中的**timeOff**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-114">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="2ca8c-115">[获取（.。。/api/timeoff-get.md)</span><span class="sxs-lookup"><span data-stu-id="2ca8c-115">[Get (../api/timeoff-get.md)</span></span> | [<span data-ttu-id="2ca8c-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="2ca8c-116">timeOff</span></span>](timeoff.md) | <span data-ttu-id="2ca8c-117">按 ID 获取**timeOff**对象。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-117">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="2ca8c-118">Replace</span><span class="sxs-lookup"><span data-stu-id="2ca8c-118">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="2ca8c-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="2ca8c-119">timeOff</span></span>](timeoff.md) | <span data-ttu-id="2ca8c-120">替换**timeOff**对象。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-120">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="2ca8c-121">删除</span><span class="sxs-lookup"><span data-stu-id="2ca8c-121">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="2ca8c-122">无</span><span class="sxs-lookup"><span data-stu-id="2ca8c-122">None</span></span> | <span data-ttu-id="2ca8c-123">从计划中删除**timeOff**对象。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-123">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ca8c-124">属性</span><span class="sxs-lookup"><span data-stu-id="2ca8c-124">Properties</span></span>
|<span data-ttu-id="2ca8c-125">名称</span><span class="sxs-lookup"><span data-stu-id="2ca8c-125">Name</span></span>          |<span data-ttu-id="2ca8c-126">类型</span><span class="sxs-lookup"><span data-stu-id="2ca8c-126">Type</span></span>           |<span data-ttu-id="2ca8c-127">说明</span><span class="sxs-lookup"><span data-stu-id="2ca8c-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2ca8c-128">id</span><span class="sxs-lookup"><span data-stu-id="2ca8c-128">id</span></span>            |`string`      |<span data-ttu-id="2ca8c-129">`timeOff` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="2ca8c-130">userId</span><span class="sxs-lookup"><span data-stu-id="2ca8c-130">userId</span></span>            |`string`      |<span data-ttu-id="2ca8c-131">分配给的`timeOff`用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="2ca8c-132">必需。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-132">Required.</span></span>|
| <span data-ttu-id="2ca8c-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="2ca8c-133">sharedTimeOff</span></span>     | [<span data-ttu-id="2ca8c-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="2ca8c-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="2ca8c-135">员工和经理可查看`timeOff`的共享版本。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="2ca8c-136">必需。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-136">Required.</span></span>|
| <span data-ttu-id="2ca8c-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="2ca8c-137">draftTimeOff</span></span>      | [<span data-ttu-id="2ca8c-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="2ca8c-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="2ca8c-139">经理可查看的草稿`timeOff`版本。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="2ca8c-140">必需。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-140">Required.</span></span>|
| <span data-ttu-id="2ca8c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca8c-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="2ca8c-142">首次创建时的时间`timeOff`戳。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="2ca8c-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ca8c-144">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2ca8c-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca8c-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="2ca8c-146">上次更新此`timeOff`时间戳的时间戳。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="2ca8c-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ca8c-148">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2ca8c-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2ca8c-149">lastModifiedBy</span></span>        | [<span data-ttu-id="2ca8c-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ca8c-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="2ca8c-151">上次更新 `timeOff` 的标识。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2ca8c-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ca8c-152">JSON representation</span></span>

<span data-ttu-id="2ca8c-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ca8c-153">Here is a JSON representation of the resource.</span></span>

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
