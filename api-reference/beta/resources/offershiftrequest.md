---
title: offerShiftRequest 资源类型
description: 表示要向团队中的其他用户提供班次的班次请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d1b26d7801a3eb4570104ff68b9037fd9c553a68
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156707"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="05614-103">offerShiftRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="05614-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="05614-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05614-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05614-105">表示要向团队中的其他用户提供班次的班次请求类型。</span><span class="sxs-lookup"><span data-stu-id="05614-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="05614-106">方法</span><span class="sxs-lookup"><span data-stu-id="05614-106">Methods</span></span>

| <span data-ttu-id="05614-107">方法</span><span class="sxs-lookup"><span data-stu-id="05614-107">Method</span></span>       | <span data-ttu-id="05614-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="05614-108">Return Type</span></span> | <span data-ttu-id="05614-109">说明</span><span class="sxs-lookup"><span data-stu-id="05614-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="05614-110">创建</span><span class="sxs-lookup"><span data-stu-id="05614-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="05614-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="05614-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="05614-112">创建 offerShiftRequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="05614-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="05614-113">Get</span><span class="sxs-lookup"><span data-stu-id="05614-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="05614-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="05614-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="05614-115">读取 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05614-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="05614-116">列表</span><span class="sxs-lookup"><span data-stu-id="05614-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="05614-117">[offerShiftRequest 集合](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="05614-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="05614-118">读取团队中所有 offerShiftRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05614-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="05614-119">批准</span><span class="sxs-lookup"><span data-stu-id="05614-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="05614-120">无</span><span class="sxs-lookup"><span data-stu-id="05614-120">None</span></span>|<span data-ttu-id="05614-121">批准 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="05614-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="05614-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="05614-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="05614-123">无</span><span class="sxs-lookup"><span data-stu-id="05614-123">None</span></span>|<span data-ttu-id="05614-124">拒绝 offerShiftRequest。</span><span class="sxs-lookup"><span data-stu-id="05614-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="05614-125">属性</span><span class="sxs-lookup"><span data-stu-id="05614-125">Properties</span></span>

| <span data-ttu-id="05614-126">属性</span><span class="sxs-lookup"><span data-stu-id="05614-126">Property</span></span>     | <span data-ttu-id="05614-127">类型</span><span class="sxs-lookup"><span data-stu-id="05614-127">Type</span></span>        | <span data-ttu-id="05614-128">说明</span><span class="sxs-lookup"><span data-stu-id="05614-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="05614-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="05614-129">recipientActionDateTime</span></span>|<span data-ttu-id="05614-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05614-130">DateTimeOffset</span></span>|<span data-ttu-id="05614-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="05614-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="05614-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="05614-133">recipientActionMessage</span></span>|<span data-ttu-id="05614-134">String</span><span class="sxs-lookup"><span data-stu-id="05614-134">String</span></span>| <span data-ttu-id="05614-135">产品/服务班次请求的收件人发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="05614-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="05614-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="05614-136">recipientUserId</span></span>|<span data-ttu-id="05614-137">String</span><span class="sxs-lookup"><span data-stu-id="05614-137">String</span></span>| <span data-ttu-id="05614-138">产品/服务班次请求的收件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="05614-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="05614-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="05614-139">senderShiftId</span></span>|<span data-ttu-id="05614-140">String</span><span class="sxs-lookup"><span data-stu-id="05614-140">String</span></span>| <span data-ttu-id="05614-141">产品/服务班次请求发件人的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="05614-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05614-142">关系</span><span class="sxs-lookup"><span data-stu-id="05614-142">Relationships</span></span>

<span data-ttu-id="05614-143">无</span><span class="sxs-lookup"><span data-stu-id="05614-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05614-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05614-144">JSON representation</span></span>

<span data-ttu-id="05614-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05614-145">The following is a JSON representation of the resource.</span></span>

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


