---
title: 会话资源类型
description: 会话类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8c1af52332c5650123d604b8e405bf88d0c2f965
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353123"
---
# <a name="session-resource-type"></a><span data-ttu-id="3214d-103">会话资源类型</span><span class="sxs-lookup"><span data-stu-id="3214d-103">session resource type</span></span>

<span data-ttu-id="3214d-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3214d-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3214d-105">表示在召开会议呼叫时的用户用户通信或用户会议通信。</span><span class="sxs-lookup"><span data-stu-id="3214d-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="3214d-106">方法</span><span class="sxs-lookup"><span data-stu-id="3214d-106">Methods</span></span>

<span data-ttu-id="3214d-107">不存在直接访问会话的方法。</span><span class="sxs-lookup"><span data-stu-id="3214d-107">No methods exist to directly access sessions.</span></span> <span data-ttu-id="3214d-108">请使用[Get callRecord](../api/callrecords-callrecord-get.md) api With `$expand=sessions` 获取[callRecord](callrecords-callrecord.md)的会话。</span><span class="sxs-lookup"><span data-stu-id="3214d-108">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions` to get the sessions for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3214d-109">属性</span><span class="sxs-lookup"><span data-stu-id="3214d-109">Properties</span></span>

| <span data-ttu-id="3214d-110">属性</span><span class="sxs-lookup"><span data-stu-id="3214d-110">Property</span></span>     | <span data-ttu-id="3214d-111">类型</span><span class="sxs-lookup"><span data-stu-id="3214d-111">Type</span></span>        | <span data-ttu-id="3214d-112">说明</span><span class="sxs-lookup"><span data-stu-id="3214d-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3214d-113">id</span><span class="sxs-lookup"><span data-stu-id="3214d-113">id</span></span>|<span data-ttu-id="3214d-114">string</span><span class="sxs-lookup"><span data-stu-id="3214d-114">string</span></span>|<span data-ttu-id="3214d-115">会话的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3214d-115">Unique identifier for the session.</span></span> <span data-ttu-id="3214d-116">只读。</span><span class="sxs-lookup"><span data-stu-id="3214d-116">Read-only.</span></span>|
|<span data-ttu-id="3214d-117">者</span><span class="sxs-lookup"><span data-stu-id="3214d-117">caller</span></span>|[<span data-ttu-id="3214d-118">callRecords。</span><span class="sxs-lookup"><span data-stu-id="3214d-118">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="3214d-119">启动会话的终结点。</span><span class="sxs-lookup"><span data-stu-id="3214d-119">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="3214d-120">约定</span><span class="sxs-lookup"><span data-stu-id="3214d-120">callee</span></span>|[<span data-ttu-id="3214d-121">callRecords。</span><span class="sxs-lookup"><span data-stu-id="3214d-121">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="3214d-122">应答会话的终结点。</span><span class="sxs-lookup"><span data-stu-id="3214d-122">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="3214d-123">failureInfo</span><span class="sxs-lookup"><span data-stu-id="3214d-123">failureInfo</span></span>|[<span data-ttu-id="3214d-124">callRecords。 failureInfo</span><span class="sxs-lookup"><span data-stu-id="3214d-124">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="3214d-125">会话失败时与会话关联的失败信息。</span><span class="sxs-lookup"><span data-stu-id="3214d-125">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="3214d-126">形式</span><span class="sxs-lookup"><span data-stu-id="3214d-126">modalities</span></span>|<span data-ttu-id="3214d-127">callRecords 集合。</span><span class="sxs-lookup"><span data-stu-id="3214d-127">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="3214d-128">会话中存在的形式的列表。</span><span class="sxs-lookup"><span data-stu-id="3214d-128">List of modalities present in the session.</span></span> <span data-ttu-id="3214d-129">可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3214d-129">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3214d-130">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3214d-130">startDateTime</span></span>|<span data-ttu-id="3214d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3214d-131">DateTimeOffset</span></span>|<span data-ttu-id="3214d-132">当第一个用户加入会话时，UTC fime。</span><span class="sxs-lookup"><span data-stu-id="3214d-132">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="3214d-133">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3214d-133">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3214d-134">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3214d-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3214d-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3214d-135">endDateTime</span></span>|<span data-ttu-id="3214d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3214d-136">DateTimeOffset</span></span>|<span data-ttu-id="3214d-137">上次用户离开会话时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3214d-137">UTC time when the last user left the session.</span></span> <span data-ttu-id="3214d-138">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3214d-138">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3214d-139">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3214d-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="3214d-140">关系</span><span class="sxs-lookup"><span data-stu-id="3214d-140">Relationships</span></span>

| <span data-ttu-id="3214d-141">关系</span><span class="sxs-lookup"><span data-stu-id="3214d-141">Relationship</span></span> | <span data-ttu-id="3214d-142">类型</span><span class="sxs-lookup"><span data-stu-id="3214d-142">Type</span></span>        | <span data-ttu-id="3214d-143">说明</span><span class="sxs-lookup"><span data-stu-id="3214d-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3214d-144">段</span><span class="sxs-lookup"><span data-stu-id="3214d-144">segments</span></span>|<span data-ttu-id="3214d-145">[callRecords 集合。](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="3214d-145">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="3214d-146">会话中涉及的段的列表。</span><span class="sxs-lookup"><span data-stu-id="3214d-146">The list of segments involved in the session.</span></span> <span data-ttu-id="3214d-147">只读。</span><span class="sxs-lookup"><span data-stu-id="3214d-147">Read-only.</span></span> <span data-ttu-id="3214d-148">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3214d-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3214d-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3214d-149">JSON representation</span></span>

<span data-ttu-id="3214d-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3214d-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "modalities": ["string"],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "session resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->