---
title: changeNotification 资源类型
description: 表示发送给订阅者的更改通知。
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1bb5f8d5177e294a969fb48d335bd4a3061f1bb1
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681758"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="c5396-103">changeNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5396-103">changeNotification resource type</span></span>

<span data-ttu-id="c5396-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5396-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5396-105">表示发送给订阅者的通知。</span><span class="sxs-lookup"><span data-stu-id="c5396-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="c5396-106">有关详细信息，请参阅[使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="c5396-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c5396-107">Methods</span><span class="sxs-lookup"><span data-stu-id="c5396-107">Methods</span></span>

<span data-ttu-id="c5396-108">无。</span><span class="sxs-lookup"><span data-stu-id="c5396-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="c5396-109">属性</span><span class="sxs-lookup"><span data-stu-id="c5396-109">Properties</span></span>

| <span data-ttu-id="c5396-110">属性</span><span class="sxs-lookup"><span data-stu-id="c5396-110">Property</span></span> | <span data-ttu-id="c5396-111">类型</span><span class="sxs-lookup"><span data-stu-id="c5396-111">Type</span></span> | <span data-ttu-id="c5396-112">说明</span><span class="sxs-lookup"><span data-stu-id="c5396-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c5396-113">changeType</span><span class="sxs-lookup"><span data-stu-id="c5396-113">changeType</span></span> | <span data-ttu-id="c5396-114">string</span><span class="sxs-lookup"><span data-stu-id="c5396-114">string</span></span> | <span data-ttu-id="c5396-115">指示将引发更改通知的更改的类型。</span><span class="sxs-lookup"><span data-stu-id="c5396-115">Indicates the type of change that will raised the change notification.</span></span> <span data-ttu-id="c5396-116">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="c5396-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="c5396-117">必填。</span><span class="sxs-lookup"><span data-stu-id="c5396-117">Required.</span></span> |
| <span data-ttu-id="c5396-118">clientState</span><span class="sxs-lookup"><span data-stu-id="c5396-118">clientState</span></span> | <span data-ttu-id="c5396-119">string</span><span class="sxs-lookup"><span data-stu-id="c5396-119">string</span></span> | <span data-ttu-id="c5396-120">在订阅请求中指定的**clientState**属性的值（如果有）。</span><span class="sxs-lookup"><span data-stu-id="c5396-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="c5396-121">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="c5396-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="c5396-122">客户端可以通过将随订阅发送的**clientState**属性的值与每个更改通知接收的**clientState**属性的值进行比较，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="c5396-122">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="c5396-123">可选。</span><span class="sxs-lookup"><span data-stu-id="c5396-123">Optional.</span></span> |
| <span data-ttu-id="c5396-124">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="c5396-124">encryptedContent</span></span> | [<span data-ttu-id="c5396-125">changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="c5396-125">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="c5396-126">预览随更改通知附加的加密内容。</span><span class="sxs-lookup"><span data-stu-id="c5396-126">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="c5396-127">仅当**encryptionCertificate**和**includeResourceData**在订阅请求期间定义并且资源支持它时才提供。</span><span class="sxs-lookup"><span data-stu-id="c5396-127">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="c5396-128">可选</span><span class="sxs-lookup"><span data-stu-id="c5396-128">Optional</span></span> |
| <span data-ttu-id="c5396-129">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="c5396-129">lifecycleEvent</span></span> | <span data-ttu-id="c5396-130">string</span><span class="sxs-lookup"><span data-stu-id="c5396-130">string</span></span> | <span data-ttu-id="c5396-131">如果当前通知是生命周期通知，则为生命周期通知的类型。</span><span class="sxs-lookup"><span data-stu-id="c5396-131">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="c5396-132">可选。</span><span class="sxs-lookup"><span data-stu-id="c5396-132">Optional.</span></span> <span data-ttu-id="c5396-133">支持的值为 `missed` 、 `removed` 、 `reauthorizationRequired` 。</span><span class="sxs-lookup"><span data-stu-id="c5396-133">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="c5396-134">id</span><span class="sxs-lookup"><span data-stu-id="c5396-134">id</span></span> | <span data-ttu-id="c5396-135">字符串</span><span class="sxs-lookup"><span data-stu-id="c5396-135">string</span></span> | <span data-ttu-id="c5396-136">通知的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c5396-136">Unique ID for the notification.</span></span> <span data-ttu-id="c5396-137">可选。</span><span class="sxs-lookup"><span data-stu-id="c5396-137">Optional.</span></span> |
| <span data-ttu-id="c5396-138">resource</span><span class="sxs-lookup"><span data-stu-id="c5396-138">resource</span></span> | <span data-ttu-id="c5396-139">string</span><span class="sxs-lookup"><span data-stu-id="c5396-139">string</span></span> | <span data-ttu-id="c5396-140">发出更改通知的资源的 URI （相对于） `https://graph.microsoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="c5396-140">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="c5396-141">必填。</span><span class="sxs-lookup"><span data-stu-id="c5396-141">Required.</span></span> |
| <span data-ttu-id="c5396-142">resourceData</span><span class="sxs-lookup"><span data-stu-id="c5396-142">resourceData</span></span> | [<span data-ttu-id="c5396-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="c5396-143">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="c5396-144">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="c5396-144">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="c5396-145">必填。</span><span class="sxs-lookup"><span data-stu-id="c5396-145">Required.</span></span> |
| <span data-ttu-id="c5396-146">sequenceNumber</span><span class="sxs-lookup"><span data-stu-id="c5396-146">sequenceNumber</span></span> | <span data-ttu-id="c5396-147">int</span><span class="sxs-lookup"><span data-stu-id="c5396-147">int</span></span> | <span data-ttu-id="c5396-148">通知的序列号，帮助客户端应用程序确定通知是否按顺序排列或者是否缺少通知。</span><span class="sxs-lookup"><span data-stu-id="c5396-148">A number in sequence for a notification, to help the client app identify if notifications are in sequence or if a notification is missing.</span></span> <span data-ttu-id="c5396-149">可选。</span><span class="sxs-lookup"><span data-stu-id="c5396-149">Optional.</span></span> |
| <span data-ttu-id="c5396-150">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c5396-150">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="c5396-151">dateTime</span><span class="sxs-lookup"><span data-stu-id="c5396-151">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="c5396-152">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="c5396-152">The expiration time for the subscription.</span></span> <span data-ttu-id="c5396-153">必填。</span><span class="sxs-lookup"><span data-stu-id="c5396-153">Required.</span></span> |
| <span data-ttu-id="c5396-154">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="c5396-154">subscriptionId</span></span> | <span data-ttu-id="c5396-155">string</span><span class="sxs-lookup"><span data-stu-id="c5396-155">string</span></span> | <span data-ttu-id="c5396-156">生成通知的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c5396-156">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="c5396-157">tenantId</span><span class="sxs-lookup"><span data-stu-id="c5396-157">tenantId</span></span> | <span data-ttu-id="c5396-158">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="c5396-158">guid</span></span> | <span data-ttu-id="c5396-159">从其发出更改通知的租户的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="c5396-159">The unique identified of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c5396-160">关系</span><span class="sxs-lookup"><span data-stu-id="c5396-160">Relationships</span></span>

<span data-ttu-id="c5396-161">无。</span><span class="sxs-lookup"><span data-stu-id="c5396-161">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5396-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5396-162">JSON representation</span></span>

<span data-ttu-id="c5396-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5396-163">The following is a JSON representation of the resource.</span></span>

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
