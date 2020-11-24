---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68ef4c0275ad06ae2e2635044ab3792241dafaae
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742069"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="a6d6c-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="a6d6c-104">subscription resource type</span></span>

<span data-ttu-id="a6d6c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6d6c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6d6c-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="a6d6c-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="a6d6c-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="a6d6c-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="a6d6c-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="a6d6c-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="a6d6c-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="a6d6c-110">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="a6d6c-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="a6d6c-111">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="a6d6c-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="a6d6c-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="a6d6c-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="a6d6c-113">SharePoint [site][]下的[list][] </span><span class="sxs-lookup"><span data-stu-id="a6d6c-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="a6d6c-114">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="a6d6c-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="a6d6c-115">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="a6d6c-115">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="a6d6c-116">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-116">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="a6d6c-117">方法</span><span class="sxs-lookup"><span data-stu-id="a6d6c-117">Methods</span></span>

| <span data-ttu-id="a6d6c-118">方法</span><span class="sxs-lookup"><span data-stu-id="a6d6c-118">Method</span></span> | <span data-ttu-id="a6d6c-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6d6c-119">Return Type</span></span> | <span data-ttu-id="a6d6c-120">说明</span><span class="sxs-lookup"><span data-stu-id="a6d6c-120">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="a6d6c-121">创建订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-121">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="a6d6c-122">订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-122">subscription</span></span>](subscription.md) | <span data-ttu-id="a6d6c-123">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-123">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="a6d6c-124">更新订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-124">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="a6d6c-125">订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-125">subscription</span></span>](subscription.md) | <span data-ttu-id="a6d6c-126">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-126">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="a6d6c-127">列出订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-127">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="a6d6c-128">订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-128">subscription</span></span>](subscription.md) | <span data-ttu-id="a6d6c-129">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-129">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="a6d6c-130">获取订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-130">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="a6d6c-131">订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-131">subscription</span></span>](subscription.md) | <span data-ttu-id="a6d6c-132">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-132">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="a6d6c-133">删除订阅</span><span class="sxs-lookup"><span data-stu-id="a6d6c-133">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="a6d6c-134">无</span><span class="sxs-lookup"><span data-stu-id="a6d6c-134">None</span></span> | <span data-ttu-id="a6d6c-135">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-135">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a6d6c-136">属性</span><span class="sxs-lookup"><span data-stu-id="a6d6c-136">Properties</span></span>

| <span data-ttu-id="a6d6c-137">属性</span><span class="sxs-lookup"><span data-stu-id="a6d6c-137">Property</span></span> | <span data-ttu-id="a6d6c-138">类型</span><span class="sxs-lookup"><span data-stu-id="a6d6c-138">Type</span></span> | <span data-ttu-id="a6d6c-139">说明</span><span class="sxs-lookup"><span data-stu-id="a6d6c-139">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a6d6c-140">changeType</span><span class="sxs-lookup"><span data-stu-id="a6d6c-140">changeType</span></span> | <span data-ttu-id="a6d6c-141">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-141">string</span></span> | <span data-ttu-id="a6d6c-142">必填。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-142">Required.</span></span> <span data-ttu-id="a6d6c-143">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="a6d6c-144">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="a6d6c-145">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-145">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="a6d6c-146">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-146">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="a6d6c-147">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-147">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="a6d6c-148">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="a6d6c-148">notificationUrl</span></span> | <span data-ttu-id="a6d6c-149">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-149">string</span></span> | <span data-ttu-id="a6d6c-150">必填。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-150">Required.</span></span> <span data-ttu-id="a6d6c-151">将接收变更通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-151">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="a6d6c-152">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-152">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="a6d6c-153">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="a6d6c-153">lifecycleNotificationUrl</span></span> | <span data-ttu-id="a6d6c-154">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-154">string</span></span> | <span data-ttu-id="a6d6c-155">接收生命周期通知（包括 `subscriptionRemoved` 和 `missed` 通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-155">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="a6d6c-156">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-156">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="a6d6c-157">可选。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-157">Optional.</span></span> <br><br><span data-ttu-id="a6d6c-158">[阅读](/graph/webhooks-lifecycle)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-158">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="a6d6c-159">resource</span><span class="sxs-lookup"><span data-stu-id="a6d6c-159">resource</span></span> | <span data-ttu-id="a6d6c-160">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-160">string</span></span> | <span data-ttu-id="a6d6c-161">必填。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-161">Required.</span></span> <span data-ttu-id="a6d6c-162">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-162">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="a6d6c-163">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-163">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="a6d6c-164">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-164">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="a6d6c-165">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a6d6c-165">expirationDateTime</span></span> | [<span data-ttu-id="a6d6c-166">dateTime</span><span class="sxs-lookup"><span data-stu-id="a6d6c-166">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="a6d6c-167">必填。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-167">Required.</span></span> <span data-ttu-id="a6d6c-168">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-168">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="a6d6c-169">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-169">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="a6d6c-170">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-170">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="a6d6c-171">clientState</span><span class="sxs-lookup"><span data-stu-id="a6d6c-171">clientState</span></span> | <span data-ttu-id="a6d6c-172">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-172">string</span></span> | <span data-ttu-id="a6d6c-173">可选。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-173">Optional.</span></span> <span data-ttu-id="a6d6c-174">指定服务为每个变更通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-174">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="a6d6c-175">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-175">The maximum length is 128 characters.</span></span> <span data-ttu-id="a6d6c-176">通过对比与订阅一起发送的 `clientState` 属性值和与每个变更通知一起接收的 `clientState` 属性值，客户端可以检查变更通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-176">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="a6d6c-177">id</span><span class="sxs-lookup"><span data-stu-id="a6d6c-177">id</span></span> | <span data-ttu-id="a6d6c-178">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-178">string</span></span> | <span data-ttu-id="a6d6c-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="a6d6c-181">applicationId</span><span class="sxs-lookup"><span data-stu-id="a6d6c-181">applicationId</span></span> | <span data-ttu-id="a6d6c-182">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-182">string</span></span> | <span data-ttu-id="a6d6c-183">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-183">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="a6d6c-184">只读。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-184">Read-only.</span></span> |
| <span data-ttu-id="a6d6c-185">creatorId</span><span class="sxs-lookup"><span data-stu-id="a6d6c-185">creatorId</span></span> | <span data-ttu-id="a6d6c-186">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-186">string</span></span> | <span data-ttu-id="a6d6c-187">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-187">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="a6d6c-188">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-188">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="a6d6c-189">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-189">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="a6d6c-190">只读。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-190">Read-only.</span></span> |
| <span data-ttu-id="a6d6c-191">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="a6d6c-191">includeResourceData</span></span> | <span data-ttu-id="a6d6c-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="a6d6c-192">Boolean</span></span> | <span data-ttu-id="a6d6c-193">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-193">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="a6d6c-194">可选。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-194">Optional.</span></span> | 
| <span data-ttu-id="a6d6c-195">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="a6d6c-195">encryptionCertificate</span></span> | <span data-ttu-id="a6d6c-196">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-196">string</span></span> | <span data-ttu-id="a6d6c-197">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-197">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="a6d6c-198">可选。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-198">Optional.</span></span> <span data-ttu-id="a6d6c-199">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-199">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="a6d6c-200">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="a6d6c-200">encryptionCertificateId</span></span> | <span data-ttu-id="a6d6c-201">string</span><span class="sxs-lookup"><span data-stu-id="a6d6c-201">string</span></span> | <span data-ttu-id="a6d6c-202">自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-202">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="a6d6c-203">可选。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-203">Optional.</span></span> 
| <span data-ttu-id="a6d6c-204">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="a6d6c-204">latestSupportedTlsVersion</span></span> | <span data-ttu-id="a6d6c-205">字符串</span><span class="sxs-lookup"><span data-stu-id="a6d6c-205">String</span></span> | <span data-ttu-id="a6d6c-206">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-206">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="a6d6c-207">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-207">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="a6d6c-208">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-208">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="a6d6c-209">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-209">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="a6d6c-210">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-210">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="a6d6c-211">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-211">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="a6d6c-212">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="a6d6c-212">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="a6d6c-213">Resource</span><span class="sxs-lookup"><span data-stu-id="a6d6c-213">Resource</span></span>            | <span data-ttu-id="a6d6c-214">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="a6d6c-214">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="a6d6c-215">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-215">Security **alert**</span></span>     | <span data-ttu-id="a6d6c-216">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-216">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="a6d6c-217">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-217">Teams **callRecord**</span></span>    | <span data-ttu-id="a6d6c-218">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-218">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="a6d6c-219">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-219">Teams **chatMessage**</span></span>    | <span data-ttu-id="a6d6c-220">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-220">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="a6d6c-221">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-221">Group **conversation**</span></span> | <span data-ttu-id="a6d6c-222">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-222">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="a6d6c-223">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-223">OneDrive **driveItem**</span></span>    | <span data-ttu-id="a6d6c-224">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-224">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="a6d6c-225">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-225">SharePoint **list**</span></span>    | <span data-ttu-id="a6d6c-226">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-226">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="a6d6c-227">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="a6d6c-227">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="a6d6c-228">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-228">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="a6d6c-229">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="a6d6c-229">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="a6d6c-230">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="a6d6c-230">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="a6d6c-231">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-231">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="a6d6c-232">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-232">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="a6d6c-233">关系</span><span class="sxs-lookup"><span data-stu-id="a6d6c-233">Relationships</span></span>

<span data-ttu-id="a6d6c-234">无</span><span class="sxs-lookup"><span data-stu-id="a6d6c-234">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6d6c-235">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6d6c-235">JSON representation</span></span>

<span data-ttu-id="a6d6c-236">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6d6c-236">Here is a JSON representation of the resource.</span></span>

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
  "lifecycleNotificationUrl": "string",
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

