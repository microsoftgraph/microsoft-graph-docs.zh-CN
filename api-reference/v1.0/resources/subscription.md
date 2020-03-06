---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a490257ccc1ba17e7e425c24126c24689c612a9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533605"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="89d5d-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="89d5d-104">subscription resource type</span></span>

<span data-ttu-id="89d5d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d5d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89d5d-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="89d5d-106">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="89d5d-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="89d5d-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="89d5d-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="89d5d-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="89d5d-109">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="89d5d-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="89d5d-110">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="89d5d-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="89d5d-111">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="89d5d-111">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="89d5d-112">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="89d5d-112">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="89d5d-113">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="89d5d-113">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="89d5d-114">方法</span><span class="sxs-lookup"><span data-stu-id="89d5d-114">Methods</span></span>

| <span data-ttu-id="89d5d-115">方法</span><span class="sxs-lookup"><span data-stu-id="89d5d-115">Method</span></span> | <span data-ttu-id="89d5d-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="89d5d-116">Return Type</span></span> | <span data-ttu-id="89d5d-117">说明</span><span class="sxs-lookup"><span data-stu-id="89d5d-117">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="89d5d-118">创建订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-118">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="89d5d-119">订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-119">subscription</span></span>](subscription.md) | <span data-ttu-id="89d5d-120">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="89d5d-120">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="89d5d-121">更新订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-121">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="89d5d-122">订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-122">subscription</span></span>](subscription.md) | <span data-ttu-id="89d5d-123">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="89d5d-123">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="89d5d-124">列出订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-124">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="89d5d-125">订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-125">subscription</span></span>](subscription.md) | <span data-ttu-id="89d5d-126">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="89d5d-126">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="89d5d-127">获取订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-127">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="89d5d-128">订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-128">subscription</span></span>](subscription.md) | <span data-ttu-id="89d5d-129">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89d5d-129">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="89d5d-130">删除订阅</span><span class="sxs-lookup"><span data-stu-id="89d5d-130">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="89d5d-131">无</span><span class="sxs-lookup"><span data-stu-id="89d5d-131">None</span></span> | <span data-ttu-id="89d5d-132">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="89d5d-132">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="89d5d-133">属性</span><span class="sxs-lookup"><span data-stu-id="89d5d-133">Properties</span></span>

| <span data-ttu-id="89d5d-134">属性</span><span class="sxs-lookup"><span data-stu-id="89d5d-134">Property</span></span> | <span data-ttu-id="89d5d-135">类型</span><span class="sxs-lookup"><span data-stu-id="89d5d-135">Type</span></span> | <span data-ttu-id="89d5d-136">说明</span><span class="sxs-lookup"><span data-stu-id="89d5d-136">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="89d5d-137">changeType</span><span class="sxs-lookup"><span data-stu-id="89d5d-137">changeType</span></span> | <span data-ttu-id="89d5d-138">string</span><span class="sxs-lookup"><span data-stu-id="89d5d-138">string</span></span> | <span data-ttu-id="89d5d-139">必需。</span><span class="sxs-lookup"><span data-stu-id="89d5d-139">Required.</span></span> <span data-ttu-id="89d5d-140">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="89d5d-140">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="89d5d-141">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="89d5d-141">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="89d5d-142">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="89d5d-142">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="89d5d-143">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="89d5d-143">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="89d5d-144">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="89d5d-144">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="89d5d-145">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="89d5d-145">notificationUrl</span></span> | <span data-ttu-id="89d5d-146">string</span><span class="sxs-lookup"><span data-stu-id="89d5d-146">string</span></span> | <span data-ttu-id="89d5d-147">必需。</span><span class="sxs-lookup"><span data-stu-id="89d5d-147">Required.</span></span> <span data-ttu-id="89d5d-148">将接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="89d5d-148">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="89d5d-149">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="89d5d-149">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="89d5d-150">resource</span><span class="sxs-lookup"><span data-stu-id="89d5d-150">resource</span></span> | <span data-ttu-id="89d5d-151">string</span><span class="sxs-lookup"><span data-stu-id="89d5d-151">string</span></span> | <span data-ttu-id="89d5d-152">必需。</span><span class="sxs-lookup"><span data-stu-id="89d5d-152">Required.</span></span> <span data-ttu-id="89d5d-153">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="89d5d-153">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="89d5d-154">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="89d5d-154">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="89d5d-155">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="89d5d-155">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="89d5d-156">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="89d5d-156">expirationDateTime</span></span> | [<span data-ttu-id="89d5d-157">dateTime</span><span class="sxs-lookup"><span data-stu-id="89d5d-157">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="89d5d-158">必需。</span><span class="sxs-lookup"><span data-stu-id="89d5d-158">Required.</span></span> <span data-ttu-id="89d5d-159">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="89d5d-159">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="89d5d-160">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="89d5d-160">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="89d5d-161">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="89d5d-161">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="89d5d-162">clientState</span><span class="sxs-lookup"><span data-stu-id="89d5d-162">clientState</span></span> | <span data-ttu-id="89d5d-163">字符串</span><span class="sxs-lookup"><span data-stu-id="89d5d-163">string</span></span> | <span data-ttu-id="89d5d-164">可选。</span><span class="sxs-lookup"><span data-stu-id="89d5d-164">Optional.</span></span> <span data-ttu-id="89d5d-165">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="89d5d-165">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="89d5d-166">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="89d5d-166">The maximum length is 128 characters.</span></span> <span data-ttu-id="89d5d-167">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="89d5d-167">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="89d5d-168">id</span><span class="sxs-lookup"><span data-stu-id="89d5d-168">id</span></span> | <span data-ttu-id="89d5d-169">string</span><span class="sxs-lookup"><span data-stu-id="89d5d-169">string</span></span> | <span data-ttu-id="89d5d-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="89d5d-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="89d5d-172">applicationId</span><span class="sxs-lookup"><span data-stu-id="89d5d-172">applicationId</span></span> | <span data-ttu-id="89d5d-173">string</span><span class="sxs-lookup"><span data-stu-id="89d5d-173">string</span></span> | <span data-ttu-id="89d5d-174">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="89d5d-174">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="89d5d-175">只读。</span><span class="sxs-lookup"><span data-stu-id="89d5d-175">Read-only.</span></span> |
| <span data-ttu-id="89d5d-176">creatorId</span><span class="sxs-lookup"><span data-stu-id="89d5d-176">creatorId</span></span> | <span data-ttu-id="89d5d-177">string</span><span class="sxs-lookup"><span data-stu-id="89d5d-177">string</span></span> | <span data-ttu-id="89d5d-178">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="89d5d-178">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="89d5d-179">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="89d5d-179">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="89d5d-180">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="89d5d-180">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="89d5d-181">只读。</span><span class="sxs-lookup"><span data-stu-id="89d5d-181">Read-only.</span></span> |
| <span data-ttu-id="89d5d-182">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="89d5d-182">latestSupportedTlsVersion</span></span> | <span data-ttu-id="89d5d-183">字符串</span><span class="sxs-lookup"><span data-stu-id="89d5d-183">String</span></span> | <span data-ttu-id="89d5d-184">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="89d5d-184">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="89d5d-185">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="89d5d-185">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="89d5d-186">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="89d5d-186">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="89d5d-187">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="89d5d-187">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="89d5d-188">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="89d5d-188">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="89d5d-189">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="89d5d-189">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="89d5d-190">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="89d5d-190">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="89d5d-191">Resource</span><span class="sxs-lookup"><span data-stu-id="89d5d-191">Resource</span></span>            | <span data-ttu-id="89d5d-192">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="89d5d-192">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="89d5d-193">用户、组和其他目录资源</span><span class="sxs-lookup"><span data-stu-id="89d5d-193">User, group, other directory resources</span></span>   | <span data-ttu-id="89d5d-194">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-194">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="89d5d-195">邮件</span><span class="sxs-lookup"><span data-stu-id="89d5d-195">Mail</span></span>                | <span data-ttu-id="89d5d-196">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="89d5d-197">日历</span><span class="sxs-lookup"><span data-stu-id="89d5d-197">Calendar</span></span>            | <span data-ttu-id="89d5d-198">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="89d5d-199">联系人</span><span class="sxs-lookup"><span data-stu-id="89d5d-199">Contacts</span></span>            | <span data-ttu-id="89d5d-200">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="89d5d-201">组对话</span><span class="sxs-lookup"><span data-stu-id="89d5d-201">Group conversations</span></span> | <span data-ttu-id="89d5d-202">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="89d5d-203">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="89d5d-203">Drive root items</span></span>    | <span data-ttu-id="89d5d-204">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-204">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="89d5d-205">安全警报</span><span class="sxs-lookup"><span data-stu-id="89d5d-205">Security alerts</span></span>     | <span data-ttu-id="89d5d-206">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="89d5d-206">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="89d5d-207">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="89d5d-207">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="89d5d-208">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="89d5d-208">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="89d5d-209">关系</span><span class="sxs-lookup"><span data-stu-id="89d5d-209">Relationships</span></span>

<span data-ttu-id="89d5d-210">无</span><span class="sxs-lookup"><span data-stu-id="89d5d-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89d5d-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89d5d-211">JSON representation</span></span>

<span data-ttu-id="89d5d-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d5d-212">Here is a JSON representation of the resource.</span></span>

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
