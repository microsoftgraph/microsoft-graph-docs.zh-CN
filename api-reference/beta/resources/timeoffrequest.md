---
title: timeOffRequest 资源类型
description: 表示一种要休息的班次请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 42ad70594dfc5f5c0491b88c95d88e19e226ec1c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720177"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="73f11-103">timeOffRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="73f11-103">timeOffRequest resource type</span></span>

<span data-ttu-id="73f11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73f11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f11-105">表示一种要休息的班次 [请求类型](../resources/timeoff.md)。</span><span class="sxs-lookup"><span data-stu-id="73f11-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="73f11-106">方法</span><span class="sxs-lookup"><span data-stu-id="73f11-106">Methods</span></span>

| <span data-ttu-id="73f11-107">方法</span><span class="sxs-lookup"><span data-stu-id="73f11-107">Method</span></span>       | <span data-ttu-id="73f11-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="73f11-108">Return Type</span></span> | <span data-ttu-id="73f11-109">Description</span><span class="sxs-lookup"><span data-stu-id="73f11-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="73f11-110">List</span><span class="sxs-lookup"><span data-stu-id="73f11-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="73f11-111">[timeOffRequest](timeoffrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73f11-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="73f11-112">获取此 **计划中的 timeOffRequest** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="73f11-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="73f11-113">获取</span><span class="sxs-lookup"><span data-stu-id="73f11-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="73f11-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="73f11-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="73f11-115">读取 **timeOffRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73f11-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="73f11-116">删除</span><span class="sxs-lookup"><span data-stu-id="73f11-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="73f11-117">无</span><span class="sxs-lookup"><span data-stu-id="73f11-117">None</span></span> | <span data-ttu-id="73f11-118">删除 **timeOffRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="73f11-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="73f11-119">批准</span><span class="sxs-lookup"><span data-stu-id="73f11-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="73f11-120">无</span><span class="sxs-lookup"><span data-stu-id="73f11-120">None</span></span>|<span data-ttu-id="73f11-121">批准请假请求。</span><span class="sxs-lookup"><span data-stu-id="73f11-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="73f11-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="73f11-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="73f11-123">无</span><span class="sxs-lookup"><span data-stu-id="73f11-123">None</span></span>|<span data-ttu-id="73f11-124">拒绝请假请求。</span><span class="sxs-lookup"><span data-stu-id="73f11-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="73f11-125">属性</span><span class="sxs-lookup"><span data-stu-id="73f11-125">Properties</span></span>

| <span data-ttu-id="73f11-126">属性</span><span class="sxs-lookup"><span data-stu-id="73f11-126">Property</span></span>     | <span data-ttu-id="73f11-127">类型</span><span class="sxs-lookup"><span data-stu-id="73f11-127">Type</span></span>        | <span data-ttu-id="73f11-128">说明</span><span class="sxs-lookup"><span data-stu-id="73f11-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73f11-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="73f11-129">endDateTime</span></span>|<span data-ttu-id="73f11-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f11-130">DateTimeOffset</span></span>|<span data-ttu-id="73f11-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="73f11-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73f11-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="73f11-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="73f11-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73f11-133">startDateTime</span></span>|<span data-ttu-id="73f11-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f11-134">DateTimeOffset</span></span>|<span data-ttu-id="73f11-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="73f11-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73f11-136">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="73f11-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="73f11-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="73f11-137">timeOffReasonId</span></span>|<span data-ttu-id="73f11-138">String</span><span class="sxs-lookup"><span data-stu-id="73f11-138">String</span></span>|<span data-ttu-id="73f11-139">请假的原因。</span><span class="sxs-lookup"><span data-stu-id="73f11-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73f11-140">关系</span><span class="sxs-lookup"><span data-stu-id="73f11-140">Relationships</span></span>

<span data-ttu-id="73f11-141">无。</span><span class="sxs-lookup"><span data-stu-id="73f11-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73f11-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73f11-142">JSON representation</span></span>

<span data-ttu-id="73f11-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73f11-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


