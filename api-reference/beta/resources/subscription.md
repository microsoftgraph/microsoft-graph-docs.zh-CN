---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 6a7fd50a53e68313ba72c8bd5d90b47d2b5b2607
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537203"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="2cf7e-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="2cf7e-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cf7e-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="2cf7e-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="2cf7e-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="2cf7e-107">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="2cf7e-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="2cf7e-108">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="2cf7e-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="2cf7e-109">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="2cf7e-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="2cf7e-110">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="2cf7e-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="2cf7e-111">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="2cf7e-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="2cf7e-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cf7e-112">JSON representation</span></span>

<span data-ttu-id="2cf7e-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-113">Here is a JSON representation of the resource.</span></span>

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
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2cf7e-114">属性</span><span class="sxs-lookup"><span data-stu-id="2cf7e-114">Properties</span></span>

| <span data-ttu-id="2cf7e-115">属性</span><span class="sxs-lookup"><span data-stu-id="2cf7e-115">Property</span></span> | <span data-ttu-id="2cf7e-116">类型</span><span class="sxs-lookup"><span data-stu-id="2cf7e-116">Type</span></span> | <span data-ttu-id="2cf7e-117">说明</span><span class="sxs-lookup"><span data-stu-id="2cf7e-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="2cf7e-118">changeType</span><span class="sxs-lookup"><span data-stu-id="2cf7e-118">changeType</span></span> | <span data-ttu-id="2cf7e-119">string</span><span class="sxs-lookup"><span data-stu-id="2cf7e-119">string</span></span> | <span data-ttu-id="2cf7e-120">必需。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-120">Required.</span></span> <span data-ttu-id="2cf7e-121">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="2cf7e-122">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="2cf7e-123">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="2cf7e-124">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="2cf7e-125">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="2cf7e-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="2cf7e-126">notificationUrl</span></span> | <span data-ttu-id="2cf7e-127">string</span><span class="sxs-lookup"><span data-stu-id="2cf7e-127">string</span></span> | <span data-ttu-id="2cf7e-128">必需。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-128">Required.</span></span> <span data-ttu-id="2cf7e-129">接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-129">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="2cf7e-130">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="2cf7e-131">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="2cf7e-131">lifecycleNotificationUrl</span></span> | <span data-ttu-id="2cf7e-132">string</span><span class="sxs-lookup"><span data-stu-id="2cf7e-132">string</span></span> | <span data-ttu-id="2cf7e-133">可选。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-133">Optional.</span></span> <span data-ttu-id="2cf7e-134">接收生命周期通知 (包括`subscriptionRemoved`和`missed`通知) 的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-134">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="2cf7e-135">如果未提供, 这些通知将传递给**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-135">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="2cf7e-136">[阅读](/graph/webhooks-outlook-authz.md)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-136">[Read more](/graph/webhooks-outlook-authz.md) about how Outlook resources use lifecycle notifications.</span></span>  <span data-ttu-id="2cf7e-137">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-137">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="2cf7e-138">resource</span><span class="sxs-lookup"><span data-stu-id="2cf7e-138">resource</span></span> | <span data-ttu-id="2cf7e-139">string</span><span class="sxs-lookup"><span data-stu-id="2cf7e-139">string</span></span> | <span data-ttu-id="2cf7e-140">必需。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-140">Required.</span></span> <span data-ttu-id="2cf7e-141">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-141">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="2cf7e-142">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-142">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="2cf7e-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2cf7e-143">expirationDateTime</span></span> | <span data-ttu-id="2cf7e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cf7e-144">DateTimeOffset</span></span> | <span data-ttu-id="2cf7e-145">必需。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-145">Required.</span></span> <span data-ttu-id="2cf7e-146">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-146">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="2cf7e-147">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-147">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="2cf7e-148">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-148">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="2cf7e-149">clientState</span><span class="sxs-lookup"><span data-stu-id="2cf7e-149">clientState</span></span> | <span data-ttu-id="2cf7e-150">字符串</span><span class="sxs-lookup"><span data-stu-id="2cf7e-150">string</span></span> | <span data-ttu-id="2cf7e-151">可选。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-151">Optional.</span></span> <span data-ttu-id="2cf7e-152">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-152">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="2cf7e-153">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-153">The maximum length is 255 characters.</span></span> <span data-ttu-id="2cf7e-154">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-154">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="2cf7e-155">id</span><span class="sxs-lookup"><span data-stu-id="2cf7e-155">id</span></span> | <span data-ttu-id="2cf7e-156">string</span><span class="sxs-lookup"><span data-stu-id="2cf7e-156">string</span></span> | <span data-ttu-id="2cf7e-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="2cf7e-159">applicationId</span><span class="sxs-lookup"><span data-stu-id="2cf7e-159">applicationId</span></span> | <span data-ttu-id="2cf7e-160">字符串</span><span class="sxs-lookup"><span data-stu-id="2cf7e-160">string</span></span> | <span data-ttu-id="2cf7e-161">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-161">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="2cf7e-162">只读。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-162">Read-only.</span></span> |
| <span data-ttu-id="2cf7e-163">creatorId</span><span class="sxs-lookup"><span data-stu-id="2cf7e-163">creatorId</span></span> | <span data-ttu-id="2cf7e-164">string</span><span class="sxs-lookup"><span data-stu-id="2cf7e-164">string</span></span> | <span data-ttu-id="2cf7e-165">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-165">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="2cf7e-166">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-166">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="2cf7e-167">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-167">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="2cf7e-168">只读。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-168">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="2cf7e-169">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="2cf7e-169">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="2cf7e-170">资源</span><span class="sxs-lookup"><span data-stu-id="2cf7e-170">Resource</span></span>            | <span data-ttu-id="2cf7e-171">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="2cf7e-171">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="2cf7e-172">用户、组、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="2cf7e-172">User, group, other directory resources</span></span>   | <span data-ttu-id="2cf7e-173">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-173">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2cf7e-174">邮件</span><span class="sxs-lookup"><span data-stu-id="2cf7e-174">Mail</span></span>                | <span data-ttu-id="2cf7e-175">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-175">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2cf7e-176">日历</span><span class="sxs-lookup"><span data-stu-id="2cf7e-176">Calendar</span></span>            | <span data-ttu-id="2cf7e-177">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-177">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2cf7e-178">联系人</span><span class="sxs-lookup"><span data-stu-id="2cf7e-178">Contacts</span></span>            | <span data-ttu-id="2cf7e-179">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-179">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2cf7e-180">组对话</span><span class="sxs-lookup"><span data-stu-id="2cf7e-180">Group conversations</span></span> | <span data-ttu-id="2cf7e-181">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-181">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2cf7e-182">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="2cf7e-182">Drive root items</span></span>    | <span data-ttu-id="2cf7e-183">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-183">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2cf7e-184">安全警报</span><span class="sxs-lookup"><span data-stu-id="2cf7e-184">Security alerts</span></span>     | <span data-ttu-id="2cf7e-185">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="2cf7e-185">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="2cf7e-186">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-186">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="2cf7e-187">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-187">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="2cf7e-188">关系</span><span class="sxs-lookup"><span data-stu-id="2cf7e-188">Relationships</span></span>

<span data-ttu-id="2cf7e-189">无</span><span class="sxs-lookup"><span data-stu-id="2cf7e-189">None</span></span>

## <a name="methods"></a><span data-ttu-id="2cf7e-190">方法</span><span class="sxs-lookup"><span data-stu-id="2cf7e-190">Methods</span></span>

| <span data-ttu-id="2cf7e-191">方法</span><span class="sxs-lookup"><span data-stu-id="2cf7e-191">Method</span></span> | <span data-ttu-id="2cf7e-192">返回类型</span><span class="sxs-lookup"><span data-stu-id="2cf7e-192">Return Type</span></span> | <span data-ttu-id="2cf7e-193">说明</span><span class="sxs-lookup"><span data-stu-id="2cf7e-193">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="2cf7e-194">创建订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-194">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="2cf7e-195">订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-195">subscription</span></span>](subscription.md) | <span data-ttu-id="2cf7e-196">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-196">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="2cf7e-197">更新订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-197">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="2cf7e-198">订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-198">subscription</span></span>](subscription.md) | <span data-ttu-id="2cf7e-199">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-199">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="2cf7e-200">列出订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-200">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="2cf7e-201">订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-201">subscription</span></span>](subscription.md) | <span data-ttu-id="2cf7e-202">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-202">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="2cf7e-203">获取订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-203">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="2cf7e-204">订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-204">subscription</span></span>](subscription.md) | <span data-ttu-id="2cf7e-205">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-205">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="2cf7e-206">删除订阅</span><span class="sxs-lookup"><span data-stu-id="2cf7e-206">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="2cf7e-207">无</span><span class="sxs-lookup"><span data-stu-id="2cf7e-207">None</span></span> | <span data-ttu-id="2cf7e-208">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="2cf7e-208">Delete a subscription object.</span></span> |

[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[event]: ./event.md
[组]: ./group.md
[group]: ./group.md
[邮件]: ./message.md
[message]: ./message.md
[用户]: ./user.md
[user]: ./user.md
[警报]: ./alert.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
