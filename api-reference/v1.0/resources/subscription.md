---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cda3163cd7538c418338e5d2c6d1ab0a076b33ff
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159134"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="8d392-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="8d392-104">subscription resource type</span></span>

<span data-ttu-id="8d392-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="8d392-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="8d392-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="8d392-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="8d392-107">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="8d392-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="8d392-108">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="8d392-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="8d392-109">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="8d392-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="8d392-110">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="8d392-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="8d392-111">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="8d392-111">An [alert][] from the Microsoft Graph Security API</span></span>

<span data-ttu-id="8d392-112">有关每项资源支持的资源路径表达式（可在订阅的 **resource** 属性中使用），可查看[概述文章](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="8d392-112">The resource path expressions supported for each resource - that can be used in the **resource** property of the subscription - are documented in [the overview article](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8d392-113">方法</span><span class="sxs-lookup"><span data-stu-id="8d392-113">Methods</span></span>

| <span data-ttu-id="8d392-114">方法</span><span class="sxs-lookup"><span data-stu-id="8d392-114">Method</span></span> | <span data-ttu-id="8d392-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d392-115">Return Type</span></span> | <span data-ttu-id="8d392-116">说明</span><span class="sxs-lookup"><span data-stu-id="8d392-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="8d392-117">创建订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="8d392-118">订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-118">subscription</span></span>](subscription.md) | <span data-ttu-id="8d392-119">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="8d392-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="8d392-120">更新订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="8d392-121">订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-121">subscription</span></span>](subscription.md) | <span data-ttu-id="8d392-122">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="8d392-122">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="8d392-123">列出订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="8d392-124">订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-124">subscription</span></span>](subscription.md) | <span data-ttu-id="8d392-125">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="8d392-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="8d392-126">获取订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="8d392-127">订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-127">subscription</span></span>](subscription.md) | <span data-ttu-id="8d392-128">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d392-128">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="8d392-129">删除订阅</span><span class="sxs-lookup"><span data-stu-id="8d392-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="8d392-130">无</span><span class="sxs-lookup"><span data-stu-id="8d392-130">None</span></span> | <span data-ttu-id="8d392-131">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="8d392-131">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d392-132">属性</span><span class="sxs-lookup"><span data-stu-id="8d392-132">Properties</span></span>

| <span data-ttu-id="8d392-133">属性</span><span class="sxs-lookup"><span data-stu-id="8d392-133">Property</span></span> | <span data-ttu-id="8d392-134">类型</span><span class="sxs-lookup"><span data-stu-id="8d392-134">Type</span></span> | <span data-ttu-id="8d392-135">说明</span><span class="sxs-lookup"><span data-stu-id="8d392-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8d392-136">changeType</span><span class="sxs-lookup"><span data-stu-id="8d392-136">changeType</span></span> | <span data-ttu-id="8d392-137">string</span><span class="sxs-lookup"><span data-stu-id="8d392-137">string</span></span> | <span data-ttu-id="8d392-138">必需。</span><span class="sxs-lookup"><span data-stu-id="8d392-138">Required.</span></span> <span data-ttu-id="8d392-139">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="8d392-139">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="8d392-140">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="8d392-140">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="8d392-141">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="8d392-141">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="8d392-142">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="8d392-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="8d392-143">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="8d392-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="8d392-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="8d392-144">notificationUrl</span></span> | <span data-ttu-id="8d392-145">string</span><span class="sxs-lookup"><span data-stu-id="8d392-145">string</span></span> | <span data-ttu-id="8d392-146">必需。</span><span class="sxs-lookup"><span data-stu-id="8d392-146">Required.</span></span> <span data-ttu-id="8d392-147">将接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="8d392-147">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="8d392-148">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="8d392-148">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="8d392-149">resource</span><span class="sxs-lookup"><span data-stu-id="8d392-149">resource</span></span> | <span data-ttu-id="8d392-150">string</span><span class="sxs-lookup"><span data-stu-id="8d392-150">string</span></span> | <span data-ttu-id="8d392-151">必需。</span><span class="sxs-lookup"><span data-stu-id="8d392-151">Required.</span></span> <span data-ttu-id="8d392-152">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="8d392-152">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="8d392-153">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="8d392-153">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="8d392-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8d392-154">expirationDateTime</span></span> | [<span data-ttu-id="8d392-155">dateTime</span><span class="sxs-lookup"><span data-stu-id="8d392-155">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="8d392-156">必需。</span><span class="sxs-lookup"><span data-stu-id="8d392-156">Required.</span></span> <span data-ttu-id="8d392-157">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8d392-157">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="8d392-158">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="8d392-158">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="8d392-159">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="8d392-159">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="8d392-160">clientState</span><span class="sxs-lookup"><span data-stu-id="8d392-160">clientState</span></span> | <span data-ttu-id="8d392-161">字符串</span><span class="sxs-lookup"><span data-stu-id="8d392-161">string</span></span> | <span data-ttu-id="8d392-162">可选。</span><span class="sxs-lookup"><span data-stu-id="8d392-162">Optional.</span></span> <span data-ttu-id="8d392-163">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="8d392-163">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="8d392-164">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="8d392-164">The maximum length is 128 characters.</span></span> <span data-ttu-id="8d392-165">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="8d392-165">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="8d392-166">id</span><span class="sxs-lookup"><span data-stu-id="8d392-166">id</span></span> | <span data-ttu-id="8d392-167">string</span><span class="sxs-lookup"><span data-stu-id="8d392-167">string</span></span> | <span data-ttu-id="8d392-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8d392-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="8d392-170">applicationId</span><span class="sxs-lookup"><span data-stu-id="8d392-170">applicationId</span></span> | <span data-ttu-id="8d392-171">string</span><span class="sxs-lookup"><span data-stu-id="8d392-171">string</span></span> | <span data-ttu-id="8d392-172">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="8d392-172">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="8d392-173">只读。</span><span class="sxs-lookup"><span data-stu-id="8d392-173">Read-only.</span></span> |
| <span data-ttu-id="8d392-174">creatorId</span><span class="sxs-lookup"><span data-stu-id="8d392-174">creatorId</span></span> | <span data-ttu-id="8d392-175">string</span><span class="sxs-lookup"><span data-stu-id="8d392-175">string</span></span> | <span data-ttu-id="8d392-176">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="8d392-176">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="8d392-177">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="8d392-177">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="8d392-178">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="8d392-178">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="8d392-179">只读。</span><span class="sxs-lookup"><span data-stu-id="8d392-179">Read-only.</span></span> |
| <span data-ttu-id="8d392-180">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="8d392-180">latestSupportedTlsVersion</span></span> | <span data-ttu-id="8d392-181">字符串</span><span class="sxs-lookup"><span data-stu-id="8d392-181">String</span></span> | <span data-ttu-id="8d392-182">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="8d392-182">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="8d392-183">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="8d392-183">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="8d392-184">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="8d392-184">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="8d392-185">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="8d392-185">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="8d392-186">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="8d392-186">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="8d392-187">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="8d392-187">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="8d392-188">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="8d392-188">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="8d392-189">Resource</span><span class="sxs-lookup"><span data-stu-id="8d392-189">Resource</span></span>            | <span data-ttu-id="8d392-190">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="8d392-190">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="8d392-191">用户、组和其他目录资源</span><span class="sxs-lookup"><span data-stu-id="8d392-191">User, group, other directory resources</span></span>   | <span data-ttu-id="8d392-192">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-192">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8d392-193">邮件</span><span class="sxs-lookup"><span data-stu-id="8d392-193">Mail</span></span>                | <span data-ttu-id="8d392-194">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-194">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8d392-195">日历</span><span class="sxs-lookup"><span data-stu-id="8d392-195">Calendar</span></span>            | <span data-ttu-id="8d392-196">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8d392-197">联系人</span><span class="sxs-lookup"><span data-stu-id="8d392-197">Contacts</span></span>            | <span data-ttu-id="8d392-198">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8d392-199">组对话</span><span class="sxs-lookup"><span data-stu-id="8d392-199">Group conversations</span></span> | <span data-ttu-id="8d392-200">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8d392-201">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="8d392-201">Drive root items</span></span>    | <span data-ttu-id="8d392-202">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8d392-203">安全警报</span><span class="sxs-lookup"><span data-stu-id="8d392-203">Security alerts</span></span>     | <span data-ttu-id="8d392-204">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="8d392-204">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="8d392-205">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="8d392-205">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="8d392-206">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="8d392-206">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="8d392-207">关系</span><span class="sxs-lookup"><span data-stu-id="8d392-207">Relationships</span></span>

<span data-ttu-id="8d392-208">无</span><span class="sxs-lookup"><span data-stu-id="8d392-208">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d392-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d392-209">JSON representation</span></span>

<span data-ttu-id="8d392-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d392-210">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "latestSupportedTlsVersion": "string"
}
```

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
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
