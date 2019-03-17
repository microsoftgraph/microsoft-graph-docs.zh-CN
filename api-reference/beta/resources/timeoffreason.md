---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657530"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="c4707-103">timeOffReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4707-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4707-104">[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。</span><span class="sxs-lookup"><span data-stu-id="c4707-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c4707-105">方法</span><span class="sxs-lookup"><span data-stu-id="c4707-105">Methods</span></span>

| <span data-ttu-id="c4707-106">方法</span><span class="sxs-lookup"><span data-stu-id="c4707-106">Method</span></span>       | <span data-ttu-id="c4707-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c4707-107">Return Type</span></span>  |<span data-ttu-id="c4707-108">说明</span><span class="sxs-lookup"><span data-stu-id="c4707-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4707-109">创建 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="c4707-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="c4707-111">创建新`timeOffReason`的。</span><span class="sxs-lookup"><span data-stu-id="c4707-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="c4707-112">列出 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="c4707-113">[timeOffReason](timeoffreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="c4707-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="c4707-114">获取日程安排中`timeOffReasons`的列表。</span><span class="sxs-lookup"><span data-stu-id="c4707-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="c4707-115">获取 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="c4707-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="c4707-117">`timeOffReason`按 ID 获取。</span><span class="sxs-lookup"><span data-stu-id="c4707-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="c4707-118">替换 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="c4707-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="c4707-120">替换`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="c4707-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="c4707-121">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c4707-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="c4707-122">无</span><span class="sxs-lookup"><span data-stu-id="c4707-122">None</span></span> | <span data-ttu-id="c4707-123">标记`timeOffReason`为非活动。</span><span class="sxs-lookup"><span data-stu-id="c4707-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4707-124">属性</span><span class="sxs-lookup"><span data-stu-id="c4707-124">Properties</span></span>
|<span data-ttu-id="c4707-125">名称</span><span class="sxs-lookup"><span data-stu-id="c4707-125">Name</span></span>          |<span data-ttu-id="c4707-126">类型</span><span class="sxs-lookup"><span data-stu-id="c4707-126">Type</span></span>           |<span data-ttu-id="c4707-127">说明</span><span class="sxs-lookup"><span data-stu-id="c4707-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="c4707-128">id</span><span class="sxs-lookup"><span data-stu-id="c4707-128">id</span></span>            |`string`      |<span data-ttu-id="c4707-129">的 ID `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="c4707-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="c4707-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c4707-130">displayName</span></span>               | `string`                  | <span data-ttu-id="c4707-131">的名称`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="c4707-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="c4707-132">必需。</span><span class="sxs-lookup"><span data-stu-id="c4707-132">Required.</span></span> |
| <span data-ttu-id="c4707-133">iconType</span><span class="sxs-lookup"><span data-stu-id="c4707-133">iconType</span></span> | `enum`   | <span data-ttu-id="c4707-134">支持的图标类型: 无;car式运行planefirstAid;dr。notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny。</span><span class="sxs-lookup"><span data-stu-id="c4707-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="c4707-135">必需。</span><span class="sxs-lookup"><span data-stu-id="c4707-135">Required.</span></span> |
| <span data-ttu-id="c4707-136">isActive</span><span class="sxs-lookup"><span data-stu-id="c4707-136">isActive</span></span>          |`bool`      | <span data-ttu-id="c4707-137">指示在创建`timeOffReason`新实体或更新现有实体时是否可以使用此文件。</span><span class="sxs-lookup"><span data-stu-id="c4707-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="c4707-138">必需。</span><span class="sxs-lookup"><span data-stu-id="c4707-138">Required.</span></span> |
| <span data-ttu-id="c4707-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4707-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="c4707-140">首次在其上创建`timeOffReason`此项的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c4707-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="c4707-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c4707-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4707-142">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="c4707-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c4707-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4707-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="c4707-144">对其最后更新的`timeOffReason`时间戳。</span><span class="sxs-lookup"><span data-stu-id="c4707-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="c4707-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c4707-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4707-146">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="c4707-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c4707-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c4707-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="c4707-148">最后更新此`timeOffReason`的标识。</span><span class="sxs-lookup"><span data-stu-id="c4707-148">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4707-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4707-149">JSON representation</span></span>

<span data-ttu-id="c4707-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4707-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
