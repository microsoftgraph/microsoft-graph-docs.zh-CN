---
title: offerShiftRequest 资源类型
description: 表示一个向团队中的其他用户提供班次的请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 57db39a398501a8b19b4978a17c1f60e26606dd3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025219"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="bede9-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="bede9-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="bede9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bede9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bede9-105">表示一个向团队中的其他用户提供班次的请求。</span><span class="sxs-lookup"><span data-stu-id="bede9-105">Represents a request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="bede9-106">方法</span><span class="sxs-lookup"><span data-stu-id="bede9-106">Methods</span></span>

| <span data-ttu-id="bede9-107">方法</span><span class="sxs-lookup"><span data-stu-id="bede9-107">Method</span></span>       | <span data-ttu-id="bede9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bede9-108">Return Type</span></span> | <span data-ttu-id="bede9-109">Description</span><span class="sxs-lookup"><span data-stu-id="bede9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bede9-110">List</span><span class="sxs-lookup"><span data-stu-id="bede9-110">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="bede9-111">[OfferShiftRequest](offershiftrequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="bede9-111">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="bede9-112">读取团队中所有 **offerShiftRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bede9-112">Read the properties and relationships of all **offerShiftRequest** objects in a team.</span></span> |
| [<span data-ttu-id="bede9-113">创建</span><span class="sxs-lookup"><span data-stu-id="bede9-113">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="bede9-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="bede9-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="bede9-115">创建 **offerShiftRequest** 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="bede9-115">Create an instance of an **offerShiftRequest** object.</span></span> |
| [<span data-ttu-id="bede9-116">获取</span><span class="sxs-lookup"><span data-stu-id="bede9-116">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="bede9-117">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="bede9-117">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="bede9-118">读取 **offerShiftRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bede9-118">Read the properties and relationships of an **offerShiftRequest** object.</span></span> |
|[<span data-ttu-id="bede9-119">批准</span><span class="sxs-lookup"><span data-stu-id="bede9-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="bede9-120">无</span><span class="sxs-lookup"><span data-stu-id="bede9-120">None</span></span>|<span data-ttu-id="bede9-121">批准 **offerShiftRequest**。</span><span class="sxs-lookup"><span data-stu-id="bede9-121">Approve an **offerShiftRequest**.</span></span> |
|[<span data-ttu-id="bede9-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="bede9-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="bede9-123">无</span><span class="sxs-lookup"><span data-stu-id="bede9-123">None</span></span>|<span data-ttu-id="bede9-124">拒绝 **offerShiftRequest**。</span><span class="sxs-lookup"><span data-stu-id="bede9-124">Decline an **offerShiftRequest**.</span></span> |

## <a name="properties"></a><span data-ttu-id="bede9-125">属性</span><span class="sxs-lookup"><span data-stu-id="bede9-125">Properties</span></span>

| <span data-ttu-id="bede9-126">属性</span><span class="sxs-lookup"><span data-stu-id="bede9-126">Property</span></span>     | <span data-ttu-id="bede9-127">类型</span><span class="sxs-lookup"><span data-stu-id="bede9-127">Type</span></span>        | <span data-ttu-id="bede9-128">说明</span><span class="sxs-lookup"><span data-stu-id="bede9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bede9-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="bede9-129">recipientActionDateTime</span></span>|<span data-ttu-id="bede9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bede9-130">DateTimeOffset</span></span>|<span data-ttu-id="bede9-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bede9-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bede9-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="bede9-133">recipientActionMessage</span></span>|<span data-ttu-id="bede9-134">String</span><span class="sxs-lookup"><span data-stu-id="bede9-134">String</span></span>| <span data-ttu-id="bede9-135">由服务移动请求的收件人发送的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="bede9-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="bede9-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="bede9-136">recipientUserId</span></span>|<span data-ttu-id="bede9-137">String</span><span class="sxs-lookup"><span data-stu-id="bede9-137">String</span></span>| <span data-ttu-id="bede9-138">提供班次请求的收件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="bede9-138">User ID of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="bede9-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="bede9-139">senderShiftId</span></span>|<span data-ttu-id="bede9-140">String</span><span class="sxs-lookup"><span data-stu-id="bede9-140">String</span></span>| <span data-ttu-id="bede9-141">提供班次请求的发件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="bede9-141">User ID of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bede9-142">关系</span><span class="sxs-lookup"><span data-stu-id="bede9-142">Relationships</span></span>

<span data-ttu-id="bede9-143">无。</span><span class="sxs-lookup"><span data-stu-id="bede9-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bede9-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bede9-144">JSON representation</span></span>

<span data-ttu-id="bede9-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bede9-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": ""
}-->

```json
{
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

