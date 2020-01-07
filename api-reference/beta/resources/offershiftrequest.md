---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户提供班次的 shift 请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2b12dd9df816ad7fecbf6c520f0fff579087428
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952291"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="09ce4-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="09ce4-103">offerShiftRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ce4-104">表示向团队中的其他用户提供班次的 shift 请求的类型。</span><span class="sxs-lookup"><span data-stu-id="09ce4-104">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="09ce4-105">Methods</span><span class="sxs-lookup"><span data-stu-id="09ce4-105">Methods</span></span>

| <span data-ttu-id="09ce4-106">方法</span><span class="sxs-lookup"><span data-stu-id="09ce4-106">Method</span></span>       | <span data-ttu-id="09ce4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="09ce4-107">Return Type</span></span> | <span data-ttu-id="09ce4-108">说明</span><span class="sxs-lookup"><span data-stu-id="09ce4-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="09ce4-109">Create</span><span class="sxs-lookup"><span data-stu-id="09ce4-109">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="09ce4-110">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="09ce4-110">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="09ce4-111">创建 offerShiftRequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="09ce4-111">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="09ce4-112">Get</span><span class="sxs-lookup"><span data-stu-id="09ce4-112">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="09ce4-113">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="09ce4-113">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="09ce4-114">读取 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09ce4-114">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="09ce4-115">List</span><span class="sxs-lookup"><span data-stu-id="09ce4-115">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="09ce4-116">[OfferShiftRequest](offershiftrequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="09ce4-116">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="09ce4-117">读取团队中所有 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09ce4-117">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="09ce4-118">批准</span><span class="sxs-lookup"><span data-stu-id="09ce4-118">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="09ce4-119">无</span><span class="sxs-lookup"><span data-stu-id="09ce4-119">None</span></span>|<span data-ttu-id="09ce4-120">批准 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="09ce4-120">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="09ce4-121">拒绝</span><span class="sxs-lookup"><span data-stu-id="09ce4-121">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="09ce4-122">无</span><span class="sxs-lookup"><span data-stu-id="09ce4-122">None</span></span>|<span data-ttu-id="09ce4-123">拒绝 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="09ce4-123">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="09ce4-124">属性</span><span class="sxs-lookup"><span data-stu-id="09ce4-124">Properties</span></span>

| <span data-ttu-id="09ce4-125">属性</span><span class="sxs-lookup"><span data-stu-id="09ce4-125">Property</span></span>     | <span data-ttu-id="09ce4-126">类型</span><span class="sxs-lookup"><span data-stu-id="09ce4-126">Type</span></span>        | <span data-ttu-id="09ce4-127">Description</span><span class="sxs-lookup"><span data-stu-id="09ce4-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09ce4-128">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="09ce4-128">recipientActionDateTime</span></span>|<span data-ttu-id="09ce4-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09ce4-129">DateTimeOffset</span></span>|<span data-ttu-id="09ce4-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="09ce4-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="09ce4-132">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="09ce4-132">recipientActionMessage</span></span>|<span data-ttu-id="09ce4-133">String</span><span class="sxs-lookup"><span data-stu-id="09ce4-133">String</span></span>| <span data-ttu-id="09ce4-134">由服务移动请求的收件人发送的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="09ce4-134">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="09ce4-135">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="09ce4-135">recipientUserId</span></span>|<span data-ttu-id="09ce4-136">String</span><span class="sxs-lookup"><span data-stu-id="09ce4-136">String</span></span>| <span data-ttu-id="09ce4-137">提供班次请求的收件人的用户 id。</span><span class="sxs-lookup"><span data-stu-id="09ce4-137">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="09ce4-138">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="09ce4-138">senderShiftId</span></span>|<span data-ttu-id="09ce4-139">String</span><span class="sxs-lookup"><span data-stu-id="09ce4-139">String</span></span>| <span data-ttu-id="09ce4-140">提供班次请求的发件人的用户 id。</span><span class="sxs-lookup"><span data-stu-id="09ce4-140">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09ce4-141">关系</span><span class="sxs-lookup"><span data-stu-id="09ce4-141">Relationships</span></span>

<span data-ttu-id="09ce4-142">无</span><span class="sxs-lookup"><span data-stu-id="09ce4-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09ce4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09ce4-143">JSON representation</span></span>

<span data-ttu-id="09ce4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09ce4-144">The following is a JSON representation of the resource.</span></span>

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
