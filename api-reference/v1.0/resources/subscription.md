---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7f6c933b2cdc306941e391dc486fd607616b196a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094132"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="f1a81-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="f1a81-104">subscription resource type</span></span>

<span data-ttu-id="f1a81-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a81-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1a81-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="f1a81-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="f1a81-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="f1a81-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="f1a81-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="f1a81-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="f1a81-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="f1a81-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="f1a81-110">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="f1a81-110">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="f1a81-111">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="f1a81-111">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="f1a81-112">SharePoint [网站][]下的[列表][] </span><span class="sxs-lookup"><span data-stu-id="f1a81-112">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="f1a81-113">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="f1a81-113">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="f1a81-114">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="f1a81-114">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="f1a81-115">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="f1a81-115">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="f1a81-116">方法</span><span class="sxs-lookup"><span data-stu-id="f1a81-116">Methods</span></span>

| <span data-ttu-id="f1a81-117">方法</span><span class="sxs-lookup"><span data-stu-id="f1a81-117">Method</span></span> | <span data-ttu-id="f1a81-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1a81-118">Return Type</span></span> | <span data-ttu-id="f1a81-119">说明</span><span class="sxs-lookup"><span data-stu-id="f1a81-119">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="f1a81-120">创建订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-120">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f1a81-121">订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-121">subscription</span></span>](subscription.md) | <span data-ttu-id="f1a81-122">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="f1a81-122">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="f1a81-123">更新订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-123">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="f1a81-124">订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-124">subscription</span></span>](subscription.md) | <span data-ttu-id="f1a81-125">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="f1a81-125">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="f1a81-126">列出订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-126">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="f1a81-127">订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-127">subscription</span></span>](subscription.md) | <span data-ttu-id="f1a81-128">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="f1a81-128">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="f1a81-129">获取订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-129">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="f1a81-130">订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-130">subscription</span></span>](subscription.md) | <span data-ttu-id="f1a81-131">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1a81-131">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="f1a81-132">删除订阅</span><span class="sxs-lookup"><span data-stu-id="f1a81-132">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="f1a81-133">无</span><span class="sxs-lookup"><span data-stu-id="f1a81-133">None</span></span> | <span data-ttu-id="f1a81-134">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="f1a81-134">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f1a81-135">属性</span><span class="sxs-lookup"><span data-stu-id="f1a81-135">Properties</span></span>

| <span data-ttu-id="f1a81-136">属性</span><span class="sxs-lookup"><span data-stu-id="f1a81-136">Property</span></span> | <span data-ttu-id="f1a81-137">类型</span><span class="sxs-lookup"><span data-stu-id="f1a81-137">Type</span></span> | <span data-ttu-id="f1a81-138">说明</span><span class="sxs-lookup"><span data-stu-id="f1a81-138">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f1a81-139">changeType</span><span class="sxs-lookup"><span data-stu-id="f1a81-139">changeType</span></span> | <span data-ttu-id="f1a81-140">string</span><span class="sxs-lookup"><span data-stu-id="f1a81-140">string</span></span> | <span data-ttu-id="f1a81-141">必填。</span><span class="sxs-lookup"><span data-stu-id="f1a81-141">Required.</span></span> <span data-ttu-id="f1a81-142">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="f1a81-142">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="f1a81-143">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="f1a81-143">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f1a81-144">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="f1a81-144">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="f1a81-145">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="f1a81-145">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="f1a81-146">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="f1a81-146">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="f1a81-147">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="f1a81-147">notificationUrl</span></span> | <span data-ttu-id="f1a81-148">string</span><span class="sxs-lookup"><span data-stu-id="f1a81-148">string</span></span> | <span data-ttu-id="f1a81-149">必填。</span><span class="sxs-lookup"><span data-stu-id="f1a81-149">Required.</span></span> <span data-ttu-id="f1a81-150">将接收变更通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="f1a81-150">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="f1a81-151">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="f1a81-151">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="f1a81-152">resource</span><span class="sxs-lookup"><span data-stu-id="f1a81-152">resource</span></span> | <span data-ttu-id="f1a81-153">string</span><span class="sxs-lookup"><span data-stu-id="f1a81-153">string</span></span> | <span data-ttu-id="f1a81-154">必需。</span><span class="sxs-lookup"><span data-stu-id="f1a81-154">Required.</span></span> <span data-ttu-id="f1a81-155">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="f1a81-155">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="f1a81-156">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="f1a81-156">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="f1a81-157">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="f1a81-157">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="f1a81-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a81-158">expirationDateTime</span></span> | [<span data-ttu-id="f1a81-159">dateTime</span><span class="sxs-lookup"><span data-stu-id="f1a81-159">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="f1a81-160">必需。</span><span class="sxs-lookup"><span data-stu-id="f1a81-160">Required.</span></span> <span data-ttu-id="f1a81-161">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f1a81-161">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="f1a81-162">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="f1a81-162">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="f1a81-163">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="f1a81-163">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="f1a81-164">clientState</span><span class="sxs-lookup"><span data-stu-id="f1a81-164">clientState</span></span> | <span data-ttu-id="f1a81-165">字符串</span><span class="sxs-lookup"><span data-stu-id="f1a81-165">string</span></span> | <span data-ttu-id="f1a81-166">可选。</span><span class="sxs-lookup"><span data-stu-id="f1a81-166">Optional.</span></span> <span data-ttu-id="f1a81-167">指定服务为每个变更通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="f1a81-167">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="f1a81-168">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="f1a81-168">The maximum length is 128 characters.</span></span> <span data-ttu-id="f1a81-169">通过对比与订阅一起发送的 `clientState` 属性值和与每个变更通知一起接收的 `clientState` 属性值，客户端可以检查变更通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="f1a81-169">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="f1a81-170">id</span><span class="sxs-lookup"><span data-stu-id="f1a81-170">id</span></span> | <span data-ttu-id="f1a81-171">string</span><span class="sxs-lookup"><span data-stu-id="f1a81-171">string</span></span> | <span data-ttu-id="f1a81-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f1a81-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="f1a81-174">applicationId</span><span class="sxs-lookup"><span data-stu-id="f1a81-174">applicationId</span></span> | <span data-ttu-id="f1a81-175">string</span><span class="sxs-lookup"><span data-stu-id="f1a81-175">string</span></span> | <span data-ttu-id="f1a81-176">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="f1a81-176">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="f1a81-177">只读。</span><span class="sxs-lookup"><span data-stu-id="f1a81-177">Read-only.</span></span> |
| <span data-ttu-id="f1a81-178">creatorId</span><span class="sxs-lookup"><span data-stu-id="f1a81-178">creatorId</span></span> | <span data-ttu-id="f1a81-179">string</span><span class="sxs-lookup"><span data-stu-id="f1a81-179">string</span></span> | <span data-ttu-id="f1a81-180">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="f1a81-180">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="f1a81-181">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="f1a81-181">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="f1a81-182">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="f1a81-182">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="f1a81-183">只读。</span><span class="sxs-lookup"><span data-stu-id="f1a81-183">Read-only.</span></span> |
| <span data-ttu-id="f1a81-184">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="f1a81-184">latestSupportedTlsVersion</span></span> | <span data-ttu-id="f1a81-185">字符串</span><span class="sxs-lookup"><span data-stu-id="f1a81-185">String</span></span> | <span data-ttu-id="f1a81-186">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="f1a81-186">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="f1a81-187">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="f1a81-187">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="f1a81-188">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="f1a81-188">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="f1a81-189">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="f1a81-189">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="f1a81-190">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="f1a81-190">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="f1a81-191">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="f1a81-191">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="f1a81-192">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="f1a81-192">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="f1a81-193">Resource</span><span class="sxs-lookup"><span data-stu-id="f1a81-193">Resource</span></span>            | <span data-ttu-id="f1a81-194">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="f1a81-194">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="f1a81-195">用户、组和其他目录资源</span><span class="sxs-lookup"><span data-stu-id="f1a81-195">User, group, other directory resources</span></span>   | <span data-ttu-id="f1a81-196">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-197">邮件</span><span class="sxs-lookup"><span data-stu-id="f1a81-197">Mail</span></span>                | <span data-ttu-id="f1a81-198">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-199">日历</span><span class="sxs-lookup"><span data-stu-id="f1a81-199">Calendar</span></span>            | <span data-ttu-id="f1a81-200">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-201">联系人</span><span class="sxs-lookup"><span data-stu-id="f1a81-201">Contacts</span></span>            | <span data-ttu-id="f1a81-202">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-203">组对话</span><span class="sxs-lookup"><span data-stu-id="f1a81-203">Group conversations</span></span> | <span data-ttu-id="f1a81-204">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-204">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-205">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="f1a81-205">Drive root items</span></span>    | <span data-ttu-id="f1a81-206">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-206">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-207">SharePoint 列表</span><span class="sxs-lookup"><span data-stu-id="f1a81-207">SharePoint list</span></span>     | <span data-ttu-id="f1a81-208">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-208">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f1a81-209">Teams callRecord</span><span class="sxs-lookup"><span data-stu-id="f1a81-209">Teams callRecord</span></span>    | <span data-ttu-id="f1a81-210">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-210">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="f1a81-211">安全警报</span><span class="sxs-lookup"><span data-stu-id="f1a81-211">Security alerts</span></span>     | <span data-ttu-id="f1a81-212">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="f1a81-212">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="f1a81-213">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="f1a81-213">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="f1a81-214">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="f1a81-214">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="f1a81-215">关系</span><span class="sxs-lookup"><span data-stu-id="f1a81-215">Relationships</span></span>

<span data-ttu-id="f1a81-216">无</span><span class="sxs-lookup"><span data-stu-id="f1a81-216">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1a81-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1a81-217">JSON representation</span></span>

<span data-ttu-id="f1a81-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1a81-218">Here is a JSON representation of the resource.</span></span>

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
[list]: ./list.md
[site]: ./site.md
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
[callRecord]: ./callrecords-callrecord.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

