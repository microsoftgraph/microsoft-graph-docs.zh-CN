---
title: 会话资源类型
description: 会话类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 837e72c52002c0084994b74d3991c69272bdf870
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721801"
---
# <a name="session-resource-type"></a><span data-ttu-id="a690d-103">会话资源类型</span><span class="sxs-lookup"><span data-stu-id="a690d-103">session resource type</span></span>

<span data-ttu-id="a690d-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="a690d-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="a690d-105">代表User-User电话会议User-Meeting通信的一种通信方式。</span><span class="sxs-lookup"><span data-stu-id="a690d-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="a690d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a690d-106">Methods</span></span>

| <span data-ttu-id="a690d-107">方法</span><span class="sxs-lookup"><span data-stu-id="a690d-107">Method</span></span>       | <span data-ttu-id="a690d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a690d-108">Return Type</span></span> | <span data-ttu-id="a690d-109">说明</span><span class="sxs-lookup"><span data-stu-id="a690d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a690d-110">列表会话</span><span class="sxs-lookup"><span data-stu-id="a690d-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="a690d-111">[microsoft.graph.callRecords.session](callrecords-session.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a690d-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="a690d-112">检索与 [callRecord](callrecords-callrecord.md) 对象关联的会话列表。</span><span class="sxs-lookup"><span data-stu-id="a690d-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="a690d-113">属性</span><span class="sxs-lookup"><span data-stu-id="a690d-113">Properties</span></span>

| <span data-ttu-id="a690d-114">属性</span><span class="sxs-lookup"><span data-stu-id="a690d-114">Property</span></span>     | <span data-ttu-id="a690d-115">类型</span><span class="sxs-lookup"><span data-stu-id="a690d-115">Type</span></span>        | <span data-ttu-id="a690d-116">说明</span><span class="sxs-lookup"><span data-stu-id="a690d-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a690d-117">id</span><span class="sxs-lookup"><span data-stu-id="a690d-117">id</span></span>|<span data-ttu-id="a690d-118">string</span><span class="sxs-lookup"><span data-stu-id="a690d-118">string</span></span>|<span data-ttu-id="a690d-119">会话的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a690d-119">Unique identifier for the session.</span></span> <span data-ttu-id="a690d-120">只读。</span><span class="sxs-lookup"><span data-stu-id="a690d-120">Read-only.</span></span>|
|<span data-ttu-id="a690d-121">呼叫者</span><span class="sxs-lookup"><span data-stu-id="a690d-121">caller</span></span>|[<span data-ttu-id="a690d-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="a690d-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="a690d-123">启动会话的终结点。</span><span class="sxs-lookup"><span data-stu-id="a690d-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="a690d-124">被叫方</span><span class="sxs-lookup"><span data-stu-id="a690d-124">callee</span></span>|[<span data-ttu-id="a690d-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="a690d-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="a690d-126">应答会话的终结点。</span><span class="sxs-lookup"><span data-stu-id="a690d-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="a690d-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="a690d-127">failureInfo</span></span>|[<span data-ttu-id="a690d-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="a690d-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="a690d-129">与会话关联的失败信息（如果会话失败）。</span><span class="sxs-lookup"><span data-stu-id="a690d-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="a690d-130">modalities</span><span class="sxs-lookup"><span data-stu-id="a690d-130">modalities</span></span>|<span data-ttu-id="a690d-131">microsoft.graph.callRecords.modality 集合</span><span class="sxs-lookup"><span data-stu-id="a690d-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="a690d-132">会话中呈现的模态列表。</span><span class="sxs-lookup"><span data-stu-id="a690d-132">List of modalities present in the session.</span></span> <span data-ttu-id="a690d-133">可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a690d-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a690d-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a690d-134">startDateTime</span></span>|<span data-ttu-id="a690d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a690d-135">DateTimeOffset</span></span>|<span data-ttu-id="a690d-136">第一个用户加入会话的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a690d-136">UTC time when the first user joined the session.</span></span> <span data-ttu-id="a690d-137">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a690d-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a690d-138">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a690d-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a690d-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a690d-139">endDateTime</span></span>|<span data-ttu-id="a690d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a690d-140">DateTimeOffset</span></span>|<span data-ttu-id="a690d-141">最后一个用户离开会话的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a690d-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="a690d-142">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a690d-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a690d-143">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a690d-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|


## <a name="relationships"></a><span data-ttu-id="a690d-144">关系</span><span class="sxs-lookup"><span data-stu-id="a690d-144">Relationships</span></span>

| <span data-ttu-id="a690d-145">关系</span><span class="sxs-lookup"><span data-stu-id="a690d-145">Relationship</span></span> | <span data-ttu-id="a690d-146">类型</span><span class="sxs-lookup"><span data-stu-id="a690d-146">Type</span></span>        | <span data-ttu-id="a690d-147">说明</span><span class="sxs-lookup"><span data-stu-id="a690d-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a690d-148">段</span><span class="sxs-lookup"><span data-stu-id="a690d-148">segments</span></span>|<span data-ttu-id="a690d-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a690d-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="a690d-150">会话中涉及的分段列表。</span><span class="sxs-lookup"><span data-stu-id="a690d-150">The list of segments involved in the session.</span></span> <span data-ttu-id="a690d-151">只读。</span><span class="sxs-lookup"><span data-stu-id="a690d-151">Read-only.</span></span> <span data-ttu-id="a690d-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a690d-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a690d-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a690d-153">JSON representation</span></span>

<span data-ttu-id="a690d-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a690d-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
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
