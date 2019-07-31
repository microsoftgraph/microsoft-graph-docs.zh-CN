---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 62943670a0c87d34fd849e988ef5bf827aa6d72a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964279"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="57020-103">timeOffReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="57020-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57020-104">[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。</span><span class="sxs-lookup"><span data-stu-id="57020-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="57020-105">方法</span><span class="sxs-lookup"><span data-stu-id="57020-105">Methods</span></span>

| <span data-ttu-id="57020-106">方法</span><span class="sxs-lookup"><span data-stu-id="57020-106">Method</span></span>       | <span data-ttu-id="57020-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="57020-107">Return Type</span></span>  |<span data-ttu-id="57020-108">说明</span><span class="sxs-lookup"><span data-stu-id="57020-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="57020-109">创建 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="57020-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="57020-111">新建 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="57020-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="57020-112">列出 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="57020-113">[timeOffReason](timeoffreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="57020-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="57020-114">获取计划中 `timeOffReasons` 的列表。</span><span class="sxs-lookup"><span data-stu-id="57020-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="57020-115">获取 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="57020-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="57020-117">按 ID 获取 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="57020-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="57020-118">替换 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="57020-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="57020-120">更换 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="57020-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="57020-121">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="57020-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="57020-122">无</span><span class="sxs-lookup"><span data-stu-id="57020-122">None</span></span> | <span data-ttu-id="57020-123">将 `timeOffReason` 标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="57020-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="57020-124">属性</span><span class="sxs-lookup"><span data-stu-id="57020-124">Properties</span></span>
|<span data-ttu-id="57020-125">名称</span><span class="sxs-lookup"><span data-stu-id="57020-125">Name</span></span>          |<span data-ttu-id="57020-126">类型</span><span class="sxs-lookup"><span data-stu-id="57020-126">Type</span></span>           |<span data-ttu-id="57020-127">说明</span><span class="sxs-lookup"><span data-stu-id="57020-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="57020-128">id</span><span class="sxs-lookup"><span data-stu-id="57020-128">id</span></span>            |`string`      |<span data-ttu-id="57020-129">`timeOffReason` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="57020-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="57020-130">displayName</span><span class="sxs-lookup"><span data-stu-id="57020-130">displayName</span></span>               | `string`                  | <span data-ttu-id="57020-131">的名称`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="57020-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="57020-132">必需。</span><span class="sxs-lookup"><span data-stu-id="57020-132">Required.</span></span> |
| <span data-ttu-id="57020-133">iconType</span><span class="sxs-lookup"><span data-stu-id="57020-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="57020-134">支持的图标类型: 无;car式运行planefirstAid;dr.notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny.</span><span class="sxs-lookup"><span data-stu-id="57020-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="57020-135">必需。</span><span class="sxs-lookup"><span data-stu-id="57020-135">Required.</span></span> |
| <span data-ttu-id="57020-136">isActive</span><span class="sxs-lookup"><span data-stu-id="57020-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="57020-137">指示在新建实体或更新现有实体时是否可以使用 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="57020-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="57020-138">必需。</span><span class="sxs-lookup"><span data-stu-id="57020-138">Required.</span></span> |
| <span data-ttu-id="57020-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57020-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="57020-140">首次在其上创建`timeOffReason`此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="57020-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="57020-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="57020-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="57020-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="57020-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="57020-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57020-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="57020-144">对其最后更新的`timeOffReason`时间戳。</span><span class="sxs-lookup"><span data-stu-id="57020-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="57020-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="57020-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="57020-146">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="57020-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="57020-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="57020-147">lastModifiedBy</span></span>        | [<span data-ttu-id="57020-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="57020-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="57020-149">上次更新 `timeOffReason` 的标识。</span><span class="sxs-lookup"><span data-stu-id="57020-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57020-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57020-150">JSON representation</span></span>

<span data-ttu-id="57020-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57020-151">Here is a JSON representation of the resource.</span></span>

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
