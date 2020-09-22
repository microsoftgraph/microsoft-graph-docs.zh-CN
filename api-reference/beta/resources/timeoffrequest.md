---
title: timeOffRequest 资源类型
description: 表示要采用 timeoff 的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1b1e6c3f55b716590a399c9324ea759ff93810d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073388"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="17cf9-103">timeOffRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="17cf9-103">timeOffRequest resource type</span></span>

<span data-ttu-id="17cf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17cf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17cf9-105">表示要采用 [timeoff](../resources/timeoff.md)的班次请求的类型。</span><span class="sxs-lookup"><span data-stu-id="17cf9-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="17cf9-106">方法</span><span class="sxs-lookup"><span data-stu-id="17cf9-106">Methods</span></span>

| <span data-ttu-id="17cf9-107">方法</span><span class="sxs-lookup"><span data-stu-id="17cf9-107">Method</span></span>       | <span data-ttu-id="17cf9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="17cf9-108">Return Type</span></span> | <span data-ttu-id="17cf9-109">Description</span><span class="sxs-lookup"><span data-stu-id="17cf9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="17cf9-110">List</span><span class="sxs-lookup"><span data-stu-id="17cf9-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="17cf9-111">[timeOffRequest](timeoffrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17cf9-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="17cf9-112">获取此计划中的 **timeOffRequest** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="17cf9-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="17cf9-113">Get</span><span class="sxs-lookup"><span data-stu-id="17cf9-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="17cf9-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="17cf9-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="17cf9-115">读取 **timeOffRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17cf9-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="17cf9-116">删除</span><span class="sxs-lookup"><span data-stu-id="17cf9-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="17cf9-117">无</span><span class="sxs-lookup"><span data-stu-id="17cf9-117">None</span></span> | <span data-ttu-id="17cf9-118">删除 **timeOffRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="17cf9-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="17cf9-119">批准</span><span class="sxs-lookup"><span data-stu-id="17cf9-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="17cf9-120">无</span><span class="sxs-lookup"><span data-stu-id="17cf9-120">None</span></span>|<span data-ttu-id="17cf9-121">批准请假时间请求。</span><span class="sxs-lookup"><span data-stu-id="17cf9-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="17cf9-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="17cf9-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="17cf9-123">无</span><span class="sxs-lookup"><span data-stu-id="17cf9-123">None</span></span>|<span data-ttu-id="17cf9-124">拒绝休息时间请求。</span><span class="sxs-lookup"><span data-stu-id="17cf9-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="17cf9-125">属性</span><span class="sxs-lookup"><span data-stu-id="17cf9-125">Properties</span></span>

| <span data-ttu-id="17cf9-126">属性</span><span class="sxs-lookup"><span data-stu-id="17cf9-126">Property</span></span>     | <span data-ttu-id="17cf9-127">类型</span><span class="sxs-lookup"><span data-stu-id="17cf9-127">Type</span></span>        | <span data-ttu-id="17cf9-128">说明</span><span class="sxs-lookup"><span data-stu-id="17cf9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17cf9-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="17cf9-129">endDateTime</span></span>|<span data-ttu-id="17cf9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17cf9-130">DateTimeOffset</span></span>|<span data-ttu-id="17cf9-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="17cf9-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="17cf9-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="17cf9-133">startDateTime</span></span>|<span data-ttu-id="17cf9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17cf9-134">DateTimeOffset</span></span>|<span data-ttu-id="17cf9-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="17cf9-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="17cf9-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="17cf9-137">timeOffReasonId</span></span>|<span data-ttu-id="17cf9-138">String</span><span class="sxs-lookup"><span data-stu-id="17cf9-138">String</span></span>|<span data-ttu-id="17cf9-139">休息时间的原因。</span><span class="sxs-lookup"><span data-stu-id="17cf9-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17cf9-140">关系</span><span class="sxs-lookup"><span data-stu-id="17cf9-140">Relationships</span></span>

<span data-ttu-id="17cf9-141">无。</span><span class="sxs-lookup"><span data-stu-id="17cf9-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17cf9-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17cf9-142">JSON representation</span></span>

<span data-ttu-id="17cf9-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17cf9-143">The following is a JSON representation of the resource.</span></span>

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


