---
title: shift 资源类型
description: 班次是计划中计划工时的单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f76cd25a36ba070d9fa8281f31a1520a0d7b4435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008339"
---
# <a name="shift-resource-type"></a><span data-ttu-id="4ea21-103">shift 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ea21-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea21-104">计划中计划工时的单位。 [](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="4ea21-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="4ea21-105">方法</span><span class="sxs-lookup"><span data-stu-id="4ea21-105">Methods</span></span>

| <span data-ttu-id="4ea21-106">方法</span><span class="sxs-lookup"><span data-stu-id="4ea21-106">Method</span></span>       | <span data-ttu-id="4ea21-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4ea21-107">Return Type</span></span>  |<span data-ttu-id="4ea21-108">说明</span><span class="sxs-lookup"><span data-stu-id="4ea21-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ea21-109">创建班次</span><span class="sxs-lookup"><span data-stu-id="4ea21-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="4ea21-110">ctrl</span><span class="sxs-lookup"><span data-stu-id="4ea21-110">shift</span></span>](shift.md) | <span data-ttu-id="4ea21-111">新建 `shift`。</span><span class="sxs-lookup"><span data-stu-id="4ea21-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="4ea21-112">列出班次</span><span class="sxs-lookup"><span data-stu-id="4ea21-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="4ea21-113">[shift](shift.md)集合</span><span class="sxs-lookup"><span data-stu-id="4ea21-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="4ea21-114">获取此计划中`shifts`的列表。</span><span class="sxs-lookup"><span data-stu-id="4ea21-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="4ea21-115">获取 shift</span><span class="sxs-lookup"><span data-stu-id="4ea21-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="4ea21-116">ctrl</span><span class="sxs-lookup"><span data-stu-id="4ea21-116">shift</span></span>](shift.md) | <span data-ttu-id="4ea21-117">按 ID 获取 `shift`。</span><span class="sxs-lookup"><span data-stu-id="4ea21-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="4ea21-118">替换班次</span><span class="sxs-lookup"><span data-stu-id="4ea21-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="4ea21-119">ctrl</span><span class="sxs-lookup"><span data-stu-id="4ea21-119">shift</span></span>](shift.md) | <span data-ttu-id="4ea21-120">更换 `shift`。</span><span class="sxs-lookup"><span data-stu-id="4ea21-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="4ea21-121">删除班次</span><span class="sxs-lookup"><span data-stu-id="4ea21-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="4ea21-122">无</span><span class="sxs-lookup"><span data-stu-id="4ea21-122">None</span></span> | <span data-ttu-id="4ea21-123">`shift`从计划中删除。</span><span class="sxs-lookup"><span data-stu-id="4ea21-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ea21-124">属性</span><span class="sxs-lookup"><span data-stu-id="4ea21-124">Properties</span></span>
|<span data-ttu-id="4ea21-125">名称</span><span class="sxs-lookup"><span data-stu-id="4ea21-125">Name</span></span>          |<span data-ttu-id="4ea21-126">类型</span><span class="sxs-lookup"><span data-stu-id="4ea21-126">Type</span></span>           |<span data-ttu-id="4ea21-127">说明</span><span class="sxs-lookup"><span data-stu-id="4ea21-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4ea21-128">id</span><span class="sxs-lookup"><span data-stu-id="4ea21-128">id</span></span>            |`string`      |<span data-ttu-id="4ea21-129">`shift` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ea21-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="4ea21-130">userId</span><span class="sxs-lookup"><span data-stu-id="4ea21-130">userId</span></span>            |`string`      |<span data-ttu-id="4ea21-131">分配给的`shift`用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ea21-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="4ea21-132">必需。</span><span class="sxs-lookup"><span data-stu-id="4ea21-132">Required.</span></span> |
| <span data-ttu-id="4ea21-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="4ea21-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="4ea21-134">属于的计划组`shift`的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ea21-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="4ea21-135">必需。</span><span class="sxs-lookup"><span data-stu-id="4ea21-135">Required.</span></span> |
| <span data-ttu-id="4ea21-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="4ea21-136">sharedShift</span></span>   |[<span data-ttu-id="4ea21-137">shiftItem</span><span class="sxs-lookup"><span data-stu-id="4ea21-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="4ea21-138">员工和经理可查看`shift`的共享版本。</span><span class="sxs-lookup"><span data-stu-id="4ea21-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="4ea21-139">必需。</span><span class="sxs-lookup"><span data-stu-id="4ea21-139">Required.</span></span> |
| <span data-ttu-id="4ea21-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="4ea21-140">draftShift</span></span>        |[<span data-ttu-id="4ea21-141">shiftItem</span><span class="sxs-lookup"><span data-stu-id="4ea21-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="4ea21-142">经理可查看的草稿`shift`版本。</span><span class="sxs-lookup"><span data-stu-id="4ea21-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="4ea21-143">必需。</span><span class="sxs-lookup"><span data-stu-id="4ea21-143">Required.</span></span> |
| <span data-ttu-id="4ea21-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea21-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="4ea21-145">首次在其上`shift`创建此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="4ea21-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="4ea21-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="4ea21-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4ea21-147">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="4ea21-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4ea21-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea21-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="4ea21-149">上次更新此`shift`时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="4ea21-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="4ea21-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="4ea21-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4ea21-151">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="4ea21-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4ea21-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4ea21-152">lastModifiedBy</span></span>        | [<span data-ttu-id="4ea21-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ea21-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="4ea21-154">上次更新 `shift` 的标识。</span><span class="sxs-lookup"><span data-stu-id="4ea21-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ea21-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ea21-155">JSON representation</span></span>

<span data-ttu-id="4ea21-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ea21-156">Here is a JSON representation of the resource.</span></span>

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
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
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
  "suppressions": []
}
-->
