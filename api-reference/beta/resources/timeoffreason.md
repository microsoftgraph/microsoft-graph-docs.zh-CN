---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f9d84ae6b86d7d97af5ec2376879a5961da7367b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519720"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="baddf-103">timeOffReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="baddf-103">timeOffReason resource type</span></span>

<span data-ttu-id="baddf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="baddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baddf-105">[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。</span><span class="sxs-lookup"><span data-stu-id="baddf-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="baddf-106">方法</span><span class="sxs-lookup"><span data-stu-id="baddf-106">Methods</span></span>

| <span data-ttu-id="baddf-107">方法</span><span class="sxs-lookup"><span data-stu-id="baddf-107">Method</span></span>       | <span data-ttu-id="baddf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="baddf-108">Return Type</span></span>  |<span data-ttu-id="baddf-109">说明</span><span class="sxs-lookup"><span data-stu-id="baddf-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="baddf-110">Create</span><span class="sxs-lookup"><span data-stu-id="baddf-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="baddf-111">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="baddf-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="baddf-112">创建新的**timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="baddf-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="baddf-113">List</span><span class="sxs-lookup"><span data-stu-id="baddf-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="baddf-114">[timeOffReason](timeoffreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="baddf-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="baddf-115">获取计划中的**timeOffReason**列表。</span><span class="sxs-lookup"><span data-stu-id="baddf-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="baddf-116">获取</span><span class="sxs-lookup"><span data-stu-id="baddf-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="baddf-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="baddf-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="baddf-118">按 ID 获取**timeOffReason** 。</span><span class="sxs-lookup"><span data-stu-id="baddf-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="baddf-119">Replace</span><span class="sxs-lookup"><span data-stu-id="baddf-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="baddf-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="baddf-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="baddf-121">替换**timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="baddf-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="baddf-122">删除</span><span class="sxs-lookup"><span data-stu-id="baddf-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="baddf-123">无</span><span class="sxs-lookup"><span data-stu-id="baddf-123">None</span></span> | <span data-ttu-id="baddf-124">将**timeOffReason**标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="baddf-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="baddf-125">属性</span><span class="sxs-lookup"><span data-stu-id="baddf-125">Properties</span></span>
|<span data-ttu-id="baddf-126">名称</span><span class="sxs-lookup"><span data-stu-id="baddf-126">Name</span></span>          |<span data-ttu-id="baddf-127">类型</span><span class="sxs-lookup"><span data-stu-id="baddf-127">Type</span></span>           |<span data-ttu-id="baddf-128">说明</span><span class="sxs-lookup"><span data-stu-id="baddf-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="baddf-129">id</span><span class="sxs-lookup"><span data-stu-id="baddf-129">id</span></span>            |`string`      |<span data-ttu-id="baddf-130">`timeOffReason` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="baddf-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="baddf-131">displayName</span><span class="sxs-lookup"><span data-stu-id="baddf-131">displayName</span></span>               | `string`                  | <span data-ttu-id="baddf-132">的名称`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="baddf-132">The name of the `timeOffReason`.</span></span> <span data-ttu-id="baddf-133">必填。</span><span class="sxs-lookup"><span data-stu-id="baddf-133">Required.</span></span> |
| <span data-ttu-id="baddf-134">iconType</span><span class="sxs-lookup"><span data-stu-id="baddf-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="baddf-135">支持的图标类型：无;car式运行planefirstAid;dr.notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny.</span><span class="sxs-lookup"><span data-stu-id="baddf-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="baddf-136">必填。</span><span class="sxs-lookup"><span data-stu-id="baddf-136">Required.</span></span> |
| <span data-ttu-id="baddf-137">isActive</span><span class="sxs-lookup"><span data-stu-id="baddf-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="baddf-138">指示在新建实体或更新现有实体时是否可以使用 `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="baddf-138">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="baddf-139">必需。</span><span class="sxs-lookup"><span data-stu-id="baddf-139">Required.</span></span> |
| <span data-ttu-id="baddf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="baddf-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="baddf-141">首次在其上创建`timeOffReason`此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="baddf-141">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="baddf-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="baddf-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="baddf-143">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="baddf-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="baddf-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baddf-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="baddf-145">对其最后更新的`timeOffReason`时间戳。</span><span class="sxs-lookup"><span data-stu-id="baddf-145">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="baddf-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="baddf-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="baddf-147">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="baddf-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="baddf-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="baddf-148">lastModifiedBy</span></span>        | [<span data-ttu-id="baddf-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="baddf-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="baddf-150">上次更新 `timeOffReason` 的标识。</span><span class="sxs-lookup"><span data-stu-id="baddf-150">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="baddf-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baddf-151">JSON representation</span></span>

<span data-ttu-id="baddf-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baddf-152">Here is a JSON representation of the resource.</span></span>

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
