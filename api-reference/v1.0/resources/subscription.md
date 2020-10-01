---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a82995a88b3dd5829b0f1f7c9b2cb5bcb5dfa18
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314655"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="f7b5f-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="f7b5f-104">subscription resource type</span></span>

<span data-ttu-id="f7b5f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7b5f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7b5f-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="f7b5f-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="f7b5f-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="f7b5f-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="f7b5f-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="f7b5f-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="f7b5f-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="f7b5f-110">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="f7b5f-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="f7b5f-111">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="f7b5f-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="f7b5f-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="f7b5f-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="f7b5f-113">SharePoint [网站][]下的[列表][] </span><span class="sxs-lookup"><span data-stu-id="f7b5f-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="f7b5f-114">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="f7b5f-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="f7b5f-115">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="f7b5f-115">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="f7b5f-116">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-116">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="f7b5f-117">方法</span><span class="sxs-lookup"><span data-stu-id="f7b5f-117">Methods</span></span>

| <span data-ttu-id="f7b5f-118">方法</span><span class="sxs-lookup"><span data-stu-id="f7b5f-118">Method</span></span> | <span data-ttu-id="f7b5f-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7b5f-119">Return Type</span></span> | <span data-ttu-id="f7b5f-120">说明</span><span class="sxs-lookup"><span data-stu-id="f7b5f-120">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="f7b5f-121">创建订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-121">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f7b5f-122">订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-122">subscription</span></span>](subscription.md) | <span data-ttu-id="f7b5f-123">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-123">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="f7b5f-124">更新订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-124">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="f7b5f-125">订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-125">subscription</span></span>](subscription.md) | <span data-ttu-id="f7b5f-126">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-126">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="f7b5f-127">列出订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-127">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="f7b5f-128">订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-128">subscription</span></span>](subscription.md) | <span data-ttu-id="f7b5f-129">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-129">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="f7b5f-130">获取订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-130">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="f7b5f-131">订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-131">subscription</span></span>](subscription.md) | <span data-ttu-id="f7b5f-132">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-132">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="f7b5f-133">删除订阅</span><span class="sxs-lookup"><span data-stu-id="f7b5f-133">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="f7b5f-134">无</span><span class="sxs-lookup"><span data-stu-id="f7b5f-134">None</span></span> | <span data-ttu-id="f7b5f-135">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-135">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7b5f-136">属性</span><span class="sxs-lookup"><span data-stu-id="f7b5f-136">Properties</span></span>

| <span data-ttu-id="f7b5f-137">属性</span><span class="sxs-lookup"><span data-stu-id="f7b5f-137">Property</span></span> | <span data-ttu-id="f7b5f-138">类型</span><span class="sxs-lookup"><span data-stu-id="f7b5f-138">Type</span></span> | <span data-ttu-id="f7b5f-139">说明</span><span class="sxs-lookup"><span data-stu-id="f7b5f-139">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f7b5f-140">changeType</span><span class="sxs-lookup"><span data-stu-id="f7b5f-140">changeType</span></span> | <span data-ttu-id="f7b5f-141">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-141">string</span></span> | <span data-ttu-id="f7b5f-142">必填。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-142">Required.</span></span> <span data-ttu-id="f7b5f-143">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="f7b5f-144">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f7b5f-145">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-145">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="f7b5f-146">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-146">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="f7b5f-147">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-147">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="f7b5f-148">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="f7b5f-148">notificationUrl</span></span> | <span data-ttu-id="f7b5f-149">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-149">string</span></span> | <span data-ttu-id="f7b5f-150">必填。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-150">Required.</span></span> <span data-ttu-id="f7b5f-151">将接收变更通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-151">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="f7b5f-152">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-152">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="f7b5f-153">resource</span><span class="sxs-lookup"><span data-stu-id="f7b5f-153">resource</span></span> | <span data-ttu-id="f7b5f-154">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-154">string</span></span> | <span data-ttu-id="f7b5f-155">必需。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-155">Required.</span></span> <span data-ttu-id="f7b5f-156">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-156">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="f7b5f-157">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-157">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="f7b5f-158">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-158">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="f7b5f-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f7b5f-159">expirationDateTime</span></span> | [<span data-ttu-id="f7b5f-160">dateTime</span><span class="sxs-lookup"><span data-stu-id="f7b5f-160">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="f7b5f-161">必需。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-161">Required.</span></span> <span data-ttu-id="f7b5f-162">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-162">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="f7b5f-163">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-163">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="f7b5f-164">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-164">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="f7b5f-165">clientState</span><span class="sxs-lookup"><span data-stu-id="f7b5f-165">clientState</span></span> | <span data-ttu-id="f7b5f-166">字符串</span><span class="sxs-lookup"><span data-stu-id="f7b5f-166">string</span></span> | <span data-ttu-id="f7b5f-167">可选。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-167">Optional.</span></span> <span data-ttu-id="f7b5f-168">指定服务为每个变更通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-168">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="f7b5f-169">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-169">The maximum length is 128 characters.</span></span> <span data-ttu-id="f7b5f-170">通过对比与订阅一起发送的 `clientState` 属性值和与每个变更通知一起接收的 `clientState` 属性值，客户端可以检查变更通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-170">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="f7b5f-171">id</span><span class="sxs-lookup"><span data-stu-id="f7b5f-171">id</span></span> | <span data-ttu-id="f7b5f-172">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-172">string</span></span> | <span data-ttu-id="f7b5f-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="f7b5f-175">applicationId</span><span class="sxs-lookup"><span data-stu-id="f7b5f-175">applicationId</span></span> | <span data-ttu-id="f7b5f-176">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-176">string</span></span> | <span data-ttu-id="f7b5f-177">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-177">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="f7b5f-178">只读。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-178">Read-only.</span></span> |
| <span data-ttu-id="f7b5f-179">creatorId</span><span class="sxs-lookup"><span data-stu-id="f7b5f-179">creatorId</span></span> | <span data-ttu-id="f7b5f-180">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-180">string</span></span> | <span data-ttu-id="f7b5f-181">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-181">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="f7b5f-182">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-182">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="f7b5f-183">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-183">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="f7b5f-184">只读。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-184">Read-only.</span></span> |
| <span data-ttu-id="f7b5f-185">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="f7b5f-185">includeResourceData</span></span> | <span data-ttu-id="f7b5f-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="f7b5f-186">Boolean</span></span> | <span data-ttu-id="f7b5f-187">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-187">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="f7b5f-188">可选。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-188">Optional.</span></span> | 
| <span data-ttu-id="f7b5f-189">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="f7b5f-189">encryptionCertificate</span></span> | <span data-ttu-id="f7b5f-190">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-190">string</span></span> | <span data-ttu-id="f7b5f-191">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-191">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="f7b5f-192">可选。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-192">Optional.</span></span> <span data-ttu-id="f7b5f-193">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-193">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="f7b5f-194">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="f7b5f-194">encryptionCertificateId</span></span> | <span data-ttu-id="f7b5f-195">string</span><span class="sxs-lookup"><span data-stu-id="f7b5f-195">string</span></span> | <span data-ttu-id="f7b5f-196">自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-196">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="f7b5f-197">可选。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-197">Optional.</span></span> 
| <span data-ttu-id="f7b5f-198">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="f7b5f-198">latestSupportedTlsVersion</span></span> | <span data-ttu-id="f7b5f-199">字符串</span><span class="sxs-lookup"><span data-stu-id="f7b5f-199">String</span></span> | <span data-ttu-id="f7b5f-200">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-200">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="f7b5f-201">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-201">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="f7b5f-202">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-202">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="f7b5f-203">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-203">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="f7b5f-204">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-204">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="f7b5f-205">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-205">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="f7b5f-206">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="f7b5f-206">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="f7b5f-207">Resource</span><span class="sxs-lookup"><span data-stu-id="f7b5f-207">Resource</span></span>            | <span data-ttu-id="f7b5f-208">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="f7b5f-208">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="f7b5f-209">安全**警报**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-209">Security **alert**</span></span>     | <span data-ttu-id="f7b5f-210">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-210">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="f7b5f-211">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-211">Teams **callRecord**</span></span>    | <span data-ttu-id="f7b5f-212">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-212">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="f7b5f-213">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-213">Teams **chatMessage**</span></span>    | <span data-ttu-id="f7b5f-214">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-214">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="f7b5f-215">组**对话**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-215">Group **conversation**</span></span> | <span data-ttu-id="f7b5f-216">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-216">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f7b5f-217">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-217">OneDrive **driveItem**</span></span>    | <span data-ttu-id="f7b5f-218">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-218">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f7b5f-219">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-219">SharePoint **list**</span></span>    | <span data-ttu-id="f7b5f-220">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-220">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f7b5f-221">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="f7b5f-221">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="f7b5f-222">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-222">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f7b5f-223">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="f7b5f-223">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="f7b5f-224">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f7b5f-224">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="f7b5f-225">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-225">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="f7b5f-226">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-226">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="f7b5f-227">关系</span><span class="sxs-lookup"><span data-stu-id="f7b5f-227">Relationships</span></span>

<span data-ttu-id="f7b5f-228">无</span><span class="sxs-lookup"><span data-stu-id="f7b5f-228">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7b5f-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7b5f-229">JSON representation</span></span>

<span data-ttu-id="f7b5f-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7b5f-230">Here is a JSON representation of the resource.</span></span>

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
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
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
[chatMessage]: ./chatmessage.md
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

