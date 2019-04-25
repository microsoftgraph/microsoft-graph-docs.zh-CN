---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582841"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="ab5db-103">timeOff 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab5db-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab5db-104">计划中的非工作单位。</span><span class="sxs-lookup"><span data-stu-id="ab5db-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="ab5db-105">方法</span><span class="sxs-lookup"><span data-stu-id="ab5db-105">Methods</span></span>

| <span data-ttu-id="ab5db-106">方法</span><span class="sxs-lookup"><span data-stu-id="ab5db-106">Method</span></span>       | <span data-ttu-id="ab5db-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab5db-107">Return Type</span></span>  |<span data-ttu-id="ab5db-108">说明</span><span class="sxs-lookup"><span data-stu-id="ab5db-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab5db-109">创建 timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="ab5db-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="ab5db-111">创建一个新的 `timeOff` 对象。</span><span class="sxs-lookup"><span data-stu-id="ab5db-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="ab5db-112">列出 timeOffs</span><span class="sxs-lookup"><span data-stu-id="ab5db-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="ab5db-113">[timeOff](timeOff.md)集合</span><span class="sxs-lookup"><span data-stu-id="ab5db-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="ab5db-114">获取此计划中`timeOff`的对象列表。</span><span class="sxs-lookup"><span data-stu-id="ab5db-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="ab5db-115">获取 timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="ab5db-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="ab5db-117">按 ID 获取 `timeOff`。</span><span class="sxs-lookup"><span data-stu-id="ab5db-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="ab5db-118">替换 timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="ab5db-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="ab5db-120">更换 `timeOff`。</span><span class="sxs-lookup"><span data-stu-id="ab5db-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="ab5db-121">删除 timeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="ab5db-122">无</span><span class="sxs-lookup"><span data-stu-id="ab5db-122">None</span></span> | <span data-ttu-id="ab5db-123">`timeOff`从计划中删除。</span><span class="sxs-lookup"><span data-stu-id="ab5db-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab5db-124">属性</span><span class="sxs-lookup"><span data-stu-id="ab5db-124">Properties</span></span>
|<span data-ttu-id="ab5db-125">名称</span><span class="sxs-lookup"><span data-stu-id="ab5db-125">Name</span></span>          |<span data-ttu-id="ab5db-126">类型</span><span class="sxs-lookup"><span data-stu-id="ab5db-126">Type</span></span>           |<span data-ttu-id="ab5db-127">说明</span><span class="sxs-lookup"><span data-stu-id="ab5db-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ab5db-128">id</span><span class="sxs-lookup"><span data-stu-id="ab5db-128">id</span></span>            |`string`      |<span data-ttu-id="ab5db-129">`timeOff` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="ab5db-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="ab5db-130">userId</span><span class="sxs-lookup"><span data-stu-id="ab5db-130">userId</span></span>            |`string`      |<span data-ttu-id="ab5db-131">分配给的`timeOff`用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="ab5db-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="ab5db-132">必需。</span><span class="sxs-lookup"><span data-stu-id="ab5db-132">Required.</span></span>|
| <span data-ttu-id="ab5db-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-133">sharedTimeOff</span></span>     |[<span data-ttu-id="ab5db-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="ab5db-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="ab5db-135">员工和经理可查看`timeOff`的共享版本。</span><span class="sxs-lookup"><span data-stu-id="ab5db-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="ab5db-136">必需。</span><span class="sxs-lookup"><span data-stu-id="ab5db-136">Required.</span></span>|
| <span data-ttu-id="ab5db-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="ab5db-137">draftTimeOff</span></span>      |[<span data-ttu-id="ab5db-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="ab5db-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="ab5db-139">经理可查看的草稿`timeOff`版本。</span><span class="sxs-lookup"><span data-stu-id="ab5db-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="ab5db-140">必需。</span><span class="sxs-lookup"><span data-stu-id="ab5db-140">Required.</span></span>|
| <span data-ttu-id="ab5db-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab5db-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="ab5db-142">首次创建时的时间`timeOff`戳。</span><span class="sxs-lookup"><span data-stu-id="ab5db-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="ab5db-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ab5db-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab5db-144">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="ab5db-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ab5db-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab5db-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="ab5db-146">上次更新此`timeOff`时间戳的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ab5db-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="ab5db-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ab5db-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab5db-148">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="ab5db-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ab5db-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ab5db-149">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="ab5db-150">上次更新 `timeOff` 的标识。</span><span class="sxs-lookup"><span data-stu-id="ab5db-150">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab5db-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab5db-151">JSON representation</span></span>

<span data-ttu-id="ab5db-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab5db-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
