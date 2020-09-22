---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: aaa7fe900852f00851cafea2c18e71ec7fec7c8c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193328"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="b8a88-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="b8a88-104">subscription resource type</span></span>

<span data-ttu-id="b8a88-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8a88-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8a88-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="b8a88-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="b8a88-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="b8a88-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="b8a88-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="b8a88-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="b8a88-110">通过 Microsoft 团队中的团队或频道发送的[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="b8a88-111">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="b8a88-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="b8a88-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="b8a88-113">SharePoint [网站][]下的[列表][] </span><span class="sxs-lookup"><span data-stu-id="b8a88-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="b8a88-114">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="b8a88-115">Microsoft 团队中的用户[是否存在][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="b8a88-116">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="b8a88-116">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="b8a88-117">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="b8a88-117">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="b8a88-118">方法</span><span class="sxs-lookup"><span data-stu-id="b8a88-118">Methods</span></span>

| <span data-ttu-id="b8a88-119">方法</span><span class="sxs-lookup"><span data-stu-id="b8a88-119">Method</span></span> | <span data-ttu-id="b8a88-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8a88-120">Return Type</span></span> | <span data-ttu-id="b8a88-121">说明</span><span class="sxs-lookup"><span data-stu-id="b8a88-121">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="b8a88-122">创建订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-122">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="b8a88-123">订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-123">subscription</span></span>](subscription.md) | <span data-ttu-id="b8a88-124">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="b8a88-124">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="b8a88-125">更新订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-125">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="b8a88-126">订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-126">subscription</span></span>](subscription.md) | <span data-ttu-id="b8a88-127">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="b8a88-127">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="b8a88-128">列出订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-128">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="b8a88-129">订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-129">subscription</span></span>](subscription.md) | <span data-ttu-id="b8a88-130">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="b8a88-130">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="b8a88-131">获取订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-131">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="b8a88-132">订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-132">subscription</span></span>](subscription.md) | <span data-ttu-id="b8a88-133">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8a88-133">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="b8a88-134">删除订阅</span><span class="sxs-lookup"><span data-stu-id="b8a88-134">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="b8a88-135">无</span><span class="sxs-lookup"><span data-stu-id="b8a88-135">None</span></span> | <span data-ttu-id="b8a88-136">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="b8a88-136">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8a88-137">属性</span><span class="sxs-lookup"><span data-stu-id="b8a88-137">Properties</span></span>

| <span data-ttu-id="b8a88-138">属性</span><span class="sxs-lookup"><span data-stu-id="b8a88-138">Property</span></span> | <span data-ttu-id="b8a88-139">类型</span><span class="sxs-lookup"><span data-stu-id="b8a88-139">Type</span></span> | <span data-ttu-id="b8a88-140">说明</span><span class="sxs-lookup"><span data-stu-id="b8a88-140">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b8a88-141">changeType</span><span class="sxs-lookup"><span data-stu-id="b8a88-141">changeType</span></span> | <span data-ttu-id="b8a88-142">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-142">string</span></span> | <span data-ttu-id="b8a88-143">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="b8a88-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="b8a88-144">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b8a88-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="b8a88-145">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="b8a88-145">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="b8a88-146">必需。</span><span class="sxs-lookup"><span data-stu-id="b8a88-146">Required.</span></span> <br><br><span data-ttu-id="b8a88-147">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="b8a88-147">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="b8a88-148">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="b8a88-148">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="b8a88-149">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="b8a88-149">notificationUrl</span></span> | <span data-ttu-id="b8a88-150">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-150">string</span></span> | <span data-ttu-id="b8a88-151">接收更改通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="b8a88-151">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="b8a88-152">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="b8a88-152">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="b8a88-153">必需。</span><span class="sxs-lookup"><span data-stu-id="b8a88-153">Required.</span></span> |
| <span data-ttu-id="b8a88-154">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="b8a88-154">lifecycleNotificationUrl</span></span> | <span data-ttu-id="b8a88-155">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-155">string</span></span> | <span data-ttu-id="b8a88-156">接收生命周期通知（包括和通知）的终结点的 URL `subscriptionRemoved` `missed` 。</span><span class="sxs-lookup"><span data-stu-id="b8a88-156">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="b8a88-157">如果未提供，这些通知将传递给 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="b8a88-157">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="b8a88-158">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="b8a88-158">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="b8a88-159">可选。</span><span class="sxs-lookup"><span data-stu-id="b8a88-159">Optional.</span></span> <br><br><span data-ttu-id="b8a88-160">[阅读](/graph/webhooks-outlook-authz) 有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b8a88-160">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="b8a88-161">resource</span><span class="sxs-lookup"><span data-stu-id="b8a88-161">resource</span></span> | <span data-ttu-id="b8a88-162">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-162">string</span></span> | <span data-ttu-id="b8a88-163">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="b8a88-163">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="b8a88-164">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="b8a88-164">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="b8a88-165">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="b8a88-165">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="b8a88-166">必需。</span><span class="sxs-lookup"><span data-stu-id="b8a88-166">Required.</span></span> |
| <span data-ttu-id="b8a88-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b8a88-167">expirationDateTime</span></span> | <span data-ttu-id="b8a88-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8a88-168">DateTimeOffset</span></span> | <span data-ttu-id="b8a88-169">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b8a88-169">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="b8a88-170">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="b8a88-170">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="b8a88-171">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="b8a88-171">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="b8a88-172">必需。</span><span class="sxs-lookup"><span data-stu-id="b8a88-172">Required.</span></span> |
| <span data-ttu-id="b8a88-173">clientState</span><span class="sxs-lookup"><span data-stu-id="b8a88-173">clientState</span></span> | <span data-ttu-id="b8a88-174">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-174">string</span></span> | <span data-ttu-id="b8a88-175">指定在每次更改通知中由服务发送的 **clientState** 属性的值。</span><span class="sxs-lookup"><span data-stu-id="b8a88-175">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="b8a88-176">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="b8a88-176">The maximum length is 255 characters.</span></span> <span data-ttu-id="b8a88-177">客户端可以通过将随订阅发送的 **clientState** 属性的值与每个更改通知接收的 **clientState** 属性的值进行比较，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="b8a88-177">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="b8a88-178">可选。</span><span class="sxs-lookup"><span data-stu-id="b8a88-178">Optional.</span></span> |
| <span data-ttu-id="b8a88-179">id</span><span class="sxs-lookup"><span data-stu-id="b8a88-179">id</span></span> | <span data-ttu-id="b8a88-180">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-180">string</span></span> | <span data-ttu-id="b8a88-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b8a88-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="b8a88-183">applicationId</span><span class="sxs-lookup"><span data-stu-id="b8a88-183">applicationId</span></span> | <span data-ttu-id="b8a88-184">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-184">string</span></span> | <span data-ttu-id="b8a88-185">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="b8a88-185">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="b8a88-186">只读。</span><span class="sxs-lookup"><span data-stu-id="b8a88-186">Read-only.</span></span> |
| <span data-ttu-id="b8a88-187">creatorId</span><span class="sxs-lookup"><span data-stu-id="b8a88-187">creatorId</span></span> | <span data-ttu-id="b8a88-188">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-188">string</span></span> | <span data-ttu-id="b8a88-189">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="b8a88-189">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="b8a88-190">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="b8a88-190">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="b8a88-191">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="b8a88-191">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="b8a88-192">只读。</span><span class="sxs-lookup"><span data-stu-id="b8a88-192">Read-only.</span></span> |
| <span data-ttu-id="b8a88-193">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="b8a88-193">includeResourceData</span></span> | <span data-ttu-id="b8a88-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8a88-194">Boolean</span></span> | <span data-ttu-id="b8a88-195">当设置为时 `true` ，更改通知 [包括资源数据](/graph/webhooks-with-resource-data) (如聊天邮件的内容) 。</span><span class="sxs-lookup"><span data-stu-id="b8a88-195">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="b8a88-196">可选。</span><span class="sxs-lookup"><span data-stu-id="b8a88-196">Optional.</span></span> | 
| <span data-ttu-id="b8a88-197">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="b8a88-197">encryptionCertificate</span></span> | <span data-ttu-id="b8a88-198">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-198">string</span></span> | <span data-ttu-id="b8a88-199">具有用于在更改通知中对资源数据进行加密的公钥的证书的 base64 编码表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8a88-199">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="b8a88-200">可选。</span><span class="sxs-lookup"><span data-stu-id="b8a88-200">Optional.</span></span> <span data-ttu-id="b8a88-201">当 **includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="b8a88-201">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="b8a88-202">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="b8a88-202">encryptionCertificateId</span></span> | <span data-ttu-id="b8a88-203">string</span><span class="sxs-lookup"><span data-stu-id="b8a88-203">string</span></span> | <span data-ttu-id="b8a88-204">自定义应用程序提供的标识符，用于帮助确定解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="b8a88-204">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="b8a88-205">可选。</span><span class="sxs-lookup"><span data-stu-id="b8a88-205">Optional.</span></span> <span data-ttu-id="b8a88-206">当 **includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="b8a88-206">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="b8a88-207">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="b8a88-207">latestSupportedTlsVersion</span></span> | <span data-ttu-id="b8a88-208">字符串</span><span class="sxs-lookup"><span data-stu-id="b8a88-208">String</span></span> | <span data-ttu-id="b8a88-209">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="b8a88-209">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="b8a88-210">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="b8a88-210">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="b8a88-211">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="b8a88-211">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="b8a88-212">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="b8a88-212">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="b8a88-213">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="b8a88-213">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="b8a88-214">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="b8a88-214">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="b8a88-215">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="b8a88-215">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="b8a88-216">Resource</span><span class="sxs-lookup"><span data-stu-id="b8a88-216">Resource</span></span>            | <span data-ttu-id="b8a88-217">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="b8a88-217">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="b8a88-218">安全**警报**</span><span class="sxs-lookup"><span data-stu-id="b8a88-218">Security **alert**</span></span>     | <span data-ttu-id="b8a88-219">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-219">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="b8a88-220">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="b8a88-220">Teams **callRecord**</span></span>    | <span data-ttu-id="b8a88-221">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-221">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="b8a88-222">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="b8a88-222">Teams **chatMessage**</span></span>    | <span data-ttu-id="b8a88-223">60分钟 (1 小时) </span><span class="sxs-lookup"><span data-stu-id="b8a88-223">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="b8a88-224">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="b8a88-224">Group **conversation**</span></span> | <span data-ttu-id="b8a88-225">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-225">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b8a88-226">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="b8a88-226">OneDrive **driveItem**</span></span>    | <span data-ttu-id="b8a88-227">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-227">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b8a88-228">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="b8a88-228">SharePoint **list**</span></span>    | <span data-ttu-id="b8a88-229">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-229">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b8a88-230">Outlook **邮件**、 **事件**、 **联系人**</span><span class="sxs-lookup"><span data-stu-id="b8a88-230">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="b8a88-231">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-231">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b8a88-232">**用户**、 **组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="b8a88-232">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="b8a88-233">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="b8a88-233">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b8a88-234">**状态**</span><span class="sxs-lookup"><span data-stu-id="b8a88-234">**presence**</span></span>        | <span data-ttu-id="b8a88-235">60分钟 (1 小时) </span><span class="sxs-lookup"><span data-stu-id="b8a88-235">60 minutes (1 hour)</span></span> |


> <span data-ttu-id="b8a88-236">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="b8a88-236">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="b8a88-237">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="b8a88-237">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="b8a88-238">关系</span><span class="sxs-lookup"><span data-stu-id="b8a88-238">Relationships</span></span>

<span data-ttu-id="b8a88-239">无。</span><span class="sxs-lookup"><span data-stu-id="b8a88-239">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8a88-240">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8a88-240">JSON representation</span></span>

<span data-ttu-id="b8a88-241">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8a88-241">Here is a JSON representation of the resource.</span></span>

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


