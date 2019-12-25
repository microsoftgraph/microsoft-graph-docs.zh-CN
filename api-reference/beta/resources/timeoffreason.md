---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 514ca74bb9826546e95f225e394e8fc07a0f674f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866516"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="b0445-103">timeOffReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0445-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0445-104">[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。</span><span class="sxs-lookup"><span data-stu-id="b0445-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b0445-105">方法</span><span class="sxs-lookup"><span data-stu-id="b0445-105">Methods</span></span>

| <span data-ttu-id="b0445-106">方法</span><span class="sxs-lookup"><span data-stu-id="b0445-106">Method</span></span>       | <span data-ttu-id="b0445-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0445-107">Return Type</span></span>  |<span data-ttu-id="b0445-108">说明</span><span class="sxs-lookup"><span data-stu-id="b0445-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0445-109">Create</span><span class="sxs-lookup"><span data-stu-id="b0445-109">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="b0445-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b0445-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b0445-111">创建新的**timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="b0445-111">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="b0445-112">List</span><span class="sxs-lookup"><span data-stu-id="b0445-112">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="b0445-113">[timeOffReason](timeoffreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0445-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="b0445-114">获取计划中的**timeOffReason**列表。</span><span class="sxs-lookup"><span data-stu-id="b0445-114">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="b0445-115">获取</span><span class="sxs-lookup"><span data-stu-id="b0445-115">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="b0445-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b0445-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b0445-117">按 ID 获取**timeOffReason** 。</span><span class="sxs-lookup"><span data-stu-id="b0445-117">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="b0445-118">Replace</span><span class="sxs-lookup"><span data-stu-id="b0445-118">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="b0445-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b0445-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b0445-120">替换**timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="b0445-120">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="b0445-121">删除</span><span class="sxs-lookup"><span data-stu-id="b0445-121">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="b0445-122">无</span><span class="sxs-lookup"><span data-stu-id="b0445-122">None</span></span> | <span data-ttu-id="b0445-123">将**timeOffReason**标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="b0445-123">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0445-124">属性</span><span class="sxs-lookup"><span data-stu-id="b0445-124">Properties</span></span>
|<span data-ttu-id="b0445-125">名称</span><span class="sxs-lookup"><span data-stu-id="b0445-125">Name</span></span>          |<span data-ttu-id="b0445-126">类型</span><span class="sxs-lookup"><span data-stu-id="b0445-126">Type</span></span>           |<span data-ttu-id="b0445-127">说明</span><span class="sxs-lookup"><span data-stu-id="b0445-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="b0445-128">id</span><span class="sxs-lookup"><span data-stu-id="b0445-128">id</span></span>            |`string`      |<span data-ttu-id="b0445-129">`timeOffReason` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="b0445-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="b0445-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b0445-130">displayName</span></span>               | `string`                  | <span data-ttu-id="b0445-131">的名称`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="b0445-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="b0445-132">必需。</span><span class="sxs-lookup"><span data-stu-id="b0445-132">Required.</span></span> |
| <span data-ttu-id="b0445-133">iconType</span><span class="sxs-lookup"><span data-stu-id="b0445-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="b0445-134">支持的图标类型：无;car式运行planefirstAid;dr.notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny.</span><span class="sxs-lookup"><span data-stu-id="b0445-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="b0445-135">必需。</span><span class="sxs-lookup"><span data-stu-id="b0445-135">Required.</span></span> |
| <span data-ttu-id="b0445-136">isActive</span><span class="sxs-lookup"><span data-stu-id="b0445-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="b0445-137">指示在新建实体或更新现有实体时是否可以使用 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="b0445-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="b0445-138">必需。</span><span class="sxs-lookup"><span data-stu-id="b0445-138">Required.</span></span> |
| <span data-ttu-id="b0445-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0445-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b0445-140">首次在其上创建`timeOffReason`此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="b0445-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="b0445-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b0445-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0445-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="b0445-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b0445-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0445-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="b0445-144">对其最后更新的`timeOffReason`时间戳。</span><span class="sxs-lookup"><span data-stu-id="b0445-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="b0445-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b0445-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0445-146">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="b0445-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b0445-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b0445-147">lastModifiedBy</span></span>        | [<span data-ttu-id="b0445-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="b0445-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="b0445-149">上次更新 `timeOffReason` 的标识。</span><span class="sxs-lookup"><span data-stu-id="b0445-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0445-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0445-150">JSON representation</span></span>

<span data-ttu-id="b0445-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0445-151">Here is a JSON representation of the resource.</span></span>

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
