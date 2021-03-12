---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户转移的请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 508f8c79606ef6e9e0d3778899cb04789b9defde
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720800"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="2bccc-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bccc-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="2bccc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bccc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bccc-105">表示向团队中的其他用户转移的请求。</span><span class="sxs-lookup"><span data-stu-id="2bccc-105">Represents a request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="2bccc-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2bccc-106">Methods</span></span>

| <span data-ttu-id="2bccc-107">方法</span><span class="sxs-lookup"><span data-stu-id="2bccc-107">Method</span></span>       | <span data-ttu-id="2bccc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2bccc-108">Return Type</span></span> | <span data-ttu-id="2bccc-109">Description</span><span class="sxs-lookup"><span data-stu-id="2bccc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2bccc-110">List</span><span class="sxs-lookup"><span data-stu-id="2bccc-110">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="2bccc-111">[offerShiftRequest 集合](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2bccc-111">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="2bccc-112">读取团队中 **所有 offerShiftRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bccc-112">Read the properties and relationships of all **offerShiftRequest** objects in a team.</span></span> |
| [<span data-ttu-id="2bccc-113">创建</span><span class="sxs-lookup"><span data-stu-id="2bccc-113">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="2bccc-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="2bccc-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="2bccc-115">创建 **offerShiftRequest 对象** 的实例。</span><span class="sxs-lookup"><span data-stu-id="2bccc-115">Create an instance of an **offerShiftRequest** object.</span></span> |
| [<span data-ttu-id="2bccc-116">获取</span><span class="sxs-lookup"><span data-stu-id="2bccc-116">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="2bccc-117">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="2bccc-117">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="2bccc-118">读取 **offerShiftRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bccc-118">Read the properties and relationships of an **offerShiftRequest** object.</span></span> |
|[<span data-ttu-id="2bccc-119">批准</span><span class="sxs-lookup"><span data-stu-id="2bccc-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="2bccc-120">无</span><span class="sxs-lookup"><span data-stu-id="2bccc-120">None</span></span>|<span data-ttu-id="2bccc-121">批准 **offerShiftRequest**。</span><span class="sxs-lookup"><span data-stu-id="2bccc-121">Approve an **offerShiftRequest**.</span></span> |
|[<span data-ttu-id="2bccc-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="2bccc-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="2bccc-123">无</span><span class="sxs-lookup"><span data-stu-id="2bccc-123">None</span></span>|<span data-ttu-id="2bccc-124">拒绝 **offerShiftRequest**。</span><span class="sxs-lookup"><span data-stu-id="2bccc-124">Decline an **offerShiftRequest**.</span></span> |

## <a name="properties"></a><span data-ttu-id="2bccc-125">属性</span><span class="sxs-lookup"><span data-stu-id="2bccc-125">Properties</span></span>

| <span data-ttu-id="2bccc-126">属性</span><span class="sxs-lookup"><span data-stu-id="2bccc-126">Property</span></span>     | <span data-ttu-id="2bccc-127">类型</span><span class="sxs-lookup"><span data-stu-id="2bccc-127">Type</span></span>        | <span data-ttu-id="2bccc-128">说明</span><span class="sxs-lookup"><span data-stu-id="2bccc-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bccc-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="2bccc-129">recipientActionDateTime</span></span>|<span data-ttu-id="2bccc-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bccc-130">DateTimeOffset</span></span>|<span data-ttu-id="2bccc-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2bccc-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2bccc-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2bccc-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2bccc-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="2bccc-133">recipientActionMessage</span></span>|<span data-ttu-id="2bccc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2bccc-134">String</span></span>| <span data-ttu-id="2bccc-135">产品/服务班次请求的收件人发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="2bccc-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="2bccc-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="2bccc-136">recipientUserId</span></span>|<span data-ttu-id="2bccc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2bccc-137">String</span></span>| <span data-ttu-id="2bccc-138">产品/服务班次请求的收件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2bccc-138">User ID of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="2bccc-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="2bccc-139">senderShiftId</span></span>|<span data-ttu-id="2bccc-140">字符串</span><span class="sxs-lookup"><span data-stu-id="2bccc-140">String</span></span>| <span data-ttu-id="2bccc-141">产品/服务班次请求发件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2bccc-141">User ID of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bccc-142">关系</span><span class="sxs-lookup"><span data-stu-id="2bccc-142">Relationships</span></span>

<span data-ttu-id="2bccc-143">无。</span><span class="sxs-lookup"><span data-stu-id="2bccc-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bccc-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bccc-144">JSON representation</span></span>

<span data-ttu-id="2bccc-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bccc-145">The following is a JSON representation of the resource.</span></span>

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

