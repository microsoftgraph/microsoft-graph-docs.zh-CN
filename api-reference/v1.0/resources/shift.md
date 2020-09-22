---
title: shift 资源类型
description: 表示计划中计划工时的单位。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52c83c8052725e99d1136df8b0c14d8d3c24ffe4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086429"
---
# <a name="shift-resource-type"></a><span data-ttu-id="6c7fc-103">shift 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c7fc-103">shift resource type</span></span>

<span data-ttu-id="6c7fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c7fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c7fc-105">表示计划中计划工时的[单位。](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="6c7fc-105">Represents a unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="6c7fc-106">方法</span><span class="sxs-lookup"><span data-stu-id="6c7fc-106">Methods</span></span>

| <span data-ttu-id="6c7fc-107">方法</span><span class="sxs-lookup"><span data-stu-id="6c7fc-107">Method</span></span>       | <span data-ttu-id="6c7fc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c7fc-108">Return Type</span></span>  |<span data-ttu-id="6c7fc-109">说明</span><span class="sxs-lookup"><span data-stu-id="6c7fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c7fc-110">列出班次</span><span class="sxs-lookup"><span data-stu-id="6c7fc-110">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="6c7fc-111">[shift](shift.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c7fc-111">[shift](shift.md) collection</span></span> | <span data-ttu-id="6c7fc-112">获取此计划中 **班次** 的列表。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-112">Get the list of **shifts** in this schedule.</span></span>|
|[<span data-ttu-id="6c7fc-113">创建班次</span><span class="sxs-lookup"><span data-stu-id="6c7fc-113">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="6c7fc-114">shift</span><span class="sxs-lookup"><span data-stu-id="6c7fc-114">shift</span></span>](shift.md) | <span data-ttu-id="6c7fc-115">创建新 **班次**。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-115">Create a new **shift**.</span></span>|
|[<span data-ttu-id="6c7fc-116">获取 shift</span><span class="sxs-lookup"><span data-stu-id="6c7fc-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="6c7fc-117">shift</span><span class="sxs-lookup"><span data-stu-id="6c7fc-117">shift</span></span>](shift.md) | <span data-ttu-id="6c7fc-118">按 ID 获取 **shift** 。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-118">Get a **shift** by ID.</span></span>|
|[<span data-ttu-id="6c7fc-119">替换班次</span><span class="sxs-lookup"><span data-stu-id="6c7fc-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="6c7fc-120">shift</span><span class="sxs-lookup"><span data-stu-id="6c7fc-120">shift</span></span>](shift.md) | <span data-ttu-id="6c7fc-121">替换 **班次**。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-121">Replace a **shift**.</span></span>|
|[<span data-ttu-id="6c7fc-122">删除班次</span><span class="sxs-lookup"><span data-stu-id="6c7fc-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="6c7fc-123">无</span><span class="sxs-lookup"><span data-stu-id="6c7fc-123">None</span></span> | <span data-ttu-id="6c7fc-124">从计划中删除 **班次轮换** 。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-124">Delete a **shift** from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c7fc-125">属性</span><span class="sxs-lookup"><span data-stu-id="6c7fc-125">Properties</span></span>
|<span data-ttu-id="6c7fc-126">名称</span><span class="sxs-lookup"><span data-stu-id="6c7fc-126">Name</span></span>          |<span data-ttu-id="6c7fc-127">类型</span><span class="sxs-lookup"><span data-stu-id="6c7fc-127">Type</span></span>           |<span data-ttu-id="6c7fc-128">说明</span><span class="sxs-lookup"><span data-stu-id="6c7fc-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6c7fc-129">id</span><span class="sxs-lookup"><span data-stu-id="6c7fc-129">id</span></span>            |`string`      |<span data-ttu-id="6c7fc-130">**班次**的 ID。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-130">ID of the **shift**.</span></span>|
| <span data-ttu-id="6c7fc-131">userId</span><span class="sxs-lookup"><span data-stu-id="6c7fc-131">userId</span></span>            |`string`      |<span data-ttu-id="6c7fc-132">分配给 **班次**的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-132">ID of the user assigned to the **shift**.</span></span> <span data-ttu-id="6c7fc-133">必需。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-133">Required.</span></span> |
| <span data-ttu-id="6c7fc-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="6c7fc-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="6c7fc-135">**班次**所属的计划组的 ID。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-135">ID of the scheduling group the **shift** is part of.</span></span> <span data-ttu-id="6c7fc-136">必需。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-136">Required.</span></span> |
| <span data-ttu-id="6c7fc-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="6c7fc-137">sharedShift</span></span>   |[<span data-ttu-id="6c7fc-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="6c7fc-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="6c7fc-139">员工和经理都可查看的此 **班次** 的共享版本。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-139">The shared version of this **shift** that is viewable by both employees and managers.</span></span> <span data-ttu-id="6c7fc-140">必需。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-140">Required.</span></span> |
| <span data-ttu-id="6c7fc-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="6c7fc-141">draftShift</span></span>        |[<span data-ttu-id="6c7fc-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="6c7fc-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="6c7fc-143">由经理查看的此 **班次** 的草稿版本。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-143">The draft version of this **shift** that is viewable by managers.</span></span> <span data-ttu-id="6c7fc-144">必需。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-144">Required.</span></span> |
| <span data-ttu-id="6c7fc-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c7fc-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="6c7fc-146">此 **班次** 首次创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-146">The timestamp on which this **shift** was first created.</span></span> <span data-ttu-id="6c7fc-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c7fc-148">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6c7fc-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c7fc-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="6c7fc-150">此 **班次** 的上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-150">The timestamp on which this **shift** was last updated.</span></span> <span data-ttu-id="6c7fc-151">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c7fc-152">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6c7fc-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6c7fc-153">lastModifiedBy</span></span>        | [<span data-ttu-id="6c7fc-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c7fc-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="6c7fc-155">上次更新此 **班次**的标识。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-155">The identity that last updated this **shift**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c7fc-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c7fc-156">JSON representation</span></span>

<span data-ttu-id="6c7fc-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c7fc-157">The following is a JSON representation of the resource.</span></span>

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

