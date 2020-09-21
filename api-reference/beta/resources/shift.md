---
title: shift 资源类型
description: 班次是计划中计划工时的单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 49d877859202ca9d8dc5c7b414368a63d2fcf8ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058095"
---
# <a name="shift-resource-type"></a><span data-ttu-id="f78ed-103">shift 资源类型</span><span class="sxs-lookup"><span data-stu-id="f78ed-103">shift resource type</span></span>

<span data-ttu-id="f78ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f78ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f78ed-105">计划中计划工时的[单位。](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="f78ed-105">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="f78ed-106">方法</span><span class="sxs-lookup"><span data-stu-id="f78ed-106">Methods</span></span>

| <span data-ttu-id="f78ed-107">方法</span><span class="sxs-lookup"><span data-stu-id="f78ed-107">Method</span></span>       | <span data-ttu-id="f78ed-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f78ed-108">Return Type</span></span>  |<span data-ttu-id="f78ed-109">说明</span><span class="sxs-lookup"><span data-stu-id="f78ed-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f78ed-110">创建班次</span><span class="sxs-lookup"><span data-stu-id="f78ed-110">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="f78ed-111">shift</span><span class="sxs-lookup"><span data-stu-id="f78ed-111">shift</span></span>](shift.md) | <span data-ttu-id="f78ed-112">新建 `shift`。</span><span class="sxs-lookup"><span data-stu-id="f78ed-112">Create a new `shift`.</span></span>|
|[<span data-ttu-id="f78ed-113">列出班次</span><span class="sxs-lookup"><span data-stu-id="f78ed-113">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="f78ed-114">[shift](shift.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f78ed-114">[shift](shift.md) collection</span></span> | <span data-ttu-id="f78ed-115">获取 `shifts` 此计划中的列表。</span><span class="sxs-lookup"><span data-stu-id="f78ed-115">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="f78ed-116">获取 shift</span><span class="sxs-lookup"><span data-stu-id="f78ed-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="f78ed-117">shift</span><span class="sxs-lookup"><span data-stu-id="f78ed-117">shift</span></span>](shift.md) | <span data-ttu-id="f78ed-118">按 ID 获取 `shift`。</span><span class="sxs-lookup"><span data-stu-id="f78ed-118">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="f78ed-119">替换班次</span><span class="sxs-lookup"><span data-stu-id="f78ed-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="f78ed-120">shift</span><span class="sxs-lookup"><span data-stu-id="f78ed-120">shift</span></span>](shift.md) | <span data-ttu-id="f78ed-121">更换 `shift`。</span><span class="sxs-lookup"><span data-stu-id="f78ed-121">Replace a `shift`.</span></span>|
|[<span data-ttu-id="f78ed-122">删除班次</span><span class="sxs-lookup"><span data-stu-id="f78ed-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="f78ed-123">无</span><span class="sxs-lookup"><span data-stu-id="f78ed-123">None</span></span> | <span data-ttu-id="f78ed-124">`shift`从计划中删除。</span><span class="sxs-lookup"><span data-stu-id="f78ed-124">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="f78ed-125">属性</span><span class="sxs-lookup"><span data-stu-id="f78ed-125">Properties</span></span>
|<span data-ttu-id="f78ed-126">名称</span><span class="sxs-lookup"><span data-stu-id="f78ed-126">Name</span></span>          |<span data-ttu-id="f78ed-127">类型</span><span class="sxs-lookup"><span data-stu-id="f78ed-127">Type</span></span>           |<span data-ttu-id="f78ed-128">说明</span><span class="sxs-lookup"><span data-stu-id="f78ed-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f78ed-129">id</span><span class="sxs-lookup"><span data-stu-id="f78ed-129">id</span></span>            |`string`      |<span data-ttu-id="f78ed-130">`shift` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="f78ed-130">ID of the `shift`.</span></span>|
| <span data-ttu-id="f78ed-131">userId</span><span class="sxs-lookup"><span data-stu-id="f78ed-131">userId</span></span>            |`string`      |<span data-ttu-id="f78ed-132">分配给的用户的 ID `shift` 。</span><span class="sxs-lookup"><span data-stu-id="f78ed-132">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="f78ed-133">必需。</span><span class="sxs-lookup"><span data-stu-id="f78ed-133">Required.</span></span> |
| <span data-ttu-id="f78ed-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="f78ed-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="f78ed-135">属于的计划组的 ID `shift` 。</span><span class="sxs-lookup"><span data-stu-id="f78ed-135">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="f78ed-136">必需。</span><span class="sxs-lookup"><span data-stu-id="f78ed-136">Required.</span></span> |
| <span data-ttu-id="f78ed-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="f78ed-137">sharedShift</span></span>   |[<span data-ttu-id="f78ed-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="f78ed-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="f78ed-139">`shift`员工和经理可查看的共享版本。</span><span class="sxs-lookup"><span data-stu-id="f78ed-139">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="f78ed-140">必需。</span><span class="sxs-lookup"><span data-stu-id="f78ed-140">Required.</span></span> |
| <span data-ttu-id="f78ed-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="f78ed-141">draftShift</span></span>        |[<span data-ttu-id="f78ed-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="f78ed-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="f78ed-143">经理可查看的草稿版本 `shift` 。</span><span class="sxs-lookup"><span data-stu-id="f78ed-143">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="f78ed-144">必需。</span><span class="sxs-lookup"><span data-stu-id="f78ed-144">Required.</span></span> |
| <span data-ttu-id="f78ed-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f78ed-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="f78ed-146">首次在其上创建此项的时间戳 `shift` 。</span><span class="sxs-lookup"><span data-stu-id="f78ed-146">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="f78ed-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f78ed-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f78ed-148">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="f78ed-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="f78ed-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f78ed-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="f78ed-150">上次更新此时间的时间戳 `shift` 。</span><span class="sxs-lookup"><span data-stu-id="f78ed-150">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="f78ed-151">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f78ed-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f78ed-152">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="f78ed-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="f78ed-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f78ed-153">lastModifiedBy</span></span>        | [<span data-ttu-id="f78ed-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="f78ed-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="f78ed-155">上次更新 `shift` 的标识。</span><span class="sxs-lookup"><span data-stu-id="f78ed-155">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f78ed-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f78ed-156">JSON representation</span></span>

<span data-ttu-id="f78ed-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f78ed-157">Here is a JSON representation of the resource.</span></span>

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


