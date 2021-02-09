---
title: callRecord 资源类型
description: 表示多个参与者之间的单个对等呼叫或组呼叫，有时称为联机会议。
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 04335e2d804a0d1f824cfc70982e3c138812f8ce
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159680"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="80580-103">callRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="80580-103">callRecord resource type</span></span>

<span data-ttu-id="80580-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="80580-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80580-105">表示多个参与者之间的单个对等呼叫或组呼叫，有时称为联机会议。</span><span class="sxs-lookup"><span data-stu-id="80580-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="80580-106">方法</span><span class="sxs-lookup"><span data-stu-id="80580-106">Methods</span></span>

| <span data-ttu-id="80580-107">方法</span><span class="sxs-lookup"><span data-stu-id="80580-107">Method</span></span>       | <span data-ttu-id="80580-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="80580-108">Return Type</span></span> | <span data-ttu-id="80580-109">说明</span><span class="sxs-lookup"><span data-stu-id="80580-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="80580-110">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="80580-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="80580-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="80580-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="80580-112">读取 **callRecord** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80580-112">Read the properties and relationships of a **callRecord** object.</span></span> |
| [<span data-ttu-id="80580-113">获取 PSTN 呼叫</span><span class="sxs-lookup"><span data-stu-id="80580-113">Get PSTN calls</span></span>](../api/callrecords-callrecord-getpstncalls.md) | [<span data-ttu-id="80580-114">microsoft.graph.callRecords.pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="80580-114">microsoft.graph.callRecords.pstnCallLogRow</span></span>](callrecords-pstncalllogrow.md)| <span data-ttu-id="80580-115">读取 **pstnCallLogRow 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="80580-115">Read the properties of a **pstnCallLogRow** object.</span></span> |
| [<span data-ttu-id="80580-116">获取直接路由呼叫</span><span class="sxs-lookup"><span data-stu-id="80580-116">Get direct routing calls</span></span>](../api/callrecords-callrecord-getdirectroutingcalls.md) | [<span data-ttu-id="80580-117">microsoft.graph.callRecords.directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="80580-117">microsoft.graph.callRecords.directRoutingLogRow</span></span>](callrecords-directroutinglogrow.md)| <span data-ttu-id="80580-118">读取 **directRoutingLogRow 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="80580-118">Read the properties of a **directRoutingLogRow** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80580-119">属性</span><span class="sxs-lookup"><span data-stu-id="80580-119">Properties</span></span>

| <span data-ttu-id="80580-120">属性</span><span class="sxs-lookup"><span data-stu-id="80580-120">Property</span></span>     | <span data-ttu-id="80580-121">类型</span><span class="sxs-lookup"><span data-stu-id="80580-121">Type</span></span>        | <span data-ttu-id="80580-122">说明</span><span class="sxs-lookup"><span data-stu-id="80580-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80580-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="80580-123">endDateTime</span></span>|<span data-ttu-id="80580-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80580-124">DateTimeOffset</span></span>|<span data-ttu-id="80580-125">最后一个用户离开呼叫的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80580-125">UTC time when the last user left the call.</span></span> <span data-ttu-id="80580-126">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80580-126">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80580-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="80580-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="80580-128">id</span><span class="sxs-lookup"><span data-stu-id="80580-128">id</span></span>|<span data-ttu-id="80580-129">String</span><span class="sxs-lookup"><span data-stu-id="80580-129">String</span></span>|<span data-ttu-id="80580-130">呼叫记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="80580-130">Unique identifier for the call record.</span></span> <span data-ttu-id="80580-131">只读。</span><span class="sxs-lookup"><span data-stu-id="80580-131">Read-only.</span></span>|
|<span data-ttu-id="80580-132">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="80580-132">joinWebUrl</span></span>|<span data-ttu-id="80580-133">String</span><span class="sxs-lookup"><span data-stu-id="80580-133">String</span></span>|<span data-ttu-id="80580-134">与呼叫关联的会议 URL。</span><span class="sxs-lookup"><span data-stu-id="80580-134">Meeting URL associated to the call.</span></span> <span data-ttu-id="80580-135">peerToPeer 呼叫记录类型可能不可用。</span><span class="sxs-lookup"><span data-stu-id="80580-135">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="80580-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80580-136">lastModifiedDateTime</span></span>|<span data-ttu-id="80580-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80580-137">DateTimeOffset</span></span>|<span data-ttu-id="80580-138">创建呼叫记录时 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80580-138">UTC time when the call record was created.</span></span> <span data-ttu-id="80580-139">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80580-139">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80580-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="80580-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="80580-141">modalities</span><span class="sxs-lookup"><span data-stu-id="80580-141">modalities</span></span>|<span data-ttu-id="80580-142">microsoft.graph.callRecords.modality 集合</span><span class="sxs-lookup"><span data-stu-id="80580-142">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="80580-143">调用中使用的所有形式的列表。</span><span class="sxs-lookup"><span data-stu-id="80580-143">List of all the modalities used in the call.</span></span> <span data-ttu-id="80580-144">可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="80580-144">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="80580-145">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="80580-145">organizer</span></span>|[<span data-ttu-id="80580-146">identitySet</span><span class="sxs-lookup"><span data-stu-id="80580-146">identitySet</span></span>](identityset.md)|<span data-ttu-id="80580-147">组织方的身份。</span><span class="sxs-lookup"><span data-stu-id="80580-147">The organizing party's identity.</span></span>|
|<span data-ttu-id="80580-148">participants</span><span class="sxs-lookup"><span data-stu-id="80580-148">participants</span></span>|<span data-ttu-id="80580-149">[identitySet](identityset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80580-149">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="80580-150">调用中涉及的不同标识的列表。</span><span class="sxs-lookup"><span data-stu-id="80580-150">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="80580-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="80580-151">startDateTime</span></span>|<span data-ttu-id="80580-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80580-152">DateTimeOffset</span></span>|<span data-ttu-id="80580-153">第一个用户加入呼叫的 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80580-153">UTC time when the first user joined the call.</span></span> <span data-ttu-id="80580-154">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80580-154">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80580-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="80580-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="80580-156">type</span><span class="sxs-lookup"><span data-stu-id="80580-156">type</span></span>|<span data-ttu-id="80580-157">microsoft.graph.callRecords.callType</span><span class="sxs-lookup"><span data-stu-id="80580-157">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="80580-158">指示呼叫的类型。</span><span class="sxs-lookup"><span data-stu-id="80580-158">Indicates the type of the call.</span></span> <span data-ttu-id="80580-159">可取值为：`unknown`、`groupCall`、`peerToPeer`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="80580-159">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="80580-160">version</span><span class="sxs-lookup"><span data-stu-id="80580-160">version</span></span>|<span data-ttu-id="80580-161">Int64</span><span class="sxs-lookup"><span data-stu-id="80580-161">Int64</span></span>|<span data-ttu-id="80580-162">呼叫记录的单色增加版本。</span><span class="sxs-lookup"><span data-stu-id="80580-162">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="80580-163">与较低版本相比，具有相同 ID 的更高版本呼叫记录包含其他数据。</span><span class="sxs-lookup"><span data-stu-id="80580-163">Higher version call records with the same ID includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80580-164">关系</span><span class="sxs-lookup"><span data-stu-id="80580-164">Relationships</span></span>

| <span data-ttu-id="80580-165">关系</span><span class="sxs-lookup"><span data-stu-id="80580-165">Relationship</span></span> | <span data-ttu-id="80580-166">类型</span><span class="sxs-lookup"><span data-stu-id="80580-166">Type</span></span>        | <span data-ttu-id="80580-167">说明</span><span class="sxs-lookup"><span data-stu-id="80580-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80580-168">sessions</span><span class="sxs-lookup"><span data-stu-id="80580-168">sessions</span></span>|<span data-ttu-id="80580-169">[microsoft.graph.callRecords.session](callrecords-session.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80580-169">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="80580-170">呼叫中涉及的会话列表。</span><span class="sxs-lookup"><span data-stu-id="80580-170">List of sessions involved in the call.</span></span> <span data-ttu-id="80580-171">对等呼叫通常只有一个会话，而组呼叫通常每个参与者至少具有一个会话。</span><span class="sxs-lookup"><span data-stu-id="80580-171">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="80580-172">只读。</span><span class="sxs-lookup"><span data-stu-id="80580-172">Read-only.</span></span> <span data-ttu-id="80580-173">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="80580-173">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80580-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80580-174">JSON representation</span></span>

<span data-ttu-id="80580-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80580-175">The following is a JSON representation of the resource.</span></span>

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


