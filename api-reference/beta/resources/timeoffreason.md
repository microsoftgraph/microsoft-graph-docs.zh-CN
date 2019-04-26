---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8ba1e4bd596b82643ecbfa4b842e60232c182a4b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341965"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="5acda-103">timeOffReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="5acda-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5acda-104">[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。</span><span class="sxs-lookup"><span data-stu-id="5acda-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5acda-105">方法</span><span class="sxs-lookup"><span data-stu-id="5acda-105">Methods</span></span>

| <span data-ttu-id="5acda-106">方法</span><span class="sxs-lookup"><span data-stu-id="5acda-106">Method</span></span>       | <span data-ttu-id="5acda-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5acda-107">Return Type</span></span>  |<span data-ttu-id="5acda-108">说明</span><span class="sxs-lookup"><span data-stu-id="5acda-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5acda-109">创建 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="5acda-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="5acda-111">新建 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="5acda-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="5acda-112">列出 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="5acda-113">[timeOffReason](timeoffreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="5acda-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="5acda-114">获取计划中 `timeOffReasons` 的列表。</span><span class="sxs-lookup"><span data-stu-id="5acda-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="5acda-115">获取 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="5acda-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="5acda-117">按 ID 获取 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="5acda-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="5acda-118">替换 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="5acda-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="5acda-120">更换 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="5acda-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="5acda-121">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5acda-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="5acda-122">无</span><span class="sxs-lookup"><span data-stu-id="5acda-122">None</span></span> | <span data-ttu-id="5acda-123">将 `timeOffReason` 标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="5acda-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="5acda-124">属性</span><span class="sxs-lookup"><span data-stu-id="5acda-124">Properties</span></span>
|<span data-ttu-id="5acda-125">名称</span><span class="sxs-lookup"><span data-stu-id="5acda-125">Name</span></span>          |<span data-ttu-id="5acda-126">类型</span><span class="sxs-lookup"><span data-stu-id="5acda-126">Type</span></span>           |<span data-ttu-id="5acda-127">说明</span><span class="sxs-lookup"><span data-stu-id="5acda-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="5acda-128">id</span><span class="sxs-lookup"><span data-stu-id="5acda-128">id</span></span>            |`string`      |<span data-ttu-id="5acda-129">`timeOffReason` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5acda-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="5acda-130">displayName</span><span class="sxs-lookup"><span data-stu-id="5acda-130">displayName</span></span>               | `string`                  | <span data-ttu-id="5acda-131">的名称`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="5acda-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="5acda-132">必需。</span><span class="sxs-lookup"><span data-stu-id="5acda-132">Required.</span></span> |
| <span data-ttu-id="5acda-133">iconType</span><span class="sxs-lookup"><span data-stu-id="5acda-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="5acda-134">支持的图标类型: 无;car式运行planefirstAid;dr。notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny。</span><span class="sxs-lookup"><span data-stu-id="5acda-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="5acda-135">必需。</span><span class="sxs-lookup"><span data-stu-id="5acda-135">Required.</span></span> |
| <span data-ttu-id="5acda-136">isActive</span><span class="sxs-lookup"><span data-stu-id="5acda-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="5acda-137">指示在新建实体或更新现有实体时是否可以使用 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="5acda-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="5acda-138">必需。</span><span class="sxs-lookup"><span data-stu-id="5acda-138">Required.</span></span> |
| <span data-ttu-id="5acda-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5acda-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="5acda-140">首次在其上创建`timeOffReason`此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="5acda-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="5acda-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5acda-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5acda-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="5acda-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="5acda-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5acda-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="5acda-144">对其最后更新的`timeOffReason`时间戳。</span><span class="sxs-lookup"><span data-stu-id="5acda-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="5acda-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5acda-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5acda-146">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="5acda-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="5acda-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5acda-147">lastModifiedBy</span></span>        | [<span data-ttu-id="5acda-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="5acda-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="5acda-149">上次更新 `timeOffReason` 的标识。</span><span class="sxs-lookup"><span data-stu-id="5acda-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5acda-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5acda-150">JSON representation</span></span>

<span data-ttu-id="5acda-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5acda-151">Here is a JSON representation of the resource.</span></span>

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
