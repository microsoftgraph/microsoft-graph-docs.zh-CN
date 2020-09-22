---
title: 会话资源类型
description: 会话类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5c31acb452b8d30763e8ba0500354c9b6d6bbbfc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046887"
---
# <a name="session-resource-type"></a><span data-ttu-id="2a010-103">会话资源类型</span><span class="sxs-lookup"><span data-stu-id="2a010-103">session resource type</span></span>

<span data-ttu-id="2a010-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="2a010-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a010-105">表示在召开会议呼叫时的用户用户通信或用户会议通信。</span><span class="sxs-lookup"><span data-stu-id="2a010-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="2a010-106">方法</span><span class="sxs-lookup"><span data-stu-id="2a010-106">Methods</span></span>

| <span data-ttu-id="2a010-107">方法</span><span class="sxs-lookup"><span data-stu-id="2a010-107">Method</span></span>       | <span data-ttu-id="2a010-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a010-108">Return Type</span></span> | <span data-ttu-id="2a010-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a010-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2a010-110">列表会话</span><span class="sxs-lookup"><span data-stu-id="2a010-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="2a010-111">[callRecords](callrecords-session.md) 集合的</span><span class="sxs-lookup"><span data-stu-id="2a010-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="2a010-112">检索与 [callRecord](callrecords-callrecord.md) 对象相关联的会话列表。</span><span class="sxs-lookup"><span data-stu-id="2a010-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="2a010-113">属性</span><span class="sxs-lookup"><span data-stu-id="2a010-113">Properties</span></span>

| <span data-ttu-id="2a010-114">属性</span><span class="sxs-lookup"><span data-stu-id="2a010-114">Property</span></span>     | <span data-ttu-id="2a010-115">类型</span><span class="sxs-lookup"><span data-stu-id="2a010-115">Type</span></span>        | <span data-ttu-id="2a010-116">说明</span><span class="sxs-lookup"><span data-stu-id="2a010-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a010-117">id</span><span class="sxs-lookup"><span data-stu-id="2a010-117">id</span></span>|<span data-ttu-id="2a010-118">string</span><span class="sxs-lookup"><span data-stu-id="2a010-118">string</span></span>|<span data-ttu-id="2a010-119">会话的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a010-119">Unique identifier for the session.</span></span> <span data-ttu-id="2a010-120">只读。</span><span class="sxs-lookup"><span data-stu-id="2a010-120">Read-only.</span></span>|
|<span data-ttu-id="2a010-121">者</span><span class="sxs-lookup"><span data-stu-id="2a010-121">caller</span></span>|[<span data-ttu-id="2a010-122">callRecords。</span><span class="sxs-lookup"><span data-stu-id="2a010-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="2a010-123">启动会话的终结点。</span><span class="sxs-lookup"><span data-stu-id="2a010-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="2a010-124">约定</span><span class="sxs-lookup"><span data-stu-id="2a010-124">callee</span></span>|[<span data-ttu-id="2a010-125">callRecords。</span><span class="sxs-lookup"><span data-stu-id="2a010-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="2a010-126">应答会话的终结点。</span><span class="sxs-lookup"><span data-stu-id="2a010-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="2a010-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="2a010-127">failureInfo</span></span>|[<span data-ttu-id="2a010-128">callRecords。 failureInfo</span><span class="sxs-lookup"><span data-stu-id="2a010-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="2a010-129">会话失败时与会话关联的失败信息。</span><span class="sxs-lookup"><span data-stu-id="2a010-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="2a010-130">形式</span><span class="sxs-lookup"><span data-stu-id="2a010-130">modalities</span></span>|<span data-ttu-id="2a010-131">callRecords 集合。</span><span class="sxs-lookup"><span data-stu-id="2a010-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="2a010-132">会话中存在的形式的列表。</span><span class="sxs-lookup"><span data-stu-id="2a010-132">List of modalities present in the session.</span></span> <span data-ttu-id="2a010-133">可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a010-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2a010-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2a010-134">startDateTime</span></span>|<span data-ttu-id="2a010-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a010-135">DateTimeOffset</span></span>|<span data-ttu-id="2a010-136">当第一个用户加入会话时，UTC fime。</span><span class="sxs-lookup"><span data-stu-id="2a010-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="2a010-137">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2a010-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a010-138">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2a010-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2a010-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2a010-139">endDateTime</span></span>|<span data-ttu-id="2a010-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a010-140">DateTimeOffset</span></span>|<span data-ttu-id="2a010-141">上次用户离开会话时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2a010-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="2a010-142">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2a010-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a010-143">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2a010-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="2a010-144">关系</span><span class="sxs-lookup"><span data-stu-id="2a010-144">Relationships</span></span>

| <span data-ttu-id="2a010-145">关系</span><span class="sxs-lookup"><span data-stu-id="2a010-145">Relationship</span></span> | <span data-ttu-id="2a010-146">类型</span><span class="sxs-lookup"><span data-stu-id="2a010-146">Type</span></span>        | <span data-ttu-id="2a010-147">说明</span><span class="sxs-lookup"><span data-stu-id="2a010-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a010-148">段</span><span class="sxs-lookup"><span data-stu-id="2a010-148">segments</span></span>|<span data-ttu-id="2a010-149">[callRecords 集合。](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="2a010-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="2a010-150">会话中涉及的段的列表。</span><span class="sxs-lookup"><span data-stu-id="2a010-150">The list of segments involved in the session.</span></span> <span data-ttu-id="2a010-151">只读。</span><span class="sxs-lookup"><span data-stu-id="2a010-151">Read-only.</span></span> <span data-ttu-id="2a010-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2a010-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a010-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a010-153">JSON representation</span></span>

<span data-ttu-id="2a010-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a010-154">The following is a JSON representation of the resource.</span></span>

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

