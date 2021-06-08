---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 89b74e74b505f542730635ddc0832b834592ff4e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784995"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="381ac-103">timeOff 资源类型</span><span class="sxs-lookup"><span data-stu-id="381ac-103">timeOff resource type</span></span>

<span data-ttu-id="381ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="381ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="381ac-105">计划中的非工作单位。</span><span class="sxs-lookup"><span data-stu-id="381ac-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="381ac-106">方法</span><span class="sxs-lookup"><span data-stu-id="381ac-106">Methods</span></span>

| <span data-ttu-id="381ac-107">方法</span><span class="sxs-lookup"><span data-stu-id="381ac-107">Method</span></span>       | <span data-ttu-id="381ac-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="381ac-108">Return type</span></span>  |<span data-ttu-id="381ac-109">说明</span><span class="sxs-lookup"><span data-stu-id="381ac-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="381ac-110">创建</span><span class="sxs-lookup"><span data-stu-id="381ac-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="381ac-111">timeOff</span><span class="sxs-lookup"><span data-stu-id="381ac-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="381ac-112">创建新的 **timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="381ac-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="381ac-113">List</span><span class="sxs-lookup"><span data-stu-id="381ac-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="381ac-114">[timeOff](timeoff.md) 集合</span><span class="sxs-lookup"><span data-stu-id="381ac-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="381ac-115">获取此 **计划中的 timeOff** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="381ac-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|[<span data-ttu-id="381ac-116">获取</span><span class="sxs-lookup"><span data-stu-id="381ac-116">Get</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="381ac-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="381ac-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="381ac-118">按 ID **获取 timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="381ac-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="381ac-119">Replace</span><span class="sxs-lookup"><span data-stu-id="381ac-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="381ac-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="381ac-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="381ac-121">替换 **timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="381ac-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="381ac-122">删除</span><span class="sxs-lookup"><span data-stu-id="381ac-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="381ac-123">无</span><span class="sxs-lookup"><span data-stu-id="381ac-123">None</span></span> | <span data-ttu-id="381ac-124">从 **计划中删除 timeOff** 对象。</span><span class="sxs-lookup"><span data-stu-id="381ac-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="381ac-125">属性</span><span class="sxs-lookup"><span data-stu-id="381ac-125">Properties</span></span>
|<span data-ttu-id="381ac-126">名称</span><span class="sxs-lookup"><span data-stu-id="381ac-126">Name</span></span>          |<span data-ttu-id="381ac-127">类型</span><span class="sxs-lookup"><span data-stu-id="381ac-127">Type</span></span>           |<span data-ttu-id="381ac-128">说明</span><span class="sxs-lookup"><span data-stu-id="381ac-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="381ac-129">id</span><span class="sxs-lookup"><span data-stu-id="381ac-129">id</span></span>            |`string`      |<span data-ttu-id="381ac-130">**timeOff** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="381ac-130">ID of the **timeOff**.</span></span>|
| <span data-ttu-id="381ac-131">userId</span><span class="sxs-lookup"><span data-stu-id="381ac-131">userId</span></span>            |`string`      |<span data-ttu-id="381ac-132">分配给 **timeOff** 的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="381ac-132">ID of the user assigned to the **timeOff**.</span></span> <span data-ttu-id="381ac-133">必填。</span><span class="sxs-lookup"><span data-stu-id="381ac-133">Required.</span></span>|
| <span data-ttu-id="381ac-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="381ac-134">sharedTimeOff</span></span>     | [<span data-ttu-id="381ac-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="381ac-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="381ac-136">员工和经理都可查看的 **此 timeOff** 的共享版本。</span><span class="sxs-lookup"><span data-stu-id="381ac-136">The shared version of this **timeOff** that is viewable by both employees and managers.</span></span> <span data-ttu-id="381ac-137">必填。</span><span class="sxs-lookup"><span data-stu-id="381ac-137">Required.</span></span>|
| <span data-ttu-id="381ac-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="381ac-138">draftTimeOff</span></span>      | [<span data-ttu-id="381ac-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="381ac-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="381ac-140">经理可查看的 **此时间Off** 的草稿版本。</span><span class="sxs-lookup"><span data-stu-id="381ac-140">The draft version of this **timeOff** that is viewable by managers.</span></span> <span data-ttu-id="381ac-141">必填。</span><span class="sxs-lookup"><span data-stu-id="381ac-141">Required.</span></span>|
| <span data-ttu-id="381ac-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="381ac-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="381ac-143">首次创建 **TimeOff** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="381ac-143">The time stamp at which this **timeOff** was first created.</span></span> <span data-ttu-id="381ac-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="381ac-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="381ac-145">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="381ac-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="381ac-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="381ac-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="381ac-147">上次更新 **TimeOff** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="381ac-147">The time stamp at which this **timeOff** was last updated.</span></span> <span data-ttu-id="381ac-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="381ac-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="381ac-149">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="381ac-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="381ac-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="381ac-150">lastModifiedBy</span></span>        | [<span data-ttu-id="381ac-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="381ac-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="381ac-152">上次更新 **的标识Off**。</span><span class="sxs-lookup"><span data-stu-id="381ac-152">The identity that last updated this **timeOff**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="381ac-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="381ac-153">JSON representation</span></span>

<span data-ttu-id="381ac-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="381ac-154">Here is a JSON representation of the resource.</span></span>

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


