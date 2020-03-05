---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户提供班次的 shift 请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b0d56a3c9e3e8b098dbbe7f172a42631afbb33b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522517"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="a76ba-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="a76ba-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="a76ba-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a76ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a76ba-105">表示向团队中的其他用户提供班次的 shift 请求的类型。</span><span class="sxs-lookup"><span data-stu-id="a76ba-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="a76ba-106">方法</span><span class="sxs-lookup"><span data-stu-id="a76ba-106">Methods</span></span>

| <span data-ttu-id="a76ba-107">方法</span><span class="sxs-lookup"><span data-stu-id="a76ba-107">Method</span></span>       | <span data-ttu-id="a76ba-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a76ba-108">Return Type</span></span> | <span data-ttu-id="a76ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="a76ba-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a76ba-110">Create</span><span class="sxs-lookup"><span data-stu-id="a76ba-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="a76ba-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="a76ba-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="a76ba-112">创建 offerShiftRequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="a76ba-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="a76ba-113">获取</span><span class="sxs-lookup"><span data-stu-id="a76ba-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="a76ba-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="a76ba-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="a76ba-115">读取 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a76ba-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="a76ba-116">List</span><span class="sxs-lookup"><span data-stu-id="a76ba-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="a76ba-117">[OfferShiftRequest](offershiftrequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="a76ba-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="a76ba-118">读取团队中所有 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a76ba-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="a76ba-119">批准</span><span class="sxs-lookup"><span data-stu-id="a76ba-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="a76ba-120">无</span><span class="sxs-lookup"><span data-stu-id="a76ba-120">None</span></span>|<span data-ttu-id="a76ba-121">批准 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="a76ba-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="a76ba-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="a76ba-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="a76ba-123">无</span><span class="sxs-lookup"><span data-stu-id="a76ba-123">None</span></span>|<span data-ttu-id="a76ba-124">拒绝 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="a76ba-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="a76ba-125">属性</span><span class="sxs-lookup"><span data-stu-id="a76ba-125">Properties</span></span>

| <span data-ttu-id="a76ba-126">属性</span><span class="sxs-lookup"><span data-stu-id="a76ba-126">Property</span></span>     | <span data-ttu-id="a76ba-127">类型</span><span class="sxs-lookup"><span data-stu-id="a76ba-127">Type</span></span>        | <span data-ttu-id="a76ba-128">说明</span><span class="sxs-lookup"><span data-stu-id="a76ba-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a76ba-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a76ba-129">recipientActionDateTime</span></span>|<span data-ttu-id="a76ba-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a76ba-130">DateTimeOffset</span></span>|<span data-ttu-id="a76ba-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a76ba-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a76ba-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="a76ba-133">recipientActionMessage</span></span>|<span data-ttu-id="a76ba-134">String</span><span class="sxs-lookup"><span data-stu-id="a76ba-134">String</span></span>| <span data-ttu-id="a76ba-135">由服务移动请求的收件人发送的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="a76ba-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="a76ba-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="a76ba-136">recipientUserId</span></span>|<span data-ttu-id="a76ba-137">String</span><span class="sxs-lookup"><span data-stu-id="a76ba-137">String</span></span>| <span data-ttu-id="a76ba-138">提供班次请求的收件人的用户 id。</span><span class="sxs-lookup"><span data-stu-id="a76ba-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="a76ba-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="a76ba-139">senderShiftId</span></span>|<span data-ttu-id="a76ba-140">String</span><span class="sxs-lookup"><span data-stu-id="a76ba-140">String</span></span>| <span data-ttu-id="a76ba-141">提供班次请求的发件人的用户 id。</span><span class="sxs-lookup"><span data-stu-id="a76ba-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a76ba-142">关系</span><span class="sxs-lookup"><span data-stu-id="a76ba-142">Relationships</span></span>

<span data-ttu-id="a76ba-143">无</span><span class="sxs-lookup"><span data-stu-id="a76ba-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a76ba-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a76ba-144">JSON representation</span></span>

<span data-ttu-id="a76ba-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a76ba-145">The following is a JSON representation of the resource.</span></span>

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
