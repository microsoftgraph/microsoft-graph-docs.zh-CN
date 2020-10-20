---
title: callRecord 资源类型
description: CallRecord 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cf438689ec873ba915c735fee7ebc2162757f8ff
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601368"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="3fc26-103">callRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="3fc26-103">callRecord resource type</span></span>

<span data-ttu-id="3fc26-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3fc26-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="3fc26-105">代表一个或多个参与者之间的一个对等呼叫或组呼叫（有时称为联机会议）。</span><span class="sxs-lookup"><span data-stu-id="3fc26-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="3fc26-106">方法</span><span class="sxs-lookup"><span data-stu-id="3fc26-106">Methods</span></span>

| <span data-ttu-id="3fc26-107">方法</span><span class="sxs-lookup"><span data-stu-id="3fc26-107">Method</span></span>       | <span data-ttu-id="3fc26-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3fc26-108">Return Type</span></span> | <span data-ttu-id="3fc26-109">说明</span><span class="sxs-lookup"><span data-stu-id="3fc26-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3fc26-110">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="3fc26-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="3fc26-111">callRecords。 callRecord</span><span class="sxs-lookup"><span data-stu-id="3fc26-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="3fc26-112">读取 callRecord 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3fc26-112">Read properties and relationships of callRecord object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3fc26-113">属性</span><span class="sxs-lookup"><span data-stu-id="3fc26-113">Properties</span></span>

| <span data-ttu-id="3fc26-114">属性</span><span class="sxs-lookup"><span data-stu-id="3fc26-114">Property</span></span>     | <span data-ttu-id="3fc26-115">类型</span><span class="sxs-lookup"><span data-stu-id="3fc26-115">Type</span></span>        | <span data-ttu-id="3fc26-116">说明</span><span class="sxs-lookup"><span data-stu-id="3fc26-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fc26-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc26-117">endDateTime</span></span>|<span data-ttu-id="3fc26-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc26-118">DateTimeOffset</span></span>|<span data-ttu-id="3fc26-119">上次用户离开呼叫时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3fc26-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="3fc26-120">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3fc26-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3fc26-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3fc26-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3fc26-122">id</span><span class="sxs-lookup"><span data-stu-id="3fc26-122">id</span></span>|<span data-ttu-id="3fc26-123">String</span><span class="sxs-lookup"><span data-stu-id="3fc26-123">String</span></span>|<span data-ttu-id="3fc26-124">呼叫记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3fc26-124">Unique identifier for the call record.</span></span> <span data-ttu-id="3fc26-125">只读。</span><span class="sxs-lookup"><span data-stu-id="3fc26-125">Read-only.</span></span>|
|<span data-ttu-id="3fc26-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="3fc26-126">joinWebUrl</span></span>|<span data-ttu-id="3fc26-127">String</span><span class="sxs-lookup"><span data-stu-id="3fc26-127">String</span></span>|<span data-ttu-id="3fc26-128">与呼叫关联的会议 URL。</span><span class="sxs-lookup"><span data-stu-id="3fc26-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="3fc26-129">可能不可用于 peerToPeer 呼叫记录类型。</span><span class="sxs-lookup"><span data-stu-id="3fc26-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="3fc26-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc26-130">lastModifiedDateTime</span></span>|<span data-ttu-id="3fc26-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc26-131">DateTimeOffset</span></span>|<span data-ttu-id="3fc26-132">创建呼叫记录时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3fc26-132">UTC time when the call record was created.</span></span> <span data-ttu-id="3fc26-133">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3fc26-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3fc26-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3fc26-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3fc26-135">形式</span><span class="sxs-lookup"><span data-stu-id="3fc26-135">modalities</span></span>|<span data-ttu-id="3fc26-136">callRecords 集合。</span><span class="sxs-lookup"><span data-stu-id="3fc26-136">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="3fc26-137">在呼叫中使用的所有形式的列表。</span><span class="sxs-lookup"><span data-stu-id="3fc26-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="3fc26-138">可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3fc26-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3fc26-139">组织者</span><span class="sxs-lookup"><span data-stu-id="3fc26-139">organizer</span></span>|[<span data-ttu-id="3fc26-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="3fc26-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="3fc26-141">组织方的标识。</span><span class="sxs-lookup"><span data-stu-id="3fc26-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="3fc26-142">participants</span><span class="sxs-lookup"><span data-stu-id="3fc26-142">participants</span></span>|<span data-ttu-id="3fc26-143">[identitySet](identityset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3fc26-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="3fc26-144">呼叫中涉及的不同标识的列表。</span><span class="sxs-lookup"><span data-stu-id="3fc26-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="3fc26-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc26-145">startDateTime</span></span>|<span data-ttu-id="3fc26-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc26-146">DateTimeOffset</span></span>|<span data-ttu-id="3fc26-147">第一个用户加入呼叫时的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3fc26-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="3fc26-148">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3fc26-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3fc26-149">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3fc26-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3fc26-150">type</span><span class="sxs-lookup"><span data-stu-id="3fc26-150">type</span></span>|<span data-ttu-id="3fc26-151">callRecords。 callType</span><span class="sxs-lookup"><span data-stu-id="3fc26-151">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="3fc26-152">指示呼叫的类型。</span><span class="sxs-lookup"><span data-stu-id="3fc26-152">Indicates the type of the call.</span></span> <span data-ttu-id="3fc26-153">可取值为：`unknown`、`groupCall`、`peerToPeer`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3fc26-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3fc26-154">version</span><span class="sxs-lookup"><span data-stu-id="3fc26-154">version</span></span>|<span data-ttu-id="3fc26-155">Int64</span><span class="sxs-lookup"><span data-stu-id="3fc26-155">Int64</span></span>|<span data-ttu-id="3fc26-156">调用记录的单调递增版本。</span><span class="sxs-lookup"><span data-stu-id="3fc26-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="3fc26-157">具有相同 id 的更高版本呼叫记录包括与较低版本相比的其他数据。</span><span class="sxs-lookup"><span data-stu-id="3fc26-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fc26-158">关系</span><span class="sxs-lookup"><span data-stu-id="3fc26-158">Relationships</span></span>

| <span data-ttu-id="3fc26-159">关系</span><span class="sxs-lookup"><span data-stu-id="3fc26-159">Relationship</span></span> | <span data-ttu-id="3fc26-160">类型</span><span class="sxs-lookup"><span data-stu-id="3fc26-160">Type</span></span>        | <span data-ttu-id="3fc26-161">说明</span><span class="sxs-lookup"><span data-stu-id="3fc26-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fc26-162">会话</span><span class="sxs-lookup"><span data-stu-id="3fc26-162">sessions</span></span>|<span data-ttu-id="3fc26-163">[callRecords](callrecords-session.md) 集合的</span><span class="sxs-lookup"><span data-stu-id="3fc26-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="3fc26-164">呼叫中涉及的会话列表。</span><span class="sxs-lookup"><span data-stu-id="3fc26-164">List of sessions involved in the call.</span></span> <span data-ttu-id="3fc26-165">对等呼叫通常仅具有一个会话，而组调用通常每个参与者至少有一个会话。</span><span class="sxs-lookup"><span data-stu-id="3fc26-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="3fc26-166">只读。</span><span class="sxs-lookup"><span data-stu-id="3fc26-166">Read-only.</span></span> <span data-ttu-id="3fc26-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3fc26-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fc26-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3fc26-168">JSON representation</span></span>

<span data-ttu-id="3fc26-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fc26-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": ["string"],
  "organizer": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}],
  "startDateTime": "String (timestamp)",
  "type": "string",
  "version": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
