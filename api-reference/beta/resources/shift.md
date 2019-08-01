---
title: shift 资源类型
description: 班次是计划中计划工时的单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d3a91cd7b4f2b4d8e32219514d1190599ac416de
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049629"
---
# <a name="shift-resource-type"></a><span data-ttu-id="640a7-103">shift 资源类型</span><span class="sxs-lookup"><span data-stu-id="640a7-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="640a7-104">计划中计划工时的单位。 [](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="640a7-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="640a7-105">方法</span><span class="sxs-lookup"><span data-stu-id="640a7-105">Methods</span></span>

| <span data-ttu-id="640a7-106">方法</span><span class="sxs-lookup"><span data-stu-id="640a7-106">Method</span></span>       | <span data-ttu-id="640a7-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="640a7-107">Return Type</span></span>  |<span data-ttu-id="640a7-108">说明</span><span class="sxs-lookup"><span data-stu-id="640a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="640a7-109">创建班次</span><span class="sxs-lookup"><span data-stu-id="640a7-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="640a7-110">ctrl</span><span class="sxs-lookup"><span data-stu-id="640a7-110">shift</span></span>](shift.md) | <span data-ttu-id="640a7-111">新建 `shift`。</span><span class="sxs-lookup"><span data-stu-id="640a7-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="640a7-112">列出班次</span><span class="sxs-lookup"><span data-stu-id="640a7-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="640a7-113">[shift](shift.md)集合</span><span class="sxs-lookup"><span data-stu-id="640a7-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="640a7-114">获取此计划中`shifts`的列表。</span><span class="sxs-lookup"><span data-stu-id="640a7-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="640a7-115">获取 shift</span><span class="sxs-lookup"><span data-stu-id="640a7-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="640a7-116">ctrl</span><span class="sxs-lookup"><span data-stu-id="640a7-116">shift</span></span>](shift.md) | <span data-ttu-id="640a7-117">按 ID 获取 `shift`。</span><span class="sxs-lookup"><span data-stu-id="640a7-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="640a7-118">替换班次</span><span class="sxs-lookup"><span data-stu-id="640a7-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="640a7-119">ctrl</span><span class="sxs-lookup"><span data-stu-id="640a7-119">shift</span></span>](shift.md) | <span data-ttu-id="640a7-120">更换 `shift`。</span><span class="sxs-lookup"><span data-stu-id="640a7-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="640a7-121">删除班次</span><span class="sxs-lookup"><span data-stu-id="640a7-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="640a7-122">无</span><span class="sxs-lookup"><span data-stu-id="640a7-122">None</span></span> | <span data-ttu-id="640a7-123">`shift`从计划中删除。</span><span class="sxs-lookup"><span data-stu-id="640a7-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="640a7-124">属性</span><span class="sxs-lookup"><span data-stu-id="640a7-124">Properties</span></span>
|<span data-ttu-id="640a7-125">名称</span><span class="sxs-lookup"><span data-stu-id="640a7-125">Name</span></span>          |<span data-ttu-id="640a7-126">类型</span><span class="sxs-lookup"><span data-stu-id="640a7-126">Type</span></span>           |<span data-ttu-id="640a7-127">说明</span><span class="sxs-lookup"><span data-stu-id="640a7-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="640a7-128">id</span><span class="sxs-lookup"><span data-stu-id="640a7-128">id</span></span>            |`string`      |<span data-ttu-id="640a7-129">`shift` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="640a7-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="640a7-130">userId</span><span class="sxs-lookup"><span data-stu-id="640a7-130">userId</span></span>            |`string`      |<span data-ttu-id="640a7-131">分配给的`shift`用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="640a7-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="640a7-132">必需。</span><span class="sxs-lookup"><span data-stu-id="640a7-132">Required.</span></span> |
| <span data-ttu-id="640a7-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="640a7-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="640a7-134">属于的计划组`shift`的 ID。</span><span class="sxs-lookup"><span data-stu-id="640a7-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="640a7-135">必需。</span><span class="sxs-lookup"><span data-stu-id="640a7-135">Required.</span></span> |
| <span data-ttu-id="640a7-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="640a7-136">sharedShift</span></span>   |[<span data-ttu-id="640a7-137">shiftItem</span><span class="sxs-lookup"><span data-stu-id="640a7-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="640a7-138">员工和经理可查看`shift`的共享版本。</span><span class="sxs-lookup"><span data-stu-id="640a7-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="640a7-139">必需。</span><span class="sxs-lookup"><span data-stu-id="640a7-139">Required.</span></span> |
| <span data-ttu-id="640a7-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="640a7-140">draftShift</span></span>        |[<span data-ttu-id="640a7-141">shiftItem</span><span class="sxs-lookup"><span data-stu-id="640a7-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="640a7-142">经理可查看的草稿`shift`版本。</span><span class="sxs-lookup"><span data-stu-id="640a7-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="640a7-143">必需。</span><span class="sxs-lookup"><span data-stu-id="640a7-143">Required.</span></span> |
| <span data-ttu-id="640a7-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="640a7-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="640a7-145">首次在其上`shift`创建此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="640a7-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="640a7-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="640a7-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="640a7-147">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="640a7-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="640a7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="640a7-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="640a7-149">上次更新此`shift`时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="640a7-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="640a7-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="640a7-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="640a7-151">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="640a7-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="640a7-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="640a7-152">lastModifiedBy</span></span>        | [<span data-ttu-id="640a7-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="640a7-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="640a7-154">上次更新 `shift` 的标识。</span><span class="sxs-lookup"><span data-stu-id="640a7-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="640a7-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="640a7-155">JSON representation</span></span>

<span data-ttu-id="640a7-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="640a7-156">Here is a JSON representation of the resource.</span></span>

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
