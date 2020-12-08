---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f675f8648b15f36517c1880f7bdb0c3178ef6b67
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597412"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="969ed-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="969ed-104">subscription resource type</span></span>

<span data-ttu-id="969ed-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="969ed-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="969ed-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="969ed-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="969ed-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="969ed-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="969ed-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="969ed-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="969ed-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="969ed-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="969ed-110">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="969ed-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="969ed-111">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="969ed-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="969ed-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="969ed-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="969ed-113">SharePoint [网站][]下的[列表][] </span><span class="sxs-lookup"><span data-stu-id="969ed-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="969ed-114">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="969ed-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="969ed-115">Microsoft 团队中的用户[是否存在][]</span><span class="sxs-lookup"><span data-stu-id="969ed-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="969ed-116">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="969ed-116">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="969ed-117">打印服务中的[printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="969ed-117">A [printTaskDefinition][] in Print Service</span></span>
- <span data-ttu-id="969ed-118">Microsoft 中用户的[todoTask]</span><span class="sxs-lookup"><span data-stu-id="969ed-118">A [todoTask] of a user in Microsoft To Do</span></span>

<span data-ttu-id="969ed-119">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="969ed-119">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="969ed-120">方法</span><span class="sxs-lookup"><span data-stu-id="969ed-120">Methods</span></span>

| <span data-ttu-id="969ed-121">方法</span><span class="sxs-lookup"><span data-stu-id="969ed-121">Method</span></span> | <span data-ttu-id="969ed-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="969ed-122">Return Type</span></span> | <span data-ttu-id="969ed-123">说明</span><span class="sxs-lookup"><span data-stu-id="969ed-123">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="969ed-124">创建订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-124">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="969ed-125">订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-125">subscription</span></span>](subscription.md) | <span data-ttu-id="969ed-126">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="969ed-126">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="969ed-127">更新订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-127">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="969ed-128">订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-128">subscription</span></span>](subscription.md) | <span data-ttu-id="969ed-129">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="969ed-129">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="969ed-130">列出订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-130">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="969ed-131">订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-131">subscription</span></span>](subscription.md) | <span data-ttu-id="969ed-132">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="969ed-132">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="969ed-133">获取订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-133">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="969ed-134">订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-134">subscription</span></span>](subscription.md) | <span data-ttu-id="969ed-135">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="969ed-135">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="969ed-136">删除订阅</span><span class="sxs-lookup"><span data-stu-id="969ed-136">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="969ed-137">无</span><span class="sxs-lookup"><span data-stu-id="969ed-137">None</span></span> | <span data-ttu-id="969ed-138">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="969ed-138">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="969ed-139">属性</span><span class="sxs-lookup"><span data-stu-id="969ed-139">Properties</span></span>

| <span data-ttu-id="969ed-140">属性</span><span class="sxs-lookup"><span data-stu-id="969ed-140">Property</span></span> | <span data-ttu-id="969ed-141">类型</span><span class="sxs-lookup"><span data-stu-id="969ed-141">Type</span></span> | <span data-ttu-id="969ed-142">说明</span><span class="sxs-lookup"><span data-stu-id="969ed-142">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="969ed-143">changeType</span><span class="sxs-lookup"><span data-stu-id="969ed-143">changeType</span></span> | <span data-ttu-id="969ed-144">string</span><span class="sxs-lookup"><span data-stu-id="969ed-144">string</span></span> | <span data-ttu-id="969ed-145">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="969ed-145">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="969ed-146">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="969ed-146">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="969ed-147">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="969ed-147">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="969ed-148">必需。</span><span class="sxs-lookup"><span data-stu-id="969ed-148">Required.</span></span> <br><br><span data-ttu-id="969ed-149">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="969ed-149">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="969ed-150">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="969ed-150">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="969ed-151">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="969ed-151">notificationUrl</span></span> | <span data-ttu-id="969ed-152">string</span><span class="sxs-lookup"><span data-stu-id="969ed-152">string</span></span> | <span data-ttu-id="969ed-153">接收更改通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="969ed-153">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="969ed-154">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="969ed-154">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="969ed-155">必需。</span><span class="sxs-lookup"><span data-stu-id="969ed-155">Required.</span></span> |
| <span data-ttu-id="969ed-156">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="969ed-156">lifecycleNotificationUrl</span></span> | <span data-ttu-id="969ed-157">string</span><span class="sxs-lookup"><span data-stu-id="969ed-157">string</span></span> | <span data-ttu-id="969ed-158">接收生命周期通知（包括和通知）的终结点的 URL `subscriptionRemoved` `missed` 。</span><span class="sxs-lookup"><span data-stu-id="969ed-158">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="969ed-159">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="969ed-159">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="969ed-160">可选。</span><span class="sxs-lookup"><span data-stu-id="969ed-160">Optional.</span></span> <br><br><span data-ttu-id="969ed-161">[阅读](/graph/webhooks-lifecycle) 有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="969ed-161">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="969ed-162">resource</span><span class="sxs-lookup"><span data-stu-id="969ed-162">resource</span></span> | <span data-ttu-id="969ed-163">string</span><span class="sxs-lookup"><span data-stu-id="969ed-163">string</span></span> | <span data-ttu-id="969ed-164">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="969ed-164">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="969ed-165">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="969ed-165">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="969ed-166">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="969ed-166">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="969ed-167">必需。</span><span class="sxs-lookup"><span data-stu-id="969ed-167">Required.</span></span> |
| <span data-ttu-id="969ed-168">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="969ed-168">expirationDateTime</span></span> | <span data-ttu-id="969ed-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969ed-169">DateTimeOffset</span></span> | <span data-ttu-id="969ed-170">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="969ed-170">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="969ed-171">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="969ed-171">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="969ed-172">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="969ed-172">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="969ed-173">必需。</span><span class="sxs-lookup"><span data-stu-id="969ed-173">Required.</span></span> |
| <span data-ttu-id="969ed-174">clientState</span><span class="sxs-lookup"><span data-stu-id="969ed-174">clientState</span></span> | <span data-ttu-id="969ed-175">string</span><span class="sxs-lookup"><span data-stu-id="969ed-175">string</span></span> | <span data-ttu-id="969ed-176">指定在每次更改通知中由服务发送的 **clientState** 属性的值。</span><span class="sxs-lookup"><span data-stu-id="969ed-176">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="969ed-177">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="969ed-177">The maximum length is 255 characters.</span></span> <span data-ttu-id="969ed-178">客户端可以通过将随订阅发送的 **clientState** 属性的值与每个更改通知接收的 **clientState** 属性的值进行比较，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="969ed-178">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="969ed-179">可选。</span><span class="sxs-lookup"><span data-stu-id="969ed-179">Optional.</span></span> |
| <span data-ttu-id="969ed-180">id</span><span class="sxs-lookup"><span data-stu-id="969ed-180">id</span></span> | <span data-ttu-id="969ed-181">string</span><span class="sxs-lookup"><span data-stu-id="969ed-181">string</span></span> | <span data-ttu-id="969ed-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="969ed-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="969ed-184">applicationId</span><span class="sxs-lookup"><span data-stu-id="969ed-184">applicationId</span></span> | <span data-ttu-id="969ed-185">string</span><span class="sxs-lookup"><span data-stu-id="969ed-185">string</span></span> | <span data-ttu-id="969ed-186">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="969ed-186">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="969ed-187">只读。</span><span class="sxs-lookup"><span data-stu-id="969ed-187">Read-only.</span></span> |
| <span data-ttu-id="969ed-188">creatorId</span><span class="sxs-lookup"><span data-stu-id="969ed-188">creatorId</span></span> | <span data-ttu-id="969ed-189">string</span><span class="sxs-lookup"><span data-stu-id="969ed-189">string</span></span> | <span data-ttu-id="969ed-190">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="969ed-190">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="969ed-191">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="969ed-191">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="969ed-192">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="969ed-192">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="969ed-193">只读。</span><span class="sxs-lookup"><span data-stu-id="969ed-193">Read-only.</span></span> |
| <span data-ttu-id="969ed-194">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="969ed-194">includeResourceData</span></span> | <span data-ttu-id="969ed-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="969ed-195">Boolean</span></span> | <span data-ttu-id="969ed-196">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="969ed-196">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="969ed-197">可选。</span><span class="sxs-lookup"><span data-stu-id="969ed-197">Optional.</span></span> | 
| <span data-ttu-id="969ed-198">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="969ed-198">encryptionCertificate</span></span> | <span data-ttu-id="969ed-199">string</span><span class="sxs-lookup"><span data-stu-id="969ed-199">string</span></span> | <span data-ttu-id="969ed-200">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="969ed-200">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="969ed-201">可选。</span><span class="sxs-lookup"><span data-stu-id="969ed-201">Optional.</span></span> <span data-ttu-id="969ed-202">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="969ed-202">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="969ed-203">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="969ed-203">encryptionCertificateId</span></span> | <span data-ttu-id="969ed-204">string</span><span class="sxs-lookup"><span data-stu-id="969ed-204">string</span></span> | <span data-ttu-id="969ed-205">自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="969ed-205">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="969ed-206">可选。</span><span class="sxs-lookup"><span data-stu-id="969ed-206">Optional.</span></span> <span data-ttu-id="969ed-207">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="969ed-207">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="969ed-208">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="969ed-208">latestSupportedTlsVersion</span></span> | <span data-ttu-id="969ed-209">字符串</span><span class="sxs-lookup"><span data-stu-id="969ed-209">String</span></span> | <span data-ttu-id="969ed-210">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="969ed-210">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="969ed-211">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="969ed-211">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="969ed-212">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="969ed-212">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="969ed-213">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="969ed-213">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="969ed-214">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="969ed-214">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="969ed-215">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="969ed-215">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="969ed-216">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="969ed-216">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="969ed-217">Resource</span><span class="sxs-lookup"><span data-stu-id="969ed-217">Resource</span></span>            | <span data-ttu-id="969ed-218">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="969ed-218">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="969ed-219">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="969ed-219">Security **alert**</span></span>     | <span data-ttu-id="969ed-220">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-220">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="969ed-221">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="969ed-221">Teams **callRecord**</span></span>    | <span data-ttu-id="969ed-222">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-222">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="969ed-223">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="969ed-223">Teams **chatMessage**</span></span>    | <span data-ttu-id="969ed-224">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="969ed-224">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="969ed-225">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="969ed-225">Group **conversation**</span></span> | <span data-ttu-id="969ed-226">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-226">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="969ed-227">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="969ed-227">OneDrive **driveItem**</span></span>    | <span data-ttu-id="969ed-228">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-228">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="969ed-229">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="969ed-229">SharePoint **list**</span></span>    | <span data-ttu-id="969ed-230">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-230">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="969ed-231">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="969ed-231">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="969ed-232">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-232">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="969ed-233">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="969ed-233">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="969ed-234">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-234">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="969ed-235">**状态**</span><span class="sxs-lookup"><span data-stu-id="969ed-235">**presence**</span></span>        | <span data-ttu-id="969ed-236">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="969ed-236">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="969ed-237">打印 **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="969ed-237">Print **printTaskDefinition**</span></span> | <span data-ttu-id="969ed-238">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-238">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="969ed-239">**todoTask**</span><span class="sxs-lookup"><span data-stu-id="969ed-239">**todoTask**</span></span>              | <span data-ttu-id="969ed-240">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="969ed-240">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="969ed-241">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="969ed-241">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="969ed-242">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="969ed-242">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="969ed-243">关系</span><span class="sxs-lookup"><span data-stu-id="969ed-243">Relationships</span></span>

<span data-ttu-id="969ed-244">无。</span><span class="sxs-lookup"><span data-stu-id="969ed-244">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="969ed-245">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="969ed-245">JSON representation</span></span>

<span data-ttu-id="969ed-246">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="969ed-246">Here is a JSON representation of the resource.</span></span>

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
  "expirationDateTime": "string (timestamp)",
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
[状态]: ./presence.md
[presence]: ./presence.md
[printTaskDefinition]: ./printtaskdefinition.md
[todoTask]: ./todotask.md

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


