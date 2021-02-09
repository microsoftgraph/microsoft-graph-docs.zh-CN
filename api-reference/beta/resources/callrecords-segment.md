---
title: 段资源类型
description: 线段类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef965bcfb10eeafd0a2c4f58351aa74650abcd05
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159638"
---
# <a name="segment-resource-type"></a><span data-ttu-id="0e10e-103">段资源类型</span><span class="sxs-lookup"><span data-stu-id="0e10e-103">segment resource type</span></span>

<span data-ttu-id="0e10e-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0e10e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e10e-105">表示电话会议User-User通信或User-Meeting通信的一部分。</span><span class="sxs-lookup"><span data-stu-id="0e10e-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="0e10e-106">典型 VOIP 呼叫将每个会话具有一个段。</span><span class="sxs-lookup"><span data-stu-id="0e10e-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="0e10e-107">在某些情况下（如 PSTN 呼叫）中，由于连接呼叫需要其他服务器到服务器通信，因此每个会话将有多个分段。</span><span class="sxs-lookup"><span data-stu-id="0e10e-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="0e10e-108">方法</span><span class="sxs-lookup"><span data-stu-id="0e10e-108">Methods</span></span>

<span data-ttu-id="0e10e-109">不存在直接访问线段的方法。</span><span class="sxs-lookup"><span data-stu-id="0e10e-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="0e10e-110">Please use the [get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the List [session](../api/callrecords-session-list.md) api with to get the segments for `$expand=segments` a [callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="0e10e-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0e10e-111">属性</span><span class="sxs-lookup"><span data-stu-id="0e10e-111">Properties</span></span>

| <span data-ttu-id="0e10e-112">属性</span><span class="sxs-lookup"><span data-stu-id="0e10e-112">Property</span></span>     | <span data-ttu-id="0e10e-113">类型</span><span class="sxs-lookup"><span data-stu-id="0e10e-113">Type</span></span>        | <span data-ttu-id="0e10e-114">说明</span><span class="sxs-lookup"><span data-stu-id="0e10e-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e10e-115">id</span><span class="sxs-lookup"><span data-stu-id="0e10e-115">id</span></span>|<span data-ttu-id="0e10e-116">String</span><span class="sxs-lookup"><span data-stu-id="0e10e-116">String</span></span>|<span data-ttu-id="0e10e-117">线段的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e10e-117">Unique identifier for the segment.</span></span> <span data-ttu-id="0e10e-118">只读。</span><span class="sxs-lookup"><span data-stu-id="0e10e-118">Read-only.</span></span>|
|<span data-ttu-id="0e10e-119">调用方</span><span class="sxs-lookup"><span data-stu-id="0e10e-119">caller</span></span>|[<span data-ttu-id="0e10e-120">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="0e10e-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="0e10e-121">启动此段的终结点。</span><span class="sxs-lookup"><span data-stu-id="0e10e-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="0e10e-122">被叫方</span><span class="sxs-lookup"><span data-stu-id="0e10e-122">callee</span></span>|[<span data-ttu-id="0e10e-123">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="0e10e-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="0e10e-124">应答此段的终结点。</span><span class="sxs-lookup"><span data-stu-id="0e10e-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="0e10e-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="0e10e-125">failureInfo</span></span>|[<span data-ttu-id="0e10e-126">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="0e10e-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="0e10e-127">与该段关联的失败信息（如果失败）。</span><span class="sxs-lookup"><span data-stu-id="0e10e-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="0e10e-128">media</span><span class="sxs-lookup"><span data-stu-id="0e10e-128">media</span></span>|<span data-ttu-id="0e10e-129">[microsoft.graph.callRecords.media](callrecords-media.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e10e-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="0e10e-130">与此段关联的媒体。</span><span class="sxs-lookup"><span data-stu-id="0e10e-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="0e10e-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0e10e-131">startDateTime</span></span>|<span data-ttu-id="0e10e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e10e-132">DateTimeOffset</span></span>|<span data-ttu-id="0e10e-133">段开始的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e10e-133">UTC time when the segment started.</span></span> <span data-ttu-id="0e10e-134">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e10e-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e10e-135">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0e10e-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0e10e-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0e10e-136">endDateTime</span></span>|<span data-ttu-id="0e10e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e10e-137">DateTimeOffset</span></span>|<span data-ttu-id="0e10e-138">段结束时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e10e-138">UTC time when the segment ended.</span></span> <span data-ttu-id="0e10e-139">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e10e-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e10e-140">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0e10e-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e10e-141">关系</span><span class="sxs-lookup"><span data-stu-id="0e10e-141">Relationships</span></span>

<span data-ttu-id="0e10e-142">无</span><span class="sxs-lookup"><span data-stu-id="0e10e-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e10e-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e10e-143">JSON representation</span></span>

<span data-ttu-id="0e10e-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e10e-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
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

