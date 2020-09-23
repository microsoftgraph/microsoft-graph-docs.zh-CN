---
title: changeNotification 资源类型
description: 表示发送给订阅者的更改通知。
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: ab8533f85e541947dccfc4c76989c100c64020cf
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193463"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="2dfa9-103">changeNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="2dfa9-103">changeNotification resource type</span></span>

<span data-ttu-id="2dfa9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dfa9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2dfa9-105">表示发送给订阅者的通知。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="2dfa9-106">有关详细信息，请参阅 [使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2dfa9-107">方法</span><span class="sxs-lookup"><span data-stu-id="2dfa9-107">Methods</span></span>

<span data-ttu-id="2dfa9-108">无。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="2dfa9-109">属性</span><span class="sxs-lookup"><span data-stu-id="2dfa9-109">Properties</span></span>

| <span data-ttu-id="2dfa9-110">属性</span><span class="sxs-lookup"><span data-stu-id="2dfa9-110">Property</span></span> | <span data-ttu-id="2dfa9-111">类型</span><span class="sxs-lookup"><span data-stu-id="2dfa9-111">Type</span></span> | <span data-ttu-id="2dfa9-112">说明</span><span class="sxs-lookup"><span data-stu-id="2dfa9-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="2dfa9-113">changeType</span><span class="sxs-lookup"><span data-stu-id="2dfa9-113">changeType</span></span> | <span data-ttu-id="2dfa9-114">string</span><span class="sxs-lookup"><span data-stu-id="2dfa9-114">string</span></span> | <span data-ttu-id="2dfa9-115">指示将引发更改通知的更改的类型。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="2dfa9-116">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="2dfa9-117">必需。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-117">Required.</span></span> |
| <span data-ttu-id="2dfa9-118">clientState</span><span class="sxs-lookup"><span data-stu-id="2dfa9-118">clientState</span></span> | <span data-ttu-id="2dfa9-119">string</span><span class="sxs-lookup"><span data-stu-id="2dfa9-119">string</span></span> | <span data-ttu-id="2dfa9-120">在订阅请求中发送的 **clientState** 属性的值 (如果有任何) 。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-120">Value of the **clientState** property sent in the subscription request (if any).</span></span> <span data-ttu-id="2dfa9-121">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="2dfa9-122">客户端可以通过比较 **clientState** 属性的值，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="2dfa9-123">与订阅一起发送的 **clientState** 属性的值将与每个更改通知收到的 **clientState** 属性的值进行比较。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="2dfa9-124">可选。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-124">Optional.</span></span> |
| <span data-ttu-id="2dfa9-125">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="2dfa9-125">encryptedContent</span></span> | [<span data-ttu-id="2dfa9-126">changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="2dfa9-126">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="2dfa9-127"> (预览) 随更改通知附加的加密内容。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="2dfa9-128">仅当 **encryptionCertificate** 和 **includeResourceData** 在订阅请求期间定义并且资源支持它时才提供。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="2dfa9-129">可选。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-129">Optional.</span></span> |
| <span data-ttu-id="2dfa9-130">id</span><span class="sxs-lookup"><span data-stu-id="2dfa9-130">id</span></span> | <span data-ttu-id="2dfa9-131">string</span><span class="sxs-lookup"><span data-stu-id="2dfa9-131">string</span></span> | <span data-ttu-id="2dfa9-132">通知的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-132">Unique ID for the notification.</span></span> <span data-ttu-id="2dfa9-133">可选。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-133">Optional.</span></span> |
| <span data-ttu-id="2dfa9-134">resource</span><span class="sxs-lookup"><span data-stu-id="2dfa9-134">resource</span></span> | <span data-ttu-id="2dfa9-135">string</span><span class="sxs-lookup"><span data-stu-id="2dfa9-135">string</span></span> | <span data-ttu-id="2dfa9-136">发出更改通知的资源的 URI （相对于） `https://graph.microsoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-136">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="2dfa9-137">必需。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-137">Required.</span></span> |
| <span data-ttu-id="2dfa9-138">resourceData</span><span class="sxs-lookup"><span data-stu-id="2dfa9-138">resourceData</span></span> | [<span data-ttu-id="2dfa9-139">resourceData</span><span class="sxs-lookup"><span data-stu-id="2dfa9-139">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="2dfa9-140">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-140">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="2dfa9-141">必需。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-141">Required.</span></span> |
| <span data-ttu-id="2dfa9-142">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2dfa9-142">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="2dfa9-143">dateTime</span><span class="sxs-lookup"><span data-stu-id="2dfa9-143">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="2dfa9-144">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-144">The expiration time for the subscription.</span></span> <span data-ttu-id="2dfa9-145">必需。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-145">Required.</span></span> |
| <span data-ttu-id="2dfa9-146">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="2dfa9-146">subscriptionId</span></span> | <span data-ttu-id="2dfa9-147">string</span><span class="sxs-lookup"><span data-stu-id="2dfa9-147">string</span></span> | <span data-ttu-id="2dfa9-148">生成通知的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-148">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="2dfa9-149">tenantId</span><span class="sxs-lookup"><span data-stu-id="2dfa9-149">tenantId</span></span> | <span data-ttu-id="2dfa9-150">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="2dfa9-150">guid</span></span> | <span data-ttu-id="2dfa9-151">来自其发出更改通知的租户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-151">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2dfa9-152">关系</span><span class="sxs-lookup"><span data-stu-id="2dfa9-152">Relationships</span></span>

<span data-ttu-id="2dfa9-153">无。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dfa9-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2dfa9-154">JSON representation</span></span>

<span data-ttu-id="2dfa9-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dfa9-155">The following is a JSON representation of the resource.</span></span>

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

