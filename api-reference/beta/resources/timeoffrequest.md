---
title: timeOffRequest 资源类型
description: 表示一种要休息的班次请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31d855f21164f933fe27acc824759cee08e16c16
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786066"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="79cfd-103">timeOffRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="79cfd-103">timeOffRequest resource type</span></span>

<span data-ttu-id="79cfd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79cfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79cfd-105">表示一种班次请求采取 [时间Off](../resources/timeoff.md)。</span><span class="sxs-lookup"><span data-stu-id="79cfd-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="79cfd-106">方法</span><span class="sxs-lookup"><span data-stu-id="79cfd-106">Methods</span></span>

| <span data-ttu-id="79cfd-107">方法</span><span class="sxs-lookup"><span data-stu-id="79cfd-107">Method</span></span>       | <span data-ttu-id="79cfd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="79cfd-108">Return type</span></span> | <span data-ttu-id="79cfd-109">Description</span><span class="sxs-lookup"><span data-stu-id="79cfd-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="79cfd-110">List</span><span class="sxs-lookup"><span data-stu-id="79cfd-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="79cfd-111">[timeOffRequest](timeoffrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79cfd-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="79cfd-112">获取此 **计划中的 timeOffRequest** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="79cfd-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="79cfd-113">获取</span><span class="sxs-lookup"><span data-stu-id="79cfd-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="79cfd-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="79cfd-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="79cfd-115">读取 **timeOffRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79cfd-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="79cfd-116">删除</span><span class="sxs-lookup"><span data-stu-id="79cfd-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="79cfd-117">无</span><span class="sxs-lookup"><span data-stu-id="79cfd-117">None</span></span> | <span data-ttu-id="79cfd-118">删除 **timeOffRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="79cfd-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="79cfd-119">批准</span><span class="sxs-lookup"><span data-stu-id="79cfd-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="79cfd-120">无</span><span class="sxs-lookup"><span data-stu-id="79cfd-120">None</span></span>|<span data-ttu-id="79cfd-121">批准请假请求。</span><span class="sxs-lookup"><span data-stu-id="79cfd-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="79cfd-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="79cfd-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="79cfd-123">无</span><span class="sxs-lookup"><span data-stu-id="79cfd-123">None</span></span>|<span data-ttu-id="79cfd-124">拒绝请假请求。</span><span class="sxs-lookup"><span data-stu-id="79cfd-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="79cfd-125">属性</span><span class="sxs-lookup"><span data-stu-id="79cfd-125">Properties</span></span>

| <span data-ttu-id="79cfd-126">属性</span><span class="sxs-lookup"><span data-stu-id="79cfd-126">Property</span></span>     | <span data-ttu-id="79cfd-127">类型</span><span class="sxs-lookup"><span data-stu-id="79cfd-127">Type</span></span>        | <span data-ttu-id="79cfd-128">说明</span><span class="sxs-lookup"><span data-stu-id="79cfd-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79cfd-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="79cfd-129">endDateTime</span></span>|<span data-ttu-id="79cfd-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79cfd-130">DateTimeOffset</span></span>|<span data-ttu-id="79cfd-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="79cfd-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79cfd-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="79cfd-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="79cfd-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="79cfd-133">startDateTime</span></span>|<span data-ttu-id="79cfd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79cfd-134">DateTimeOffset</span></span>|<span data-ttu-id="79cfd-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="79cfd-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79cfd-136">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="79cfd-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="79cfd-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="79cfd-137">timeOffReasonId</span></span>|<span data-ttu-id="79cfd-138">String</span><span class="sxs-lookup"><span data-stu-id="79cfd-138">String</span></span>|<span data-ttu-id="79cfd-139">请假的原因。</span><span class="sxs-lookup"><span data-stu-id="79cfd-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79cfd-140">关系</span><span class="sxs-lookup"><span data-stu-id="79cfd-140">Relationships</span></span>

<span data-ttu-id="79cfd-141">无。</span><span class="sxs-lookup"><span data-stu-id="79cfd-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79cfd-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79cfd-142">JSON representation</span></span>

<span data-ttu-id="79cfd-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79cfd-143">The following is a JSON representation of the resource.</span></span>

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


