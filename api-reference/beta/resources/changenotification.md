---
title: changeNotification 资源类型
description: 表示发送给订阅者更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 43933d31b8ac12f77331887c0421c3b6fc50b66b
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082375"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="11477-103">changeNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="11477-103">changeNotification resource type</span></span>

<span data-ttu-id="11477-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11477-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11477-105">表示发送给订阅者的通知。</span><span class="sxs-lookup"><span data-stu-id="11477-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="11477-106">有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="11477-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="11477-107">方法</span><span class="sxs-lookup"><span data-stu-id="11477-107">Methods</span></span>

<span data-ttu-id="11477-108">无。</span><span class="sxs-lookup"><span data-stu-id="11477-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="11477-109">属性</span><span class="sxs-lookup"><span data-stu-id="11477-109">Properties</span></span>

| <span data-ttu-id="11477-110">属性</span><span class="sxs-lookup"><span data-stu-id="11477-110">Property</span></span> | <span data-ttu-id="11477-111">类型</span><span class="sxs-lookup"><span data-stu-id="11477-111">Type</span></span> | <span data-ttu-id="11477-112">说明</span><span class="sxs-lookup"><span data-stu-id="11477-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="11477-113">changeType</span><span class="sxs-lookup"><span data-stu-id="11477-113">changeType</span></span> | <span data-ttu-id="11477-114">changeType</span><span class="sxs-lookup"><span data-stu-id="11477-114">changeType</span></span> | <span data-ttu-id="11477-115">指示将引发更改通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="11477-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="11477-116">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="11477-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="11477-117">必填。</span><span class="sxs-lookup"><span data-stu-id="11477-117">Required.</span></span> |
| <span data-ttu-id="11477-118">clientState</span><span class="sxs-lookup"><span data-stu-id="11477-118">clientState</span></span> | <span data-ttu-id="11477-119">string</span><span class="sxs-lookup"><span data-stu-id="11477-119">string</span></span> | <span data-ttu-id="11477-120">订阅请求请求中指定的 **clientState** 属性的值 (（如果有) ）。</span><span class="sxs-lookup"><span data-stu-id="11477-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="11477-121">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="11477-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="11477-122">客户端可以通过比较 **clientState** 属性的值来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="11477-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="11477-123">与订阅一起发送的 **clientState** 属性的值与每次更改通知时收到的 **clientState** 属性的值进行比较。</span><span class="sxs-lookup"><span data-stu-id="11477-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="11477-124">可选。</span><span class="sxs-lookup"><span data-stu-id="11477-124">Optional.</span></span> |
| <span data-ttu-id="11477-125">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="11477-125">encryptedContent</span></span> | [<span data-ttu-id="11477-126">changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="11477-126">changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="11477-127"> (预览) 更改通知附加的加密内容。</span><span class="sxs-lookup"><span data-stu-id="11477-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="11477-128">仅在订阅 **请求期间定义了 encryptionCertificate** 和 **includeResourceData** 且资源支持它时提供。</span><span class="sxs-lookup"><span data-stu-id="11477-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="11477-129">可选。</span><span class="sxs-lookup"><span data-stu-id="11477-129">Optional.</span></span> |
| <span data-ttu-id="11477-130">id</span><span class="sxs-lookup"><span data-stu-id="11477-130">id</span></span> | <span data-ttu-id="11477-131">string</span><span class="sxs-lookup"><span data-stu-id="11477-131">string</span></span> | <span data-ttu-id="11477-132">通知的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="11477-132">Unique ID for the notification.</span></span> <span data-ttu-id="11477-133">可选。</span><span class="sxs-lookup"><span data-stu-id="11477-133">Optional.</span></span> |
| <span data-ttu-id="11477-134">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="11477-134">lifecycleEvent</span></span> | <span data-ttu-id="11477-135">lifecycleEventType</span><span class="sxs-lookup"><span data-stu-id="11477-135">lifecycleEventType</span></span> | <span data-ttu-id="11477-136">如果当前通知是生命周期通知，则生命周期通知的类型。</span><span class="sxs-lookup"><span data-stu-id="11477-136">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="11477-137">可选。</span><span class="sxs-lookup"><span data-stu-id="11477-137">Optional.</span></span> <span data-ttu-id="11477-138">支持的值是 `missed` `removed` `reauthorizationRequired` 、、。</span><span class="sxs-lookup"><span data-stu-id="11477-138">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="11477-139">resource</span><span class="sxs-lookup"><span data-stu-id="11477-139">resource</span></span> | <span data-ttu-id="11477-140">string</span><span class="sxs-lookup"><span data-stu-id="11477-140">string</span></span> | <span data-ttu-id="11477-141">发出更改通知的资源相对于 的 `https://graph.microsoft.com` URI。</span><span class="sxs-lookup"><span data-stu-id="11477-141">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="11477-142">必填。</span><span class="sxs-lookup"><span data-stu-id="11477-142">Required.</span></span> |
| <span data-ttu-id="11477-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="11477-143">resourceData</span></span> | [<span data-ttu-id="11477-144">resourceData</span><span class="sxs-lookup"><span data-stu-id="11477-144">resourceData</span></span>](resourcedata.md) | <span data-ttu-id="11477-145">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="11477-145">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="11477-146">必填。</span><span class="sxs-lookup"><span data-stu-id="11477-146">Required.</span></span> |
| <span data-ttu-id="11477-147">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="11477-147">subscriptionExpirationDateTime</span></span> | <span data-ttu-id="11477-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11477-148">DateTimeOffset</span></span> | <span data-ttu-id="11477-149">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="11477-149">The expiration time for the subscription.</span></span> <span data-ttu-id="11477-150">必填。</span><span class="sxs-lookup"><span data-stu-id="11477-150">Required.</span></span> |
| <span data-ttu-id="11477-151">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="11477-151">subscriptionId</span></span> | <span data-ttu-id="11477-152">GUID</span><span class="sxs-lookup"><span data-stu-id="11477-152">GUID</span></span> | <span data-ttu-id="11477-153">生成通知的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="11477-153">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="11477-154">tenantId</span><span class="sxs-lookup"><span data-stu-id="11477-154">tenantId</span></span> | <span data-ttu-id="11477-155">GUID</span><span class="sxs-lookup"><span data-stu-id="11477-155">GUID</span></span> | <span data-ttu-id="11477-156">源自更改通知的租户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="11477-156">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="11477-157">关系</span><span class="sxs-lookup"><span data-stu-id="11477-157">Relationships</span></span>

<span data-ttu-id="11477-158">无。</span><span class="sxs-lookup"><span data-stu-id="11477-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11477-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11477-159">JSON representation</span></span>

<span data-ttu-id="11477-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11477-160">The following is a JSON representation of the resource.</span></span>

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


