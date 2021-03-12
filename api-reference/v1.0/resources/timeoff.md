---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a3060b9fcd47bddc2d589d2ffdfc249146ee4dca
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720849"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="3f934-103">timeOff 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f934-103">timeOff resource type</span></span>

<span data-ttu-id="3f934-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f934-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f934-105">计划中的非工作单位。</span><span class="sxs-lookup"><span data-stu-id="3f934-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="3f934-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3f934-106">Methods</span></span>

| <span data-ttu-id="3f934-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f934-107">Method</span></span>       | <span data-ttu-id="3f934-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f934-108">Return Type</span></span>  |<span data-ttu-id="3f934-109">Description</span><span class="sxs-lookup"><span data-stu-id="3f934-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f934-110">List</span><span class="sxs-lookup"><span data-stu-id="3f934-110">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="3f934-111">[timeOff](timeoff.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f934-111">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="3f934-112">获取此 **计划中的 timeOff** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="3f934-112">Get the list of **timeOff** objects in this schedule.</span></span>|
|[<span data-ttu-id="3f934-113">创建</span><span class="sxs-lookup"><span data-stu-id="3f934-113">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="3f934-114">timeOff</span><span class="sxs-lookup"><span data-stu-id="3f934-114">timeOff</span></span>](timeoff.md) | <span data-ttu-id="3f934-115">创建新的 **timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="3f934-115">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="3f934-116">获取</span><span class="sxs-lookup"><span data-stu-id="3f934-116">Get</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="3f934-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="3f934-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="3f934-118">按 ID **获取 timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="3f934-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="3f934-119">Replace</span><span class="sxs-lookup"><span data-stu-id="3f934-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="3f934-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="3f934-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="3f934-121">替换 **timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="3f934-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="3f934-122">删除</span><span class="sxs-lookup"><span data-stu-id="3f934-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="3f934-123">无</span><span class="sxs-lookup"><span data-stu-id="3f934-123">None</span></span> | <span data-ttu-id="3f934-124">从 **计划中删除 timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="3f934-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f934-125">属性</span><span class="sxs-lookup"><span data-stu-id="3f934-125">Properties</span></span>
|<span data-ttu-id="3f934-126">名称</span><span class="sxs-lookup"><span data-stu-id="3f934-126">Name</span></span>          |<span data-ttu-id="3f934-127">类型</span><span class="sxs-lookup"><span data-stu-id="3f934-127">Type</span></span>           |<span data-ttu-id="3f934-128">说明</span><span class="sxs-lookup"><span data-stu-id="3f934-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3f934-129">id</span><span class="sxs-lookup"><span data-stu-id="3f934-129">id</span></span>            |`string`      |<span data-ttu-id="3f934-130">**timeOff** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f934-130">ID of the **timeOff**.</span></span>|
| <span data-ttu-id="3f934-131">userId</span><span class="sxs-lookup"><span data-stu-id="3f934-131">userId</span></span>            |`string`      |<span data-ttu-id="3f934-132">分配给 **timeOff** 的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f934-132">ID of the user assigned to the **timeOff**.</span></span> <span data-ttu-id="3f934-133">必需。</span><span class="sxs-lookup"><span data-stu-id="3f934-133">Required.</span></span>|
| <span data-ttu-id="3f934-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="3f934-134">sharedTimeOff</span></span>     | [<span data-ttu-id="3f934-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="3f934-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="3f934-136">员工和经理都可查看的 **此 timeOff** 的共享版本。</span><span class="sxs-lookup"><span data-stu-id="3f934-136">The shared version of this **timeOff** that is viewable by both employees and managers.</span></span> <span data-ttu-id="3f934-137">必需。</span><span class="sxs-lookup"><span data-stu-id="3f934-137">Required.</span></span>|
| <span data-ttu-id="3f934-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="3f934-138">draftTimeOff</span></span>      | [<span data-ttu-id="3f934-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="3f934-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="3f934-140">经理可查看的 **此时间Off** 的草稿版本。</span><span class="sxs-lookup"><span data-stu-id="3f934-140">The draft version of this **timeOff** that is viewable by managers.</span></span> <span data-ttu-id="3f934-141">必需。</span><span class="sxs-lookup"><span data-stu-id="3f934-141">Required.</span></span>|
| <span data-ttu-id="3f934-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f934-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="3f934-143">首次创建 **TimeOff** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="3f934-143">The time stamp at which this **timeOff** was first created.</span></span> <span data-ttu-id="3f934-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3f934-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f934-145">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="3f934-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="3f934-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f934-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="3f934-147">上次更新 **TimeOff** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="3f934-147">The time stamp at which this **timeOff** was last updated.</span></span> <span data-ttu-id="3f934-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3f934-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f934-149">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="3f934-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="3f934-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3f934-150">lastModifiedBy</span></span>        | [<span data-ttu-id="3f934-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="3f934-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="3f934-152">上次更新 **的标识Off**。</span><span class="sxs-lookup"><span data-stu-id="3f934-152">The identity that last updated this **timeOff**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3f934-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f934-153">JSON representation</span></span>

<span data-ttu-id="3f934-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f934-154">The following is a JSON representation of the resource.</span></span>

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

