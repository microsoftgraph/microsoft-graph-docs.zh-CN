---
title: changeNotification 资源类型
description: 表示发送给订阅者的更改通知。
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: d45c3973e5b044daf3121a740a60b29e3a181348
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45004769"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="19f30-103">changeNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="19f30-103">changeNotification resource type</span></span>

<span data-ttu-id="19f30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19f30-105">表示发送给订阅者的通知。</span><span class="sxs-lookup"><span data-stu-id="19f30-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="19f30-106">有关详细信息，请参阅[使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="19f30-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="19f30-107">方法</span><span class="sxs-lookup"><span data-stu-id="19f30-107">Methods</span></span>

<span data-ttu-id="19f30-108">无。</span><span class="sxs-lookup"><span data-stu-id="19f30-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="19f30-109">属性</span><span class="sxs-lookup"><span data-stu-id="19f30-109">Properties</span></span>

| <span data-ttu-id="19f30-110">属性</span><span class="sxs-lookup"><span data-stu-id="19f30-110">Property</span></span> | <span data-ttu-id="19f30-111">类型</span><span class="sxs-lookup"><span data-stu-id="19f30-111">Type</span></span> | <span data-ttu-id="19f30-112">说明</span><span class="sxs-lookup"><span data-stu-id="19f30-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="19f30-113">changeType</span><span class="sxs-lookup"><span data-stu-id="19f30-113">changeType</span></span> | <span data-ttu-id="19f30-114">string</span><span class="sxs-lookup"><span data-stu-id="19f30-114">string</span></span> | <span data-ttu-id="19f30-115">指示将引发更改通知的更改的类型。</span><span class="sxs-lookup"><span data-stu-id="19f30-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="19f30-116">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="19f30-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="19f30-117">必需。</span><span class="sxs-lookup"><span data-stu-id="19f30-117">Required.</span></span> |
| <span data-ttu-id="19f30-118">clientState</span><span class="sxs-lookup"><span data-stu-id="19f30-118">clientState</span></span> | <span data-ttu-id="19f30-119">string</span><span class="sxs-lookup"><span data-stu-id="19f30-119">string</span></span> | <span data-ttu-id="19f30-120">订阅请求中发送的**clientState**属性的值（如果有）。</span><span class="sxs-lookup"><span data-stu-id="19f30-120">Value of the **clientState** property sent in the subscription request (if any).</span></span> <span data-ttu-id="19f30-121">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="19f30-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="19f30-122">客户端可以通过比较**clientState**属性的值，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="19f30-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="19f30-123">与订阅一起发送的**clientState**属性的值将与每个更改通知收到的**clientState**属性的值进行比较。</span><span class="sxs-lookup"><span data-stu-id="19f30-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="19f30-124">可选。</span><span class="sxs-lookup"><span data-stu-id="19f30-124">Optional.</span></span> |
| <span data-ttu-id="19f30-125">id</span><span class="sxs-lookup"><span data-stu-id="19f30-125">id</span></span> | <span data-ttu-id="19f30-126">字符串</span><span class="sxs-lookup"><span data-stu-id="19f30-126">string</span></span> | <span data-ttu-id="19f30-127">通知的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="19f30-127">Unique ID for the notification.</span></span> <span data-ttu-id="19f30-128">可选。</span><span class="sxs-lookup"><span data-stu-id="19f30-128">Optional.</span></span> |
| <span data-ttu-id="19f30-129">resource</span><span class="sxs-lookup"><span data-stu-id="19f30-129">resource</span></span> | <span data-ttu-id="19f30-130">string</span><span class="sxs-lookup"><span data-stu-id="19f30-130">string</span></span> | <span data-ttu-id="19f30-131">发出更改通知的资源的 URI （相对于） `https://graph.microsoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="19f30-131">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="19f30-132">必需。</span><span class="sxs-lookup"><span data-stu-id="19f30-132">Required.</span></span> |
| <span data-ttu-id="19f30-133">resourceData</span><span class="sxs-lookup"><span data-stu-id="19f30-133">resourceData</span></span> | [<span data-ttu-id="19f30-134">resourceData</span><span class="sxs-lookup"><span data-stu-id="19f30-134">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="19f30-135">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="19f30-135">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="19f30-136">必需。</span><span class="sxs-lookup"><span data-stu-id="19f30-136">Required.</span></span> |
| <span data-ttu-id="19f30-137">sequenceNumber</span><span class="sxs-lookup"><span data-stu-id="19f30-137">sequenceNumber</span></span> | <span data-ttu-id="19f30-138">int</span><span class="sxs-lookup"><span data-stu-id="19f30-138">int</span></span> | <span data-ttu-id="19f30-139">通知的序列号，帮助客户端应用程序确定通知是否按顺序排列或者是否缺少通知。</span><span class="sxs-lookup"><span data-stu-id="19f30-139">A number in sequence for a notification, to help the client app identify if notifications are in sequence or if a notification is missing.</span></span> <span data-ttu-id="19f30-140">可选。</span><span class="sxs-lookup"><span data-stu-id="19f30-140">Optional.</span></span> |
| <span data-ttu-id="19f30-141">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="19f30-141">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="19f30-142">dateTime</span><span class="sxs-lookup"><span data-stu-id="19f30-142">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="19f30-143">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="19f30-143">The expiration time for the subscription.</span></span> <span data-ttu-id="19f30-144">必需。</span><span class="sxs-lookup"><span data-stu-id="19f30-144">Required.</span></span> |
| <span data-ttu-id="19f30-145">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="19f30-145">subscriptionId</span></span> | <span data-ttu-id="19f30-146">string</span><span class="sxs-lookup"><span data-stu-id="19f30-146">string</span></span> | <span data-ttu-id="19f30-147">生成通知的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="19f30-147">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="19f30-148">tenantId</span><span class="sxs-lookup"><span data-stu-id="19f30-148">tenantId</span></span> | <span data-ttu-id="19f30-149">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="19f30-149">guid</span></span> | <span data-ttu-id="19f30-150">来自其发出更改通知的租户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="19f30-150">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="19f30-151">关系</span><span class="sxs-lookup"><span data-stu-id="19f30-151">Relationships</span></span>

<span data-ttu-id="19f30-152">无。</span><span class="sxs-lookup"><span data-stu-id="19f30-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19f30-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19f30-153">JSON representation</span></span>

<span data-ttu-id="19f30-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19f30-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotification"
}-->

```json
{
  "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
  "changeType": "created",
  "clientState": "client state provided when creating subscription",
  "id": "15ee1d1f-af7b-42d9-885b-9d00db065dd9",
  "sequenceNumber": 20,
  "tenantId": "2c937fad-a8a7-496c-b0e4-bf77dcc7eb2a",
  "subscriptionExpirationDateTime": "2020-04-12T23:20:50.52Z",
  "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
  "resourceData": {
    "id": "1565293727947",
    "@odata.type": "#Microsoft.Graph.ChatMessage",
    "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
  }
}
```

<!-- uuid: 15ee1d1f-af7b-42d9-885b-9d00db065dd9
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
