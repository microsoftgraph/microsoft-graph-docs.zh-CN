---
title: timeOffRequest 资源类型
description: 表示要采用 timeoff 的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f27f0ccbd3e73ade95dedca49c15fe1489d773b5
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154379"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="4daf7-103">timeOffRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="4daf7-103">timeOffRequest resource type</span></span>

<span data-ttu-id="4daf7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4daf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4daf7-105">表示要采用[timeoff](../resources/timeoff.md)的班次请求的类型。</span><span class="sxs-lookup"><span data-stu-id="4daf7-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4daf7-106">方法</span><span class="sxs-lookup"><span data-stu-id="4daf7-106">Methods</span></span>

| <span data-ttu-id="4daf7-107">方法</span><span class="sxs-lookup"><span data-stu-id="4daf7-107">Method</span></span>       | <span data-ttu-id="4daf7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4daf7-108">Return Type</span></span> | <span data-ttu-id="4daf7-109">说明</span><span class="sxs-lookup"><span data-stu-id="4daf7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4daf7-110">List</span><span class="sxs-lookup"><span data-stu-id="4daf7-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="4daf7-111">[timeOffRequest](timeoffrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="4daf7-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="4daf7-112">获取此计划中的**timeOffRequest**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4daf7-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="4daf7-113">获取</span><span class="sxs-lookup"><span data-stu-id="4daf7-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="4daf7-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="4daf7-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="4daf7-115">读取**timeOffRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4daf7-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="4daf7-116">删除</span><span class="sxs-lookup"><span data-stu-id="4daf7-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="4daf7-117">None</span><span class="sxs-lookup"><span data-stu-id="4daf7-117">None</span></span> | <span data-ttu-id="4daf7-118">删除**timeOffRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="4daf7-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="4daf7-119">批准</span><span class="sxs-lookup"><span data-stu-id="4daf7-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="4daf7-120">None</span><span class="sxs-lookup"><span data-stu-id="4daf7-120">None</span></span>|<span data-ttu-id="4daf7-121">批准请假时间请求。</span><span class="sxs-lookup"><span data-stu-id="4daf7-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="4daf7-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="4daf7-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="4daf7-123">None</span><span class="sxs-lookup"><span data-stu-id="4daf7-123">None</span></span>|<span data-ttu-id="4daf7-124">拒绝休息时间请求。</span><span class="sxs-lookup"><span data-stu-id="4daf7-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="4daf7-125">属性</span><span class="sxs-lookup"><span data-stu-id="4daf7-125">Properties</span></span>

| <span data-ttu-id="4daf7-126">属性</span><span class="sxs-lookup"><span data-stu-id="4daf7-126">Property</span></span>     | <span data-ttu-id="4daf7-127">类型</span><span class="sxs-lookup"><span data-stu-id="4daf7-127">Type</span></span>        | <span data-ttu-id="4daf7-128">Description</span><span class="sxs-lookup"><span data-stu-id="4daf7-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4daf7-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4daf7-129">endDateTime</span></span>|<span data-ttu-id="4daf7-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4daf7-130">DateTimeOffset</span></span>|<span data-ttu-id="4daf7-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4daf7-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4daf7-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4daf7-133">startDateTime</span></span>|<span data-ttu-id="4daf7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4daf7-134">DateTimeOffset</span></span>|<span data-ttu-id="4daf7-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4daf7-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4daf7-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="4daf7-137">timeOffReasonId</span></span>|<span data-ttu-id="4daf7-138">字符串</span><span class="sxs-lookup"><span data-stu-id="4daf7-138">String</span></span>|<span data-ttu-id="4daf7-139">休息时间的原因。</span><span class="sxs-lookup"><span data-stu-id="4daf7-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4daf7-140">关系</span><span class="sxs-lookup"><span data-stu-id="4daf7-140">Relationships</span></span>

<span data-ttu-id="4daf7-141">无。</span><span class="sxs-lookup"><span data-stu-id="4daf7-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4daf7-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4daf7-142">JSON representation</span></span>

<span data-ttu-id="4daf7-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4daf7-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
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
