---
title: shift 资源类型
description: 班次是计划中计划工时的单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657894"
---
# <a name="shift-resource-type"></a><span data-ttu-id="e2f67-103">shift 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2f67-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2f67-104">计划中计划工时的单位。 [](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="e2f67-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="e2f67-105">方法</span><span class="sxs-lookup"><span data-stu-id="e2f67-105">Methods</span></span>

| <span data-ttu-id="e2f67-106">方法</span><span class="sxs-lookup"><span data-stu-id="e2f67-106">Method</span></span>       | <span data-ttu-id="e2f67-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2f67-107">Return Type</span></span>  |<span data-ttu-id="e2f67-108">说明</span><span class="sxs-lookup"><span data-stu-id="e2f67-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2f67-109">创建班次</span><span class="sxs-lookup"><span data-stu-id="e2f67-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="e2f67-110">ctrl</span><span class="sxs-lookup"><span data-stu-id="e2f67-110">shift</span></span>](shift.md) | <span data-ttu-id="e2f67-111">创建新`shift`的。</span><span class="sxs-lookup"><span data-stu-id="e2f67-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="e2f67-112">列出班次</span><span class="sxs-lookup"><span data-stu-id="e2f67-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="e2f67-113">[shift](shift.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2f67-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="e2f67-114">获取此计划中`shifts`的列表。</span><span class="sxs-lookup"><span data-stu-id="e2f67-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="e2f67-115">获取 shift</span><span class="sxs-lookup"><span data-stu-id="e2f67-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="e2f67-116">ctrl</span><span class="sxs-lookup"><span data-stu-id="e2f67-116">shift</span></span>](shift.md) | <span data-ttu-id="e2f67-117">`shift`按 ID 获取。</span><span class="sxs-lookup"><span data-stu-id="e2f67-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="e2f67-118">替换班次</span><span class="sxs-lookup"><span data-stu-id="e2f67-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="e2f67-119">ctrl</span><span class="sxs-lookup"><span data-stu-id="e2f67-119">shift</span></span>](shift.md) | <span data-ttu-id="e2f67-120">替换`shift`。</span><span class="sxs-lookup"><span data-stu-id="e2f67-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="e2f67-121">删除班次</span><span class="sxs-lookup"><span data-stu-id="e2f67-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="e2f67-122">无</span><span class="sxs-lookup"><span data-stu-id="e2f67-122">None</span></span> | <span data-ttu-id="e2f67-123">`shift`从计划中删除。</span><span class="sxs-lookup"><span data-stu-id="e2f67-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2f67-124">属性</span><span class="sxs-lookup"><span data-stu-id="e2f67-124">Properties</span></span>
|<span data-ttu-id="e2f67-125">名称</span><span class="sxs-lookup"><span data-stu-id="e2f67-125">Name</span></span>          |<span data-ttu-id="e2f67-126">类型</span><span class="sxs-lookup"><span data-stu-id="e2f67-126">Type</span></span>           |<span data-ttu-id="e2f67-127">说明</span><span class="sxs-lookup"><span data-stu-id="e2f67-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e2f67-128">id</span><span class="sxs-lookup"><span data-stu-id="e2f67-128">id</span></span>            |`string`      |<span data-ttu-id="e2f67-129">的 ID `shift`。</span><span class="sxs-lookup"><span data-stu-id="e2f67-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="e2f67-130">userId</span><span class="sxs-lookup"><span data-stu-id="e2f67-130">userId</span></span>            |`string`      |<span data-ttu-id="e2f67-131">分配给的`shift`用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="e2f67-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="e2f67-132">必需。</span><span class="sxs-lookup"><span data-stu-id="e2f67-132">Required.</span></span> |
| <span data-ttu-id="e2f67-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="e2f67-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="e2f67-134">属于的计划组`shift`的 ID。</span><span class="sxs-lookup"><span data-stu-id="e2f67-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="e2f67-135">必需。</span><span class="sxs-lookup"><span data-stu-id="e2f67-135">Required.</span></span> |
| <span data-ttu-id="e2f67-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="e2f67-136">sharedShift</span></span>   |`[shiftItem](shiftitem.md)`  |<span data-ttu-id="e2f67-137">员工和经理可查看`shift`的共享版本。</span><span class="sxs-lookup"><span data-stu-id="e2f67-137">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="e2f67-138">必需。</span><span class="sxs-lookup"><span data-stu-id="e2f67-138">Required.</span></span> |
| <span data-ttu-id="e2f67-139">draftShift</span><span class="sxs-lookup"><span data-stu-id="e2f67-139">draftShift</span></span>        |`[shiftItem](shiftitem.md)`        |<span data-ttu-id="e2f67-140">经理可查看的草稿`shift`版本。</span><span class="sxs-lookup"><span data-stu-id="e2f67-140">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="e2f67-141">必需。</span><span class="sxs-lookup"><span data-stu-id="e2f67-141">Required.</span></span> |
| <span data-ttu-id="e2f67-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f67-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="e2f67-143">首次在其上`shift`创建此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="e2f67-143">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="e2f67-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e2f67-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2f67-145">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="e2f67-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="e2f67-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f67-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="e2f67-147">上次更新此`shift`时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="e2f67-147">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="e2f67-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e2f67-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2f67-149">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="e2f67-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="e2f67-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e2f67-150">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="e2f67-151">最后更新此`shift`的标识。</span><span class="sxs-lookup"><span data-stu-id="e2f67-151">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2f67-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2f67-152">JSON representation</span></span>

<span data-ttu-id="e2f67-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2f67-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
