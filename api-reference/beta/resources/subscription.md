---
title: 订阅资源类型
description: 订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。 目前，订阅启用以下资源：
localization_priority: Normal
ms.openlocfilehash: 4879bd4afd68915200364b70ea6787e06e8c629b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813214"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="21eed-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="21eed-104">subscription resource type</span></span>

> <span data-ttu-id="21eed-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="21eed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21eed-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21eed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21eed-107">订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。</span><span class="sxs-lookup"><span data-stu-id="21eed-107">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="21eed-108">目前，订阅启用以下资源：</span><span class="sxs-lookup"><span data-stu-id="21eed-108">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="21eed-109">邮件、 事件和 Outlook 中的联系人。</span><span class="sxs-lookup"><span data-stu-id="21eed-109">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="21eed-110">来自 Office 组的对话。</span><span class="sxs-lookup"><span data-stu-id="21eed-110">Conversations from Office Groups.</span></span>
- <span data-ttu-id="21eed-111">从 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="21eed-111">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="21eed-112">用户和 Azure Active Directory 组。</span><span class="sxs-lookup"><span data-stu-id="21eed-112">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="21eed-113">来自 Microsoft Graph 安全 API 的通知。</span><span class="sxs-lookup"><span data-stu-id="21eed-113">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21eed-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21eed-114">JSON representation</span></span>

<span data-ttu-id="21eed-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21eed-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="21eed-116">属性</span><span class="sxs-lookup"><span data-stu-id="21eed-116">Properties</span></span>

| <span data-ttu-id="21eed-117">属性</span><span class="sxs-lookup"><span data-stu-id="21eed-117">Property</span></span> | <span data-ttu-id="21eed-118">类型</span><span class="sxs-lookup"><span data-stu-id="21eed-118">Type</span></span> | <span data-ttu-id="21eed-119">说明</span><span class="sxs-lookup"><span data-stu-id="21eed-119">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="21eed-120">changeType</span><span class="sxs-lookup"><span data-stu-id="21eed-120">changeType</span></span> | <span data-ttu-id="21eed-121">string</span><span class="sxs-lookup"><span data-stu-id="21eed-121">string</span></span> | <span data-ttu-id="21eed-122">必需。</span><span class="sxs-lookup"><span data-stu-id="21eed-122">Required.</span></span> <span data-ttu-id="21eed-123">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="21eed-123">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="21eed-124">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="21eed-124">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="21eed-125">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="21eed-125">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="21eed-126">注意： 驱动器根项目通知仅支持`updated`changeType。</span><span class="sxs-lookup"><span data-stu-id="21eed-126">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="21eed-127">用户和组通知支持`updated`和`deleted`changeType。</span><span class="sxs-lookup"><span data-stu-id="21eed-127">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="21eed-128">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="21eed-128">notificationUrl</span></span> | <span data-ttu-id="21eed-129">string</span><span class="sxs-lookup"><span data-stu-id="21eed-129">string</span></span> | <span data-ttu-id="21eed-130">必需。</span><span class="sxs-lookup"><span data-stu-id="21eed-130">Required.</span></span> <span data-ttu-id="21eed-131">将接收通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="21eed-131">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="21eed-132">此 URL 必须进行使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="21eed-132">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="21eed-133">resource</span><span class="sxs-lookup"><span data-stu-id="21eed-133">resource</span></span> | <span data-ttu-id="21eed-134">string</span><span class="sxs-lookup"><span data-stu-id="21eed-134">string</span></span> | <span data-ttu-id="21eed-135">必需。</span><span class="sxs-lookup"><span data-stu-id="21eed-135">Required.</span></span> <span data-ttu-id="21eed-136">指定将监视的更改的资源。</span><span class="sxs-lookup"><span data-stu-id="21eed-136">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="21eed-137">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="21eed-137">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="21eed-138">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21eed-138">expirationDateTime</span></span> | <span data-ttu-id="21eed-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21eed-139">DateTimeOffset</span></span> | <span data-ttu-id="21eed-140">必填。</span><span class="sxs-lookup"><span data-stu-id="21eed-140">Required.</span></span> <span data-ttu-id="21eed-141">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="21eed-141">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="21eed-142">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="21eed-142">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="21eed-143">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="21eed-143">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="21eed-144">clientState</span><span class="sxs-lookup"><span data-stu-id="21eed-144">clientState</span></span> | <span data-ttu-id="21eed-145">string</span><span class="sxs-lookup"><span data-stu-id="21eed-145">string</span></span> | <span data-ttu-id="21eed-146">可选。</span><span class="sxs-lookup"><span data-stu-id="21eed-146">Optional.</span></span> <span data-ttu-id="21eed-147">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="21eed-147">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="21eed-148">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="21eed-148">The maximum length is 255 characters.</span></span> <span data-ttu-id="21eed-149">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="21eed-149">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="21eed-150">id</span><span class="sxs-lookup"><span data-stu-id="21eed-150">id</span></span> | <span data-ttu-id="21eed-151">string</span><span class="sxs-lookup"><span data-stu-id="21eed-151">string</span></span> | <span data-ttu-id="21eed-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="21eed-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="21eed-154">applicationId</span><span class="sxs-lookup"><span data-stu-id="21eed-154">applicationId</span></span> | <span data-ttu-id="21eed-155">string</span><span class="sxs-lookup"><span data-stu-id="21eed-155">string</span></span> | <span data-ttu-id="21eed-156">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="21eed-156">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="21eed-157">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="21eed-157">Read-only.</span></span> |
| <span data-ttu-id="21eed-158">creatorId</span><span class="sxs-lookup"><span data-stu-id="21eed-158">creatorId</span></span> | <span data-ttu-id="21eed-159">string</span><span class="sxs-lookup"><span data-stu-id="21eed-159">string</span></span> | <span data-ttu-id="21eed-160">用户或创建订阅的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="21eed-160">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="21eed-161">如果应用程序使用委派权限创建订阅，此字段包含应用程序调用代表登录用户的 id。</span><span class="sxs-lookup"><span data-stu-id="21eed-161">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="21eed-162">如果应用程序使用应用程序权限，此字段包含对应于应用程序的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="21eed-162">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="21eed-163">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="21eed-163">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="21eed-164">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="21eed-164">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="21eed-165">资源</span><span class="sxs-lookup"><span data-stu-id="21eed-165">Resource</span></span>            | <span data-ttu-id="21eed-166">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="21eed-166">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="21eed-167">邮件</span><span class="sxs-lookup"><span data-stu-id="21eed-167">Mail</span></span>                | <span data-ttu-id="21eed-168">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="21eed-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="21eed-169">日历</span><span class="sxs-lookup"><span data-stu-id="21eed-169">Calendar</span></span>            | <span data-ttu-id="21eed-170">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="21eed-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="21eed-171">联系人</span><span class="sxs-lookup"><span data-stu-id="21eed-171">Contacts</span></span>            | <span data-ttu-id="21eed-172">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="21eed-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="21eed-173">组对话</span><span class="sxs-lookup"><span data-stu-id="21eed-173">Group conversations</span></span> | <span data-ttu-id="21eed-174">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="21eed-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="21eed-175">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="21eed-175">Drive root items</span></span>    | <span data-ttu-id="21eed-176">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="21eed-176">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="21eed-177">安全警报</span><span class="sxs-lookup"><span data-stu-id="21eed-177">Security alerts</span></span>     | <span data-ttu-id="21eed-178">43200 分钟 （在 30 天）</span><span class="sxs-lookup"><span data-stu-id="21eed-178">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="21eed-179">**注意：** 现有应用程序和新的应用程序不应超过受支持的值。</span><span class="sxs-lookup"><span data-stu-id="21eed-179">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="21eed-180">将来，任何创建或更新的最大值超出订阅已请求将失败。</span><span class="sxs-lookup"><span data-stu-id="21eed-180">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="21eed-181">Relationships</span><span class="sxs-lookup"><span data-stu-id="21eed-181">Relationships</span></span>

<span data-ttu-id="21eed-182">无</span><span class="sxs-lookup"><span data-stu-id="21eed-182">None</span></span>

## <a name="methods"></a><span data-ttu-id="21eed-183">方法</span><span class="sxs-lookup"><span data-stu-id="21eed-183">Methods</span></span>

| <span data-ttu-id="21eed-184">方法</span><span class="sxs-lookup"><span data-stu-id="21eed-184">Method</span></span> | <span data-ttu-id="21eed-185">返回类型</span><span class="sxs-lookup"><span data-stu-id="21eed-185">Return Type</span></span> | <span data-ttu-id="21eed-186">说明</span><span class="sxs-lookup"><span data-stu-id="21eed-186">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="21eed-187">创建订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-187">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="21eed-188">订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-188">subscription</span></span>](subscription.md) | <span data-ttu-id="21eed-189">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="21eed-189">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="21eed-190">更新订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-190">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="21eed-191">订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-191">subscription</span></span>](subscription.md) | <span data-ttu-id="21eed-192">通过更新其过期时间续订。</span><span class="sxs-lookup"><span data-stu-id="21eed-192">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="21eed-193">列表订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-193">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="21eed-194">订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-194">subscription</span></span>](subscription.md) | <span data-ttu-id="21eed-195">列出了活动订阅。</span><span class="sxs-lookup"><span data-stu-id="21eed-195">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="21eed-196">获取订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-196">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="21eed-197">订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-197">subscription</span></span>](subscription.md) | <span data-ttu-id="21eed-198">读取属性和订阅对象的关系。</span><span class="sxs-lookup"><span data-stu-id="21eed-198">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="21eed-199">删除订阅</span><span class="sxs-lookup"><span data-stu-id="21eed-199">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="21eed-200">无</span><span class="sxs-lookup"><span data-stu-id="21eed-200">None</span></span> | <span data-ttu-id="21eed-201">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="21eed-201">Delete a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
