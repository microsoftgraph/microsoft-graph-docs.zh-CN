---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 563d232d200797b87e894292e31eb48ad88bf540
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342877"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="dd58c-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="dd58c-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd58c-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="dd58c-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="dd58c-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="dd58c-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="dd58c-107">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="dd58c-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="dd58c-108">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="dd58c-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="dd58c-109">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="dd58c-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="dd58c-110">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="dd58c-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="dd58c-111">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="dd58c-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd58c-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd58c-112">JSON representation</span></span>

<span data-ttu-id="dd58c-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd58c-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd58c-114">属性</span><span class="sxs-lookup"><span data-stu-id="dd58c-114">Properties</span></span>

| <span data-ttu-id="dd58c-115">属性</span><span class="sxs-lookup"><span data-stu-id="dd58c-115">Property</span></span> | <span data-ttu-id="dd58c-116">类型</span><span class="sxs-lookup"><span data-stu-id="dd58c-116">Type</span></span> | <span data-ttu-id="dd58c-117">说明</span><span class="sxs-lookup"><span data-stu-id="dd58c-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="dd58c-118">changeType</span><span class="sxs-lookup"><span data-stu-id="dd58c-118">changeType</span></span> | <span data-ttu-id="dd58c-119">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-119">string</span></span> | <span data-ttu-id="dd58c-120">必需。</span><span class="sxs-lookup"><span data-stu-id="dd58c-120">Required.</span></span> <span data-ttu-id="dd58c-121">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="dd58c-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="dd58c-122">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="dd58c-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="dd58c-123">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="dd58c-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="dd58c-124">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="dd58c-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="dd58c-125">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="dd58c-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="dd58c-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="dd58c-126">notificationUrl</span></span> | <span data-ttu-id="dd58c-127">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-127">string</span></span> | <span data-ttu-id="dd58c-128">必需。</span><span class="sxs-lookup"><span data-stu-id="dd58c-128">Required.</span></span> <span data-ttu-id="dd58c-129">接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="dd58c-129">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="dd58c-130">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="dd58c-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="dd58c-131">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="dd58c-131">lifecycleNotificationUrl</span></span> | <span data-ttu-id="dd58c-132">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-132">string</span></span> | <span data-ttu-id="dd58c-133">可选。</span><span class="sxs-lookup"><span data-stu-id="dd58c-133">Optional.</span></span> <span data-ttu-id="dd58c-134">接收生命周期通知 (包括`subscriptionRemoved`和`missed`通知) 的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="dd58c-134">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="dd58c-135">如果未提供, 这些通知将传递给**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="dd58c-135">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="dd58c-136">[阅读](/graph/webhooks-outlook-authz.md)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dd58c-136">[Read more](/graph/webhooks-outlook-authz.md) about how Outlook resources use lifecycle notifications.</span></span>  <span data-ttu-id="dd58c-137">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="dd58c-137">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="dd58c-138">resource</span><span class="sxs-lookup"><span data-stu-id="dd58c-138">resource</span></span> | <span data-ttu-id="dd58c-139">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-139">string</span></span> | <span data-ttu-id="dd58c-140">必需。</span><span class="sxs-lookup"><span data-stu-id="dd58c-140">Required.</span></span> <span data-ttu-id="dd58c-141">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="dd58c-141">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="dd58c-142">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="dd58c-142">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="dd58c-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dd58c-143">expirationDateTime</span></span> | <span data-ttu-id="dd58c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd58c-144">DateTimeOffset</span></span> | <span data-ttu-id="dd58c-145">必需。</span><span class="sxs-lookup"><span data-stu-id="dd58c-145">Required.</span></span> <span data-ttu-id="dd58c-146">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dd58c-146">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="dd58c-147">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="dd58c-147">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="dd58c-148">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="dd58c-148">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="dd58c-149">clientState</span><span class="sxs-lookup"><span data-stu-id="dd58c-149">clientState</span></span> | <span data-ttu-id="dd58c-150">字符串</span><span class="sxs-lookup"><span data-stu-id="dd58c-150">string</span></span> | <span data-ttu-id="dd58c-151">可选。</span><span class="sxs-lookup"><span data-stu-id="dd58c-151">Optional.</span></span> <span data-ttu-id="dd58c-152">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="dd58c-152">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="dd58c-153">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="dd58c-153">The maximum length is 255 characters.</span></span> <span data-ttu-id="dd58c-154">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="dd58c-154">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="dd58c-155">id</span><span class="sxs-lookup"><span data-stu-id="dd58c-155">id</span></span> | <span data-ttu-id="dd58c-156">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-156">string</span></span> | <span data-ttu-id="dd58c-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="dd58c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="dd58c-159">applicationId</span><span class="sxs-lookup"><span data-stu-id="dd58c-159">applicationId</span></span> | <span data-ttu-id="dd58c-160">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-160">string</span></span> | <span data-ttu-id="dd58c-161">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="dd58c-161">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="dd58c-162">只读。</span><span class="sxs-lookup"><span data-stu-id="dd58c-162">Read-only.</span></span> |
| <span data-ttu-id="dd58c-163">creatorId</span><span class="sxs-lookup"><span data-stu-id="dd58c-163">creatorId</span></span> | <span data-ttu-id="dd58c-164">string</span><span class="sxs-lookup"><span data-stu-id="dd58c-164">string</span></span> | <span data-ttu-id="dd58c-165">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="dd58c-165">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="dd58c-166">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="dd58c-166">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="dd58c-167">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="dd58c-167">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="dd58c-168">只读。</span><span class="sxs-lookup"><span data-stu-id="dd58c-168">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="dd58c-169">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="dd58c-169">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="dd58c-170">资源</span><span class="sxs-lookup"><span data-stu-id="dd58c-170">Resource</span></span>            | <span data-ttu-id="dd58c-171">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="dd58c-171">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="dd58c-172">邮件</span><span class="sxs-lookup"><span data-stu-id="dd58c-172">Mail</span></span>                | <span data-ttu-id="dd58c-173">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dd58c-173">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dd58c-174">日历</span><span class="sxs-lookup"><span data-stu-id="dd58c-174">Calendar</span></span>            | <span data-ttu-id="dd58c-175">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dd58c-175">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dd58c-176">联系人</span><span class="sxs-lookup"><span data-stu-id="dd58c-176">Contacts</span></span>            | <span data-ttu-id="dd58c-177">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dd58c-177">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dd58c-178">组对话</span><span class="sxs-lookup"><span data-stu-id="dd58c-178">Group conversations</span></span> | <span data-ttu-id="dd58c-179">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dd58c-179">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dd58c-180">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="dd58c-180">Drive root items</span></span>    | <span data-ttu-id="dd58c-181">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dd58c-181">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dd58c-182">安全警报</span><span class="sxs-lookup"><span data-stu-id="dd58c-182">Security alerts</span></span>     | <span data-ttu-id="dd58c-183">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="dd58c-183">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="dd58c-184">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="dd58c-184">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="dd58c-185">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="dd58c-185">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="dd58c-186">关系</span><span class="sxs-lookup"><span data-stu-id="dd58c-186">Relationships</span></span>

<span data-ttu-id="dd58c-187">无</span><span class="sxs-lookup"><span data-stu-id="dd58c-187">None</span></span>

## <a name="methods"></a><span data-ttu-id="dd58c-188">方法</span><span class="sxs-lookup"><span data-stu-id="dd58c-188">Methods</span></span>

| <span data-ttu-id="dd58c-189">方法</span><span class="sxs-lookup"><span data-stu-id="dd58c-189">Method</span></span> | <span data-ttu-id="dd58c-190">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd58c-190">Return Type</span></span> | <span data-ttu-id="dd58c-191">说明</span><span class="sxs-lookup"><span data-stu-id="dd58c-191">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="dd58c-192">创建订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-192">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="dd58c-193">订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-193">subscription</span></span>](subscription.md) | <span data-ttu-id="dd58c-194">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="dd58c-194">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="dd58c-195">更新订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-195">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="dd58c-196">订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-196">subscription</span></span>](subscription.md) | <span data-ttu-id="dd58c-197">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="dd58c-197">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="dd58c-198">列出订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-198">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="dd58c-199">订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-199">subscription</span></span>](subscription.md) | <span data-ttu-id="dd58c-200">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="dd58c-200">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="dd58c-201">获取订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-201">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="dd58c-202">订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-202">subscription</span></span>](subscription.md) | <span data-ttu-id="dd58c-203">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd58c-203">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="dd58c-204">删除订阅</span><span class="sxs-lookup"><span data-stu-id="dd58c-204">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="dd58c-205">无</span><span class="sxs-lookup"><span data-stu-id="dd58c-205">None</span></span> | <span data-ttu-id="dd58c-206">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="dd58c-206">Delete a subscription object.</span></span> |

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
