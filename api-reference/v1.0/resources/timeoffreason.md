---
title: timeOffReason 资源类型
description: 表示在计划中请假的有效原因。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9d73892d8bcd8ca6beba8be66fe0acc1f036e41e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720086"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="5a19c-103">timeOffReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a19c-103">timeOffReason resource type</span></span>

<span data-ttu-id="5a19c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a19c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a19c-105">表示计划 中的 [timeOff](timeoff.md) 实例的有效 [原因](schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="5a19c-105">Represents a valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5a19c-106">Methods</span><span class="sxs-lookup"><span data-stu-id="5a19c-106">Methods</span></span>

| <span data-ttu-id="5a19c-107">方法</span><span class="sxs-lookup"><span data-stu-id="5a19c-107">Method</span></span>       | <span data-ttu-id="5a19c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a19c-108">Return Type</span></span>  |<span data-ttu-id="5a19c-109">Description</span><span class="sxs-lookup"><span data-stu-id="5a19c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a19c-110">List</span><span class="sxs-lookup"><span data-stu-id="5a19c-110">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="5a19c-111">[timeOffReason](timeoffreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a19c-111">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="5a19c-112">获取计划中的 **timeOffReason** 列表。</span><span class="sxs-lookup"><span data-stu-id="5a19c-112">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="5a19c-113">创建</span><span class="sxs-lookup"><span data-stu-id="5a19c-113">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="5a19c-114">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5a19c-114">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="5a19c-115">创建新的 **timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="5a19c-115">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="5a19c-116">获取</span><span class="sxs-lookup"><span data-stu-id="5a19c-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="5a19c-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5a19c-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="5a19c-118">按 ID **获取 timeOffReason。**</span><span class="sxs-lookup"><span data-stu-id="5a19c-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="5a19c-119">Replace</span><span class="sxs-lookup"><span data-stu-id="5a19c-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="5a19c-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5a19c-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="5a19c-121">替换 **timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="5a19c-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="5a19c-122">删除</span><span class="sxs-lookup"><span data-stu-id="5a19c-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="5a19c-123">无</span><span class="sxs-lookup"><span data-stu-id="5a19c-123">None</span></span> | <span data-ttu-id="5a19c-124">将 **timeOffReason** 标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="5a19c-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a19c-125">属性</span><span class="sxs-lookup"><span data-stu-id="5a19c-125">Properties</span></span>
|<span data-ttu-id="5a19c-126">名称</span><span class="sxs-lookup"><span data-stu-id="5a19c-126">Name</span></span>          |<span data-ttu-id="5a19c-127">类型</span><span class="sxs-lookup"><span data-stu-id="5a19c-127">Type</span></span>           |<span data-ttu-id="5a19c-128">说明</span><span class="sxs-lookup"><span data-stu-id="5a19c-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="5a19c-129">id</span><span class="sxs-lookup"><span data-stu-id="5a19c-129">id</span></span>            |`string`      |<span data-ttu-id="5a19c-130">`timeOffReason` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5a19c-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="5a19c-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5a19c-131">displayName</span></span>               | `string`                  | <span data-ttu-id="5a19c-132">**timeOffReason 的名称**。</span><span class="sxs-lookup"><span data-stu-id="5a19c-132">The name of the **timeOffReason**.</span></span> <span data-ttu-id="5a19c-133">必需。</span><span class="sxs-lookup"><span data-stu-id="5a19c-133">Required.</span></span> |
| <span data-ttu-id="5a19c-134">iconType</span><span class="sxs-lookup"><span data-stu-id="5a19c-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="5a19c-135">支持的图标类型：无;car;calendar;running;plane;firstAid;一个notWorking;clock;将duty;globe;cup;phone;weather;umbrella;bankgyBank;dog;一个trafficCone;pin;。</span><span class="sxs-lookup"><span data-stu-id="5a19c-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="5a19c-136">必需。</span><span class="sxs-lookup"><span data-stu-id="5a19c-136">Required.</span></span> |
| <span data-ttu-id="5a19c-137">isActive</span><span class="sxs-lookup"><span data-stu-id="5a19c-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="5a19c-138">指示在创建新实体或更新现有实体时是否可以使用 **timeOffReason。**</span><span class="sxs-lookup"><span data-stu-id="5a19c-138">Indicates whether the **timeOffReason** can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="5a19c-139">必需。</span><span class="sxs-lookup"><span data-stu-id="5a19c-139">Required.</span></span> |
| <span data-ttu-id="5a19c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a19c-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="5a19c-141">首次创建 **此 timeOffReason** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="5a19c-141">The time stamp on which this **timeOffReason** was first created.</span></span> <span data-ttu-id="5a19c-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5a19c-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5a19c-143">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="5a19c-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="5a19c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a19c-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="5a19c-145">上次更新 **TimeOffReason** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="5a19c-145">The time stamp on which this **timeOffReason** was last updated.</span></span> <span data-ttu-id="5a19c-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5a19c-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5a19c-147">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="5a19c-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="5a19c-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5a19c-148">lastModifiedBy</span></span>        | [<span data-ttu-id="5a19c-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a19c-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="5a19c-150">上次更新的标识 **这次是OffReason**。</span><span class="sxs-lookup"><span data-stu-id="5a19c-150">The identity that last updated this **timeOffReason**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a19c-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a19c-151">JSON representation</span></span>

<span data-ttu-id="5a19c-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a19c-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

