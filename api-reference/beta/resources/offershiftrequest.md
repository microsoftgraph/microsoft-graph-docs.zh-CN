---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户提供班次的 shift 请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c41461848fab45f3d291b175e6c584f98326fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021271"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="3102f-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="3102f-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="3102f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3102f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3102f-105">表示向团队中的其他用户提供班次的 shift 请求的类型。</span><span class="sxs-lookup"><span data-stu-id="3102f-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="3102f-106">方法</span><span class="sxs-lookup"><span data-stu-id="3102f-106">Methods</span></span>

| <span data-ttu-id="3102f-107">方法</span><span class="sxs-lookup"><span data-stu-id="3102f-107">Method</span></span>       | <span data-ttu-id="3102f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3102f-108">Return Type</span></span> | <span data-ttu-id="3102f-109">说明</span><span class="sxs-lookup"><span data-stu-id="3102f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3102f-110">创建</span><span class="sxs-lookup"><span data-stu-id="3102f-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="3102f-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="3102f-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="3102f-112">创建 offerShiftRequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="3102f-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="3102f-113">获取</span><span class="sxs-lookup"><span data-stu-id="3102f-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="3102f-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="3102f-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="3102f-115">读取 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3102f-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="3102f-116">List</span><span class="sxs-lookup"><span data-stu-id="3102f-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="3102f-117">[OfferShiftRequest](offershiftrequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="3102f-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="3102f-118">读取团队中所有 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3102f-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="3102f-119">批准</span><span class="sxs-lookup"><span data-stu-id="3102f-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="3102f-120">无</span><span class="sxs-lookup"><span data-stu-id="3102f-120">None</span></span>|<span data-ttu-id="3102f-121">批准 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="3102f-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="3102f-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="3102f-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="3102f-123">无</span><span class="sxs-lookup"><span data-stu-id="3102f-123">None</span></span>|<span data-ttu-id="3102f-124">拒绝 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="3102f-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="3102f-125">属性</span><span class="sxs-lookup"><span data-stu-id="3102f-125">Properties</span></span>

| <span data-ttu-id="3102f-126">属性</span><span class="sxs-lookup"><span data-stu-id="3102f-126">Property</span></span>     | <span data-ttu-id="3102f-127">类型</span><span class="sxs-lookup"><span data-stu-id="3102f-127">Type</span></span>        | <span data-ttu-id="3102f-128">说明</span><span class="sxs-lookup"><span data-stu-id="3102f-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3102f-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="3102f-129">recipientActionDateTime</span></span>|<span data-ttu-id="3102f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3102f-130">DateTimeOffset</span></span>|<span data-ttu-id="3102f-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3102f-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3102f-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="3102f-133">recipientActionMessage</span></span>|<span data-ttu-id="3102f-134">String</span><span class="sxs-lookup"><span data-stu-id="3102f-134">String</span></span>| <span data-ttu-id="3102f-135">由服务移动请求的收件人发送的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="3102f-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="3102f-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="3102f-136">recipientUserId</span></span>|<span data-ttu-id="3102f-137">String</span><span class="sxs-lookup"><span data-stu-id="3102f-137">String</span></span>| <span data-ttu-id="3102f-138">提供班次请求的收件人的用户 id。</span><span class="sxs-lookup"><span data-stu-id="3102f-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="3102f-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="3102f-139">senderShiftId</span></span>|<span data-ttu-id="3102f-140">String</span><span class="sxs-lookup"><span data-stu-id="3102f-140">String</span></span>| <span data-ttu-id="3102f-141">提供班次请求的发件人的用户 id。</span><span class="sxs-lookup"><span data-stu-id="3102f-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3102f-142">关系</span><span class="sxs-lookup"><span data-stu-id="3102f-142">Relationships</span></span>

<span data-ttu-id="3102f-143">无</span><span class="sxs-lookup"><span data-stu-id="3102f-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3102f-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3102f-144">JSON representation</span></span>

<span data-ttu-id="3102f-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3102f-145">The following is a JSON representation of the resource.</span></span>

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


