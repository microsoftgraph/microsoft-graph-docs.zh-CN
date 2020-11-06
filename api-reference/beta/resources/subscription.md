---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b3efc8736b5dffe745f43ad096837cb05827e734
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932491"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="f4638-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="f4638-104">subscription resource type</span></span>

<span data-ttu-id="f4638-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4638-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4638-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="f4638-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="f4638-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="f4638-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="f4638-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="f4638-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="f4638-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="f4638-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="f4638-110">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="f4638-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="f4638-111">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="f4638-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="f4638-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="f4638-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="f4638-113">SharePoint [网站][]下的[列表][] </span><span class="sxs-lookup"><span data-stu-id="f4638-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="f4638-114">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="f4638-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="f4638-115">Microsoft 团队中的用户[是否存在][]</span><span class="sxs-lookup"><span data-stu-id="f4638-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="f4638-116">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="f4638-116">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="f4638-117">打印服务中的[printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="f4638-117">A [printTaskDefinition][] in Print Service</span></span>

<span data-ttu-id="f4638-118">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="f4638-118">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="f4638-119">方法</span><span class="sxs-lookup"><span data-stu-id="f4638-119">Methods</span></span>

| <span data-ttu-id="f4638-120">方法</span><span class="sxs-lookup"><span data-stu-id="f4638-120">Method</span></span> | <span data-ttu-id="f4638-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4638-121">Return Type</span></span> | <span data-ttu-id="f4638-122">说明</span><span class="sxs-lookup"><span data-stu-id="f4638-122">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="f4638-123">创建订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-123">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f4638-124">订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-124">subscription</span></span>](subscription.md) | <span data-ttu-id="f4638-125">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="f4638-125">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="f4638-126">更新订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-126">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="f4638-127">订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-127">subscription</span></span>](subscription.md) | <span data-ttu-id="f4638-128">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="f4638-128">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="f4638-129">列出订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-129">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="f4638-130">订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-130">subscription</span></span>](subscription.md) | <span data-ttu-id="f4638-131">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="f4638-131">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="f4638-132">获取订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-132">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="f4638-133">订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-133">subscription</span></span>](subscription.md) | <span data-ttu-id="f4638-134">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4638-134">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="f4638-135">删除订阅</span><span class="sxs-lookup"><span data-stu-id="f4638-135">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="f4638-136">无</span><span class="sxs-lookup"><span data-stu-id="f4638-136">None</span></span> | <span data-ttu-id="f4638-137">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="f4638-137">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4638-138">属性</span><span class="sxs-lookup"><span data-stu-id="f4638-138">Properties</span></span>

| <span data-ttu-id="f4638-139">属性</span><span class="sxs-lookup"><span data-stu-id="f4638-139">Property</span></span> | <span data-ttu-id="f4638-140">类型</span><span class="sxs-lookup"><span data-stu-id="f4638-140">Type</span></span> | <span data-ttu-id="f4638-141">说明</span><span class="sxs-lookup"><span data-stu-id="f4638-141">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f4638-142">changeType</span><span class="sxs-lookup"><span data-stu-id="f4638-142">changeType</span></span> | <span data-ttu-id="f4638-143">string</span><span class="sxs-lookup"><span data-stu-id="f4638-143">string</span></span> | <span data-ttu-id="f4638-144">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="f4638-144">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="f4638-145">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="f4638-145">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f4638-146">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="f4638-146">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="f4638-147">必填。</span><span class="sxs-lookup"><span data-stu-id="f4638-147">Required.</span></span> <br><br><span data-ttu-id="f4638-148">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="f4638-148">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="f4638-149">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="f4638-149">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="f4638-150">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="f4638-150">notificationUrl</span></span> | <span data-ttu-id="f4638-151">string</span><span class="sxs-lookup"><span data-stu-id="f4638-151">string</span></span> | <span data-ttu-id="f4638-152">接收更改通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="f4638-152">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="f4638-153">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="f4638-153">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="f4638-154">必填。</span><span class="sxs-lookup"><span data-stu-id="f4638-154">Required.</span></span> |
| <span data-ttu-id="f4638-155">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="f4638-155">lifecycleNotificationUrl</span></span> | <span data-ttu-id="f4638-156">string</span><span class="sxs-lookup"><span data-stu-id="f4638-156">string</span></span> | <span data-ttu-id="f4638-157">接收生命周期通知（包括和通知）的终结点的 URL `subscriptionRemoved` `missed` 。</span><span class="sxs-lookup"><span data-stu-id="f4638-157">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="f4638-158">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="f4638-158">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="f4638-159">可选。</span><span class="sxs-lookup"><span data-stu-id="f4638-159">Optional.</span></span> <br><br><span data-ttu-id="f4638-160">[阅读](/graph/webhooks-lifecycle) 有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4638-160">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="f4638-161">resource</span><span class="sxs-lookup"><span data-stu-id="f4638-161">resource</span></span> | <span data-ttu-id="f4638-162">string</span><span class="sxs-lookup"><span data-stu-id="f4638-162">string</span></span> | <span data-ttu-id="f4638-163">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="f4638-163">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="f4638-164">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="f4638-164">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="f4638-165">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="f4638-165">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="f4638-166">必填。</span><span class="sxs-lookup"><span data-stu-id="f4638-166">Required.</span></span> |
| <span data-ttu-id="f4638-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f4638-167">expirationDateTime</span></span> | <span data-ttu-id="f4638-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4638-168">DateTimeOffset</span></span> | <span data-ttu-id="f4638-169">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f4638-169">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="f4638-170">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="f4638-170">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="f4638-171">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="f4638-171">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="f4638-172">必填。</span><span class="sxs-lookup"><span data-stu-id="f4638-172">Required.</span></span> |
| <span data-ttu-id="f4638-173">clientState</span><span class="sxs-lookup"><span data-stu-id="f4638-173">clientState</span></span> | <span data-ttu-id="f4638-174">string</span><span class="sxs-lookup"><span data-stu-id="f4638-174">string</span></span> | <span data-ttu-id="f4638-175">指定在每次更改通知中由服务发送的 **clientState** 属性的值。</span><span class="sxs-lookup"><span data-stu-id="f4638-175">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="f4638-176">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="f4638-176">The maximum length is 255 characters.</span></span> <span data-ttu-id="f4638-177">客户端可以通过将随订阅发送的 **clientState** 属性的值与每个更改通知接收的 **clientState** 属性的值进行比较，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="f4638-177">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="f4638-178">可选。</span><span class="sxs-lookup"><span data-stu-id="f4638-178">Optional.</span></span> |
| <span data-ttu-id="f4638-179">id</span><span class="sxs-lookup"><span data-stu-id="f4638-179">id</span></span> | <span data-ttu-id="f4638-180">string</span><span class="sxs-lookup"><span data-stu-id="f4638-180">string</span></span> | <span data-ttu-id="f4638-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f4638-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="f4638-183">applicationId</span><span class="sxs-lookup"><span data-stu-id="f4638-183">applicationId</span></span> | <span data-ttu-id="f4638-184">string</span><span class="sxs-lookup"><span data-stu-id="f4638-184">string</span></span> | <span data-ttu-id="f4638-185">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="f4638-185">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="f4638-186">只读。</span><span class="sxs-lookup"><span data-stu-id="f4638-186">Read-only.</span></span> |
| <span data-ttu-id="f4638-187">creatorId</span><span class="sxs-lookup"><span data-stu-id="f4638-187">creatorId</span></span> | <span data-ttu-id="f4638-188">string</span><span class="sxs-lookup"><span data-stu-id="f4638-188">string</span></span> | <span data-ttu-id="f4638-189">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="f4638-189">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="f4638-190">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="f4638-190">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="f4638-191">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="f4638-191">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="f4638-192">只读。</span><span class="sxs-lookup"><span data-stu-id="f4638-192">Read-only.</span></span> |
| <span data-ttu-id="f4638-193">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="f4638-193">includeResourceData</span></span> | <span data-ttu-id="f4638-194">布尔值</span><span class="sxs-lookup"><span data-stu-id="f4638-194">Boolean</span></span> | <span data-ttu-id="f4638-195">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="f4638-195">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="f4638-196">可选。</span><span class="sxs-lookup"><span data-stu-id="f4638-196">Optional.</span></span> | 
| <span data-ttu-id="f4638-197">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="f4638-197">encryptionCertificate</span></span> | <span data-ttu-id="f4638-198">string</span><span class="sxs-lookup"><span data-stu-id="f4638-198">string</span></span> | <span data-ttu-id="f4638-199">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="f4638-199">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="f4638-200">可选。</span><span class="sxs-lookup"><span data-stu-id="f4638-200">Optional.</span></span> <span data-ttu-id="f4638-201">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="f4638-201">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="f4638-202">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="f4638-202">encryptionCertificateId</span></span> | <span data-ttu-id="f4638-203">string</span><span class="sxs-lookup"><span data-stu-id="f4638-203">string</span></span> | <span data-ttu-id="f4638-204">自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="f4638-204">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="f4638-205">可选。</span><span class="sxs-lookup"><span data-stu-id="f4638-205">Optional.</span></span> <span data-ttu-id="f4638-206">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="f4638-206">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="f4638-207">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="f4638-207">latestSupportedTlsVersion</span></span> | <span data-ttu-id="f4638-208">字符串</span><span class="sxs-lookup"><span data-stu-id="f4638-208">String</span></span> | <span data-ttu-id="f4638-209">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="f4638-209">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl** , supports.</span></span> <span data-ttu-id="f4638-210">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="f4638-210">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="f4638-211">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="f4638-211">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="f4638-212">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="f4638-212">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="f4638-213">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="f4638-213">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="f4638-214">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="f4638-214">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="f4638-215">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="f4638-215">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="f4638-216">Resource</span><span class="sxs-lookup"><span data-stu-id="f4638-216">Resource</span></span>            | <span data-ttu-id="f4638-217">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="f4638-217">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="f4638-218">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="f4638-218">Security **alert**</span></span>     | <span data-ttu-id="f4638-219">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-219">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="f4638-220">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="f4638-220">Teams **callRecord**</span></span>    | <span data-ttu-id="f4638-221">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-221">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="f4638-222">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="f4638-222">Teams **chatMessage**</span></span>    | <span data-ttu-id="f4638-223">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="f4638-223">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="f4638-224">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="f4638-224">Group **conversation**</span></span> | <span data-ttu-id="f4638-225">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-225">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4638-226">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4638-226">OneDrive **driveItem**</span></span>    | <span data-ttu-id="f4638-227">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-227">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4638-228">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="f4638-228">SharePoint **list**</span></span>    | <span data-ttu-id="f4638-229">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-229">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4638-230">Outlook **邮件** 、 **事件** 、 **联系人**</span><span class="sxs-lookup"><span data-stu-id="f4638-230">Outlook **message** , **event** , **contact**</span></span>              | <span data-ttu-id="f4638-231">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-231">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4638-232">**用户** 、 **组** 、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="f4638-232">**user** , **group** , other directory resources</span></span>   | <span data-ttu-id="f4638-233">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-233">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4638-234">**状态**</span><span class="sxs-lookup"><span data-stu-id="f4638-234">**presence**</span></span>        | <span data-ttu-id="f4638-235">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="f4638-235">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="f4638-236">打印 **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="f4638-236">Print **printTaskDefinition**</span></span> | <span data-ttu-id="f4638-237">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="f4638-237">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="f4638-238">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="f4638-238">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="f4638-239">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="f4638-239">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="f4638-240">关系</span><span class="sxs-lookup"><span data-stu-id="f4638-240">Relationships</span></span>

<span data-ttu-id="f4638-241">无。</span><span class="sxs-lookup"><span data-stu-id="f4638-241">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4638-242">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4638-242">JSON representation</span></span>

<span data-ttu-id="f4638-243">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4638-243">Here is a JSON representation of the resource.</span></span>

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


