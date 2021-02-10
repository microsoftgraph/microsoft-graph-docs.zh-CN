---
title: callRecord 资源类型
description: callRecord 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc1f6498abe52386ccf8aaa67a542adb891b60bb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159407"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="941b2-103">callRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="941b2-103">callRecord resource type</span></span>

<span data-ttu-id="941b2-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="941b2-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="941b2-105">表示多个参与者之间的单个对等呼叫或组呼叫，有时称为联机会议。</span><span class="sxs-lookup"><span data-stu-id="941b2-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="941b2-106">方法</span><span class="sxs-lookup"><span data-stu-id="941b2-106">Methods</span></span>

| <span data-ttu-id="941b2-107">方法</span><span class="sxs-lookup"><span data-stu-id="941b2-107">Method</span></span>       | <span data-ttu-id="941b2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="941b2-108">Return Type</span></span> | <span data-ttu-id="941b2-109">说明</span><span class="sxs-lookup"><span data-stu-id="941b2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="941b2-110">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="941b2-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="941b2-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="941b2-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="941b2-112">读取 callRecord 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="941b2-112">Read properties and relationships of callRecord object.</span></span> |

## <a name="properties"></a><span data-ttu-id="941b2-113">属性</span><span class="sxs-lookup"><span data-stu-id="941b2-113">Properties</span></span>

| <span data-ttu-id="941b2-114">属性</span><span class="sxs-lookup"><span data-stu-id="941b2-114">Property</span></span>     | <span data-ttu-id="941b2-115">类型</span><span class="sxs-lookup"><span data-stu-id="941b2-115">Type</span></span>        | <span data-ttu-id="941b2-116">说明</span><span class="sxs-lookup"><span data-stu-id="941b2-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="941b2-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="941b2-117">endDateTime</span></span>|<span data-ttu-id="941b2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="941b2-118">DateTimeOffset</span></span>|<span data-ttu-id="941b2-119">最后一个用户离开呼叫的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="941b2-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="941b2-120">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="941b2-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="941b2-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="941b2-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="941b2-122">id</span><span class="sxs-lookup"><span data-stu-id="941b2-122">id</span></span>|<span data-ttu-id="941b2-123">String</span><span class="sxs-lookup"><span data-stu-id="941b2-123">String</span></span>|<span data-ttu-id="941b2-124">呼叫记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="941b2-124">Unique identifier for the call record.</span></span> <span data-ttu-id="941b2-125">只读。</span><span class="sxs-lookup"><span data-stu-id="941b2-125">Read-only.</span></span>|
|<span data-ttu-id="941b2-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="941b2-126">joinWebUrl</span></span>|<span data-ttu-id="941b2-127">String</span><span class="sxs-lookup"><span data-stu-id="941b2-127">String</span></span>|<span data-ttu-id="941b2-128">与呼叫关联的会议 URL。</span><span class="sxs-lookup"><span data-stu-id="941b2-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="941b2-129">peerToPeer 呼叫记录类型可能不可用。</span><span class="sxs-lookup"><span data-stu-id="941b2-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="941b2-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="941b2-130">lastModifiedDateTime</span></span>|<span data-ttu-id="941b2-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="941b2-131">DateTimeOffset</span></span>|<span data-ttu-id="941b2-132">创建呼叫记录时 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="941b2-132">UTC time when the call record was created.</span></span> <span data-ttu-id="941b2-133">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="941b2-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="941b2-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="941b2-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="941b2-135">modalities</span><span class="sxs-lookup"><span data-stu-id="941b2-135">modalities</span></span>|<span data-ttu-id="941b2-136">microsoft.graph.callRecords.modality 集合</span><span class="sxs-lookup"><span data-stu-id="941b2-136">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="941b2-137">调用中使用的所有形式的列表。</span><span class="sxs-lookup"><span data-stu-id="941b2-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="941b2-138">可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="941b2-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="941b2-139">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="941b2-139">organizer</span></span>|[<span data-ttu-id="941b2-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="941b2-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="941b2-141">组织方的身份。</span><span class="sxs-lookup"><span data-stu-id="941b2-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="941b2-142">participants</span><span class="sxs-lookup"><span data-stu-id="941b2-142">participants</span></span>|<span data-ttu-id="941b2-143">[identitySet](identityset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="941b2-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="941b2-144">调用中涉及的不同标识的列表。</span><span class="sxs-lookup"><span data-stu-id="941b2-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="941b2-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="941b2-145">startDateTime</span></span>|<span data-ttu-id="941b2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="941b2-146">DateTimeOffset</span></span>|<span data-ttu-id="941b2-147">第一个用户加入呼叫的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="941b2-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="941b2-148">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="941b2-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="941b2-149">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="941b2-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="941b2-150">type</span><span class="sxs-lookup"><span data-stu-id="941b2-150">type</span></span>|<span data-ttu-id="941b2-151">microsoft.graph.callRecords.callType</span><span class="sxs-lookup"><span data-stu-id="941b2-151">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="941b2-152">指示呼叫的类型。</span><span class="sxs-lookup"><span data-stu-id="941b2-152">Indicates the type of the call.</span></span> <span data-ttu-id="941b2-153">可取值为：`unknown`、`groupCall`、`peerToPeer`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="941b2-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="941b2-154">version</span><span class="sxs-lookup"><span data-stu-id="941b2-154">version</span></span>|<span data-ttu-id="941b2-155">Int64</span><span class="sxs-lookup"><span data-stu-id="941b2-155">Int64</span></span>|<span data-ttu-id="941b2-156">呼叫记录的单色增加版本。</span><span class="sxs-lookup"><span data-stu-id="941b2-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="941b2-157">与较低版本相比，具有相同 ID 的更高版本呼叫记录包含其他数据。</span><span class="sxs-lookup"><span data-stu-id="941b2-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="941b2-158">关系</span><span class="sxs-lookup"><span data-stu-id="941b2-158">Relationships</span></span>

| <span data-ttu-id="941b2-159">关系</span><span class="sxs-lookup"><span data-stu-id="941b2-159">Relationship</span></span> | <span data-ttu-id="941b2-160">类型</span><span class="sxs-lookup"><span data-stu-id="941b2-160">Type</span></span>        | <span data-ttu-id="941b2-161">说明</span><span class="sxs-lookup"><span data-stu-id="941b2-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="941b2-162">sessions</span><span class="sxs-lookup"><span data-stu-id="941b2-162">sessions</span></span>|<span data-ttu-id="941b2-163">[microsoft.graph.callRecords.session](callrecords-session.md) 集合</span><span class="sxs-lookup"><span data-stu-id="941b2-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="941b2-164">呼叫中涉及的会话列表。</span><span class="sxs-lookup"><span data-stu-id="941b2-164">List of sessions involved in the call.</span></span> <span data-ttu-id="941b2-165">对等呼叫通常只有一个会话，而组呼叫通常每个参与者至少具有一个会话。</span><span class="sxs-lookup"><span data-stu-id="941b2-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="941b2-166">只读。</span><span class="sxs-lookup"><span data-stu-id="941b2-166">Read-only.</span></span> <span data-ttu-id="941b2-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="941b2-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="941b2-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="941b2-168">JSON representation</span></span>

<span data-ttu-id="941b2-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="941b2-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
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
