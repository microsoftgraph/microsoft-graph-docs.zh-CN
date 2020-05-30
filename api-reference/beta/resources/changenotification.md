---
title: changeNotification 资源类型
description: 表示发送给订阅者的更改通知。
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 117bd9c6ab25ca1db00233a15b8d984f6bb512a4
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/30/2020
ms.locfileid: "44430582"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="f6f94-103">changeNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6f94-103">changeNotification resource type</span></span>

<span data-ttu-id="f6f94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6f94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6f94-105">表示发送给订阅者的通知。</span><span class="sxs-lookup"><span data-stu-id="f6f94-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="f6f94-106">有关详细信息，请参阅[使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="f6f94-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f6f94-107">方法</span><span class="sxs-lookup"><span data-stu-id="f6f94-107">Methods</span></span>

<span data-ttu-id="f6f94-108">无。</span><span class="sxs-lookup"><span data-stu-id="f6f94-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="f6f94-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6f94-109">Properties</span></span>

| <span data-ttu-id="f6f94-110">属性</span><span class="sxs-lookup"><span data-stu-id="f6f94-110">Property</span></span> | <span data-ttu-id="f6f94-111">类型</span><span class="sxs-lookup"><span data-stu-id="f6f94-111">Type</span></span> | <span data-ttu-id="f6f94-112">说明</span><span class="sxs-lookup"><span data-stu-id="f6f94-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f6f94-113">changeType</span><span class="sxs-lookup"><span data-stu-id="f6f94-113">changeType</span></span> | <span data-ttu-id="f6f94-114">string</span><span class="sxs-lookup"><span data-stu-id="f6f94-114">string</span></span> | <span data-ttu-id="f6f94-115">指示将引发更改通知的更改的类型。</span><span class="sxs-lookup"><span data-stu-id="f6f94-115">Indicates the type of change that will raised the change notification.</span></span> <span data-ttu-id="f6f94-116">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="f6f94-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f6f94-117">必填。</span><span class="sxs-lookup"><span data-stu-id="f6f94-117">Required.</span></span> |
| <span data-ttu-id="f6f94-118">clientState</span><span class="sxs-lookup"><span data-stu-id="f6f94-118">clientState</span></span> | <span data-ttu-id="f6f94-119">string</span><span class="sxs-lookup"><span data-stu-id="f6f94-119">string</span></span> | <span data-ttu-id="f6f94-120">在订阅请求中指定的**clientState**属性的值（如果有）。</span><span class="sxs-lookup"><span data-stu-id="f6f94-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="f6f94-121">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="f6f94-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="f6f94-122">客户端可以通过将随订阅发送的**clientState**属性的值与每个更改通知接收的**clientState**属性的值进行比较，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="f6f94-122">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="f6f94-123">可选。</span><span class="sxs-lookup"><span data-stu-id="f6f94-123">Optional.</span></span> |
| <span data-ttu-id="f6f94-124">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="f6f94-124">encryptedContent</span></span> | [<span data-ttu-id="f6f94-125">changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="f6f94-125">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="f6f94-126">预览随更改通知附加的加密内容。</span><span class="sxs-lookup"><span data-stu-id="f6f94-126">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="f6f94-127">仅当**encryptionCertificate**和**includeResourceData**在订阅请求期间定义并且资源支持它时才提供。</span><span class="sxs-lookup"><span data-stu-id="f6f94-127">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="f6f94-128">可选</span><span class="sxs-lookup"><span data-stu-id="f6f94-128">Optional</span></span> |
| <span data-ttu-id="f6f94-129">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="f6f94-129">lifecycleEvent</span></span> | <span data-ttu-id="f6f94-130">string</span><span class="sxs-lookup"><span data-stu-id="f6f94-130">string</span></span> | <span data-ttu-id="f6f94-131">如果当前通知是生命周期通知，则为生命周期通知的类型。</span><span class="sxs-lookup"><span data-stu-id="f6f94-131">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="f6f94-132">可选。</span><span class="sxs-lookup"><span data-stu-id="f6f94-132">Optional.</span></span> <span data-ttu-id="f6f94-133">支持的值为 `missed` 、 `removed` 、 `reauthorizationRequired` 。</span><span class="sxs-lookup"><span data-stu-id="f6f94-133">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="f6f94-134">id</span><span class="sxs-lookup"><span data-stu-id="f6f94-134">id</span></span> | <span data-ttu-id="f6f94-135">字符串</span><span class="sxs-lookup"><span data-stu-id="f6f94-135">string</span></span> | <span data-ttu-id="f6f94-136">通知的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="f6f94-136">Unique ID for the notification.</span></span> <span data-ttu-id="f6f94-137">可选。</span><span class="sxs-lookup"><span data-stu-id="f6f94-137">Optional.</span></span> |
| <span data-ttu-id="f6f94-138">resource</span><span class="sxs-lookup"><span data-stu-id="f6f94-138">resource</span></span> | <span data-ttu-id="f6f94-139">string</span><span class="sxs-lookup"><span data-stu-id="f6f94-139">string</span></span> | <span data-ttu-id="f6f94-140">发出更改通知的资源的 URI （相对于） `https://graph.microsoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="f6f94-140">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="f6f94-141">必填。</span><span class="sxs-lookup"><span data-stu-id="f6f94-141">Required.</span></span> |
| <span data-ttu-id="f6f94-142">resourceData</span><span class="sxs-lookup"><span data-stu-id="f6f94-142">resourceData</span></span> | [<span data-ttu-id="f6f94-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="f6f94-143">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="f6f94-144">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="f6f94-144">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="f6f94-145">必填。</span><span class="sxs-lookup"><span data-stu-id="f6f94-145">Required.</span></span> |
| <span data-ttu-id="f6f94-146">sequenceNumber</span><span class="sxs-lookup"><span data-stu-id="f6f94-146">sequenceNumber</span></span> | <span data-ttu-id="f6f94-147">int</span><span class="sxs-lookup"><span data-stu-id="f6f94-147">int</span></span> | <span data-ttu-id="f6f94-148">可用于确保收到的通知按顺序进行。</span><span class="sxs-lookup"><span data-stu-id="f6f94-148">Can be used to make sure received notifications are in order.</span></span> <span data-ttu-id="f6f94-149">可选。</span><span class="sxs-lookup"><span data-stu-id="f6f94-149">Optional.</span></span> |
| <span data-ttu-id="f6f94-150">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6f94-150">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="f6f94-151">dateTime</span><span class="sxs-lookup"><span data-stu-id="f6f94-151">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="f6f94-152">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="f6f94-152">The expiration time for the subscription.</span></span> <span data-ttu-id="f6f94-153">必填。</span><span class="sxs-lookup"><span data-stu-id="f6f94-153">Required.</span></span> |
| <span data-ttu-id="f6f94-154">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="f6f94-154">subscriptionId</span></span> | <span data-ttu-id="f6f94-155">string</span><span class="sxs-lookup"><span data-stu-id="f6f94-155">string</span></span> | <span data-ttu-id="f6f94-156">生成通知的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f6f94-156">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="f6f94-157">tenantId</span><span class="sxs-lookup"><span data-stu-id="f6f94-157">tenantId</span></span> | <span data-ttu-id="f6f94-158">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="f6f94-158">guid</span></span> | <span data-ttu-id="f6f94-159">从其发出更改通知的租户的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="f6f94-159">The unique identified of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f6f94-160">关系</span><span class="sxs-lookup"><span data-stu-id="f6f94-160">Relationships</span></span>

<span data-ttu-id="f6f94-161">无。</span><span class="sxs-lookup"><span data-stu-id="f6f94-161">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6f94-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6f94-162">JSON representation</span></span>

<span data-ttu-id="f6f94-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6f94-163">The following is a JSON representation of the resource.</span></span>

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
  // Other properties typical in a resource change notification
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
