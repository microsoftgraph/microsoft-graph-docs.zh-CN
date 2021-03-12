---
title: timeOffRequest 资源类型
description: 表示一种需要时间关闭的班次请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 76eea937b03f3eb117e6b5f870a316f268df615c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721695"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="a0715-103">timeOffRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0715-103">timeOffRequest resource type</span></span>

<span data-ttu-id="a0715-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0715-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0715-105">表示一种班次请求采取 [时间Off](../resources/timeoff.md)。</span><span class="sxs-lookup"><span data-stu-id="a0715-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a0715-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a0715-106">Methods</span></span>

| <span data-ttu-id="a0715-107">方法</span><span class="sxs-lookup"><span data-stu-id="a0715-107">Method</span></span>       | <span data-ttu-id="a0715-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0715-108">Return Type</span></span> | <span data-ttu-id="a0715-109">说明</span><span class="sxs-lookup"><span data-stu-id="a0715-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a0715-110">获取</span><span class="sxs-lookup"><span data-stu-id="a0715-110">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="a0715-111">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="a0715-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="a0715-112">读取 **timeOffRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0715-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="a0715-113">List</span><span class="sxs-lookup"><span data-stu-id="a0715-113">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="a0715-114">[timeOffRequest](timeoffrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0715-114">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="a0715-115">获取此 **计划中的 timeOffRequest** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="a0715-115">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="a0715-116">删除</span><span class="sxs-lookup"><span data-stu-id="a0715-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="a0715-117">无</span><span class="sxs-lookup"><span data-stu-id="a0715-117">None</span></span> | <span data-ttu-id="a0715-118">删除 **timeOffRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="a0715-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="a0715-119">批准</span><span class="sxs-lookup"><span data-stu-id="a0715-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="a0715-120">无</span><span class="sxs-lookup"><span data-stu-id="a0715-120">None</span></span>|<span data-ttu-id="a0715-121">批准请假请求。</span><span class="sxs-lookup"><span data-stu-id="a0715-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="a0715-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="a0715-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="a0715-123">无</span><span class="sxs-lookup"><span data-stu-id="a0715-123">None</span></span>|<span data-ttu-id="a0715-124">拒绝请假请求。</span><span class="sxs-lookup"><span data-stu-id="a0715-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0715-125">属性</span><span class="sxs-lookup"><span data-stu-id="a0715-125">Properties</span></span>

| <span data-ttu-id="a0715-126">属性</span><span class="sxs-lookup"><span data-stu-id="a0715-126">Property</span></span>     | <span data-ttu-id="a0715-127">类型</span><span class="sxs-lookup"><span data-stu-id="a0715-127">Type</span></span>        | <span data-ttu-id="a0715-128">说明</span><span class="sxs-lookup"><span data-stu-id="a0715-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0715-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a0715-129">endDateTime</span></span>|<span data-ttu-id="a0715-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0715-130">DateTimeOffset</span></span>|<span data-ttu-id="a0715-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a0715-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0715-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a0715-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a0715-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a0715-133">startDateTime</span></span>|<span data-ttu-id="a0715-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0715-134">DateTimeOffset</span></span>|<span data-ttu-id="a0715-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a0715-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0715-136">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a0715-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a0715-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="a0715-137">timeOffReasonId</span></span>|<span data-ttu-id="a0715-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a0715-138">String</span></span>|<span data-ttu-id="a0715-139">请假的原因。</span><span class="sxs-lookup"><span data-stu-id="a0715-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0715-140">关系</span><span class="sxs-lookup"><span data-stu-id="a0715-140">Relationships</span></span>

<span data-ttu-id="a0715-141">无。</span><span class="sxs-lookup"><span data-stu-id="a0715-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0715-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0715-142">JSON representation</span></span>

<span data-ttu-id="a0715-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0715-143">The following is a JSON representation of the resource.</span></span>

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

