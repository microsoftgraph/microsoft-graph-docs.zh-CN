---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户提供班次的轮班请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f80e8578422aa00d6af1d2df22a0dfb7472c8c8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721479"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="549b1-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="549b1-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="549b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="549b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="549b1-105">表示向团队中的其他用户提供班次的轮班请求类型。</span><span class="sxs-lookup"><span data-stu-id="549b1-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="549b1-106">方法</span><span class="sxs-lookup"><span data-stu-id="549b1-106">Methods</span></span>

| <span data-ttu-id="549b1-107">方法</span><span class="sxs-lookup"><span data-stu-id="549b1-107">Method</span></span>       | <span data-ttu-id="549b1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="549b1-108">Return Type</span></span> | <span data-ttu-id="549b1-109">说明</span><span class="sxs-lookup"><span data-stu-id="549b1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="549b1-110">Create</span><span class="sxs-lookup"><span data-stu-id="549b1-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="549b1-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="549b1-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="549b1-112">创建 offerShiftRequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="549b1-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="549b1-113">获取</span><span class="sxs-lookup"><span data-stu-id="549b1-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="549b1-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="549b1-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="549b1-115">读取 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="549b1-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="549b1-116">List</span><span class="sxs-lookup"><span data-stu-id="549b1-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="549b1-117">[offerShiftRequest 集合](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="549b1-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="549b1-118">读取团队中所有 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="549b1-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="549b1-119">批准</span><span class="sxs-lookup"><span data-stu-id="549b1-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="549b1-120">无</span><span class="sxs-lookup"><span data-stu-id="549b1-120">None</span></span>|<span data-ttu-id="549b1-121">批准 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="549b1-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="549b1-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="549b1-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="549b1-123">无</span><span class="sxs-lookup"><span data-stu-id="549b1-123">None</span></span>|<span data-ttu-id="549b1-124">拒绝 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="549b1-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="549b1-125">属性</span><span class="sxs-lookup"><span data-stu-id="549b1-125">Properties</span></span>

| <span data-ttu-id="549b1-126">属性</span><span class="sxs-lookup"><span data-stu-id="549b1-126">Property</span></span>     | <span data-ttu-id="549b1-127">类型</span><span class="sxs-lookup"><span data-stu-id="549b1-127">Type</span></span>        | <span data-ttu-id="549b1-128">说明</span><span class="sxs-lookup"><span data-stu-id="549b1-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="549b1-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="549b1-129">recipientActionDateTime</span></span>|<span data-ttu-id="549b1-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="549b1-130">DateTimeOffset</span></span>|<span data-ttu-id="549b1-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="549b1-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="549b1-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="549b1-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="549b1-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="549b1-133">recipientActionMessage</span></span>|<span data-ttu-id="549b1-134">String</span><span class="sxs-lookup"><span data-stu-id="549b1-134">String</span></span>| <span data-ttu-id="549b1-135">产品/服务班次请求的收件人发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="549b1-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="549b1-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="549b1-136">recipientUserId</span></span>|<span data-ttu-id="549b1-137">String</span><span class="sxs-lookup"><span data-stu-id="549b1-137">String</span></span>| <span data-ttu-id="549b1-138">产品/服务班次请求的收件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="549b1-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="549b1-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="549b1-139">senderShiftId</span></span>|<span data-ttu-id="549b1-140">String</span><span class="sxs-lookup"><span data-stu-id="549b1-140">String</span></span>| <span data-ttu-id="549b1-141">产品/服务班次请求发件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="549b1-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="549b1-142">关系</span><span class="sxs-lookup"><span data-stu-id="549b1-142">Relationships</span></span>

<span data-ttu-id="549b1-143">无</span><span class="sxs-lookup"><span data-stu-id="549b1-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="549b1-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="549b1-144">JSON representation</span></span>

<span data-ttu-id="549b1-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="549b1-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest"
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


