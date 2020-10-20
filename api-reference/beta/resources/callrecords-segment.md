---
title: 分段资源类型
description: 线段类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84f18568d1890b331d1bedd6d9e7114518fad3cf
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601662"
---
# <a name="segment-resource-type"></a><span data-ttu-id="c1386-103">分段资源类型</span><span class="sxs-lookup"><span data-stu-id="c1386-103">segment resource type</span></span>

<span data-ttu-id="c1386-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="c1386-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1386-105">表示在会议呼叫的情况下 User-User 通信或 User-Meeting 通信的一部分。</span><span class="sxs-lookup"><span data-stu-id="c1386-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="c1386-106">典型的 VOIP 呼叫将每个会话包含一个分段。</span><span class="sxs-lookup"><span data-stu-id="c1386-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="c1386-107">在某些情况下，例如 PSTN 呼叫，由于连接呼叫需要额外的服务器到服务器通信，因此每个会话会有多个分段。</span><span class="sxs-lookup"><span data-stu-id="c1386-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="c1386-108">方法</span><span class="sxs-lookup"><span data-stu-id="c1386-108">Methods</span></span>

<span data-ttu-id="c1386-109">不存在直接访问分段的方法。</span><span class="sxs-lookup"><span data-stu-id="c1386-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="c1386-110">请使用 [Get callRecord](../api/callrecords-callrecord-get.md) api With `$expand=sessions($expand=segments)` 或 [List session](../api/callrecords-session-list.md) api with `$expand=segments` to 获取 [callRecord](callrecords-callrecord.md)的段。</span><span class="sxs-lookup"><span data-stu-id="c1386-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1386-111">属性</span><span class="sxs-lookup"><span data-stu-id="c1386-111">Properties</span></span>

| <span data-ttu-id="c1386-112">属性</span><span class="sxs-lookup"><span data-stu-id="c1386-112">Property</span></span>     | <span data-ttu-id="c1386-113">类型</span><span class="sxs-lookup"><span data-stu-id="c1386-113">Type</span></span>        | <span data-ttu-id="c1386-114">说明</span><span class="sxs-lookup"><span data-stu-id="c1386-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1386-115">id</span><span class="sxs-lookup"><span data-stu-id="c1386-115">id</span></span>|<span data-ttu-id="c1386-116">String</span><span class="sxs-lookup"><span data-stu-id="c1386-116">String</span></span>|<span data-ttu-id="c1386-117">分段的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c1386-117">Unique identifier for the segment.</span></span> <span data-ttu-id="c1386-118">只读。</span><span class="sxs-lookup"><span data-stu-id="c1386-118">Read-only.</span></span>|
|<span data-ttu-id="c1386-119">者</span><span class="sxs-lookup"><span data-stu-id="c1386-119">caller</span></span>|[<span data-ttu-id="c1386-120">callRecords。</span><span class="sxs-lookup"><span data-stu-id="c1386-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="c1386-121">启动了此段的终结点。</span><span class="sxs-lookup"><span data-stu-id="c1386-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="c1386-122">约定</span><span class="sxs-lookup"><span data-stu-id="c1386-122">callee</span></span>|[<span data-ttu-id="c1386-123">callRecords。</span><span class="sxs-lookup"><span data-stu-id="c1386-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="c1386-124">应答此段的终结点。</span><span class="sxs-lookup"><span data-stu-id="c1386-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="c1386-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="c1386-125">failureInfo</span></span>|[<span data-ttu-id="c1386-126">callRecords。 failureInfo</span><span class="sxs-lookup"><span data-stu-id="c1386-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="c1386-127">与分段相关联的失败信息失败。</span><span class="sxs-lookup"><span data-stu-id="c1386-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="c1386-128">media</span><span class="sxs-lookup"><span data-stu-id="c1386-128">media</span></span>|<span data-ttu-id="c1386-129">[Microsoft callRecords](callrecords-media.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1386-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="c1386-130">与此分段关联的媒体。</span><span class="sxs-lookup"><span data-stu-id="c1386-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="c1386-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c1386-131">startDateTime</span></span>|<span data-ttu-id="c1386-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1386-132">DateTimeOffset</span></span>|<span data-ttu-id="c1386-133">段启动时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c1386-133">UTC time when the segment started.</span></span> <span data-ttu-id="c1386-134">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c1386-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1386-135">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c1386-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c1386-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c1386-136">endDateTime</span></span>|<span data-ttu-id="c1386-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1386-137">DateTimeOffset</span></span>|<span data-ttu-id="c1386-138">段结束时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c1386-138">UTC time when the segment ended.</span></span> <span data-ttu-id="c1386-139">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c1386-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1386-140">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c1386-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1386-141">关系</span><span class="sxs-lookup"><span data-stu-id="c1386-141">Relationships</span></span>

<span data-ttu-id="c1386-142">无</span><span class="sxs-lookup"><span data-stu-id="c1386-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1386-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1386-143">JSON representation</span></span>

<span data-ttu-id="c1386-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1386-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "media": [{"@odata.type": "microsoft.graph.callRecords.media"}],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "segment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

