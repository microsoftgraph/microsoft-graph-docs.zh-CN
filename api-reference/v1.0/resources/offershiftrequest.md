---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户提供转换的请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d17ca029d29b2b8f27a923adf4ef019ac002f404
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158721"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="73781-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="73781-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="73781-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73781-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73781-105">表示向团队中的其他用户提供转换的请求。</span><span class="sxs-lookup"><span data-stu-id="73781-105">Represents a request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="73781-106">方法</span><span class="sxs-lookup"><span data-stu-id="73781-106">Methods</span></span>

| <span data-ttu-id="73781-107">方法</span><span class="sxs-lookup"><span data-stu-id="73781-107">Method</span></span>       | <span data-ttu-id="73781-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="73781-108">Return Type</span></span> | <span data-ttu-id="73781-109">Description</span><span class="sxs-lookup"><span data-stu-id="73781-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="73781-110">List</span><span class="sxs-lookup"><span data-stu-id="73781-110">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="73781-111">[offerShiftRequest 集合](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="73781-111">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="73781-112">读取团队中 **所有 offerShiftRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73781-112">Read the properties and relationships of all **offerShiftRequest** objects in a team.</span></span> |
| [<span data-ttu-id="73781-113">创建</span><span class="sxs-lookup"><span data-stu-id="73781-113">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="73781-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="73781-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="73781-115">创建 **offerShiftRequest 对象** 的实例。</span><span class="sxs-lookup"><span data-stu-id="73781-115">Create an instance of an **offerShiftRequest** object.</span></span> |
| [<span data-ttu-id="73781-116">Get</span><span class="sxs-lookup"><span data-stu-id="73781-116">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="73781-117">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="73781-117">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="73781-118">读取 **offerShiftRequest 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="73781-118">Read the properties and relationships of an **offerShiftRequest** object.</span></span> |
|[<span data-ttu-id="73781-119">批准</span><span class="sxs-lookup"><span data-stu-id="73781-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="73781-120">无</span><span class="sxs-lookup"><span data-stu-id="73781-120">None</span></span>|<span data-ttu-id="73781-121">批准 **offerShiftRequest**。</span><span class="sxs-lookup"><span data-stu-id="73781-121">Approve an **offerShiftRequest**.</span></span> |
|[<span data-ttu-id="73781-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="73781-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="73781-123">无</span><span class="sxs-lookup"><span data-stu-id="73781-123">None</span></span>|<span data-ttu-id="73781-124">拒绝 **offerShiftRequest**。</span><span class="sxs-lookup"><span data-stu-id="73781-124">Decline an **offerShiftRequest**.</span></span> |

## <a name="properties"></a><span data-ttu-id="73781-125">属性</span><span class="sxs-lookup"><span data-stu-id="73781-125">Properties</span></span>

| <span data-ttu-id="73781-126">属性</span><span class="sxs-lookup"><span data-stu-id="73781-126">Property</span></span>     | <span data-ttu-id="73781-127">类型</span><span class="sxs-lookup"><span data-stu-id="73781-127">Type</span></span>        | <span data-ttu-id="73781-128">说明</span><span class="sxs-lookup"><span data-stu-id="73781-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73781-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="73781-129">recipientActionDateTime</span></span>|<span data-ttu-id="73781-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73781-130">DateTimeOffset</span></span>|<span data-ttu-id="73781-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="73781-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="73781-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="73781-133">recipientActionMessage</span></span>|<span data-ttu-id="73781-134">String</span><span class="sxs-lookup"><span data-stu-id="73781-134">String</span></span>| <span data-ttu-id="73781-135">产品/服务班次请求的收件人发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="73781-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="73781-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="73781-136">recipientUserId</span></span>|<span data-ttu-id="73781-137">String</span><span class="sxs-lookup"><span data-stu-id="73781-137">String</span></span>| <span data-ttu-id="73781-138">产品/服务班次请求的收件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="73781-138">User ID of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="73781-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="73781-139">senderShiftId</span></span>|<span data-ttu-id="73781-140">String</span><span class="sxs-lookup"><span data-stu-id="73781-140">String</span></span>| <span data-ttu-id="73781-141">产品/服务班次请求发件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="73781-141">User ID of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73781-142">关系</span><span class="sxs-lookup"><span data-stu-id="73781-142">Relationships</span></span>

<span data-ttu-id="73781-143">无。</span><span class="sxs-lookup"><span data-stu-id="73781-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73781-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73781-144">JSON representation</span></span>

<span data-ttu-id="73781-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73781-145">The following is a JSON representation of the resource.</span></span>

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

