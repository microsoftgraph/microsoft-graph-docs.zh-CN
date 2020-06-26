---
title: 订阅资源类型
description: 订阅允许客户端应用接收有关 Microsoft Graph 中的数据更改的更改通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 44e1588873c27631ccee22f956838f8220078bad
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44893674"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="7e502-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="7e502-104">subscription resource type</span></span>

<span data-ttu-id="7e502-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e502-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e502-106">订阅允许客户端应用接收有关 Microsoft Graph 中的数据更改的更改通知。</span><span class="sxs-lookup"><span data-stu-id="7e502-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="7e502-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="7e502-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="7e502-108">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="7e502-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="7e502-109">Microsoft 团队中的呼叫或会议之后生成的[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="7e502-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="7e502-110">通过 Microsoft 团队中的团队或频道发送的[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="7e502-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="7e502-111">Microsoft 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="7e502-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="7e502-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="7e502-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="7e502-113">SharePoint [网站][]下的[列表][] </span><span class="sxs-lookup"><span data-stu-id="7e502-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="7e502-114">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="7e502-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="7e502-115">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="7e502-115">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="7e502-116">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="7e502-116">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="7e502-117">方法</span><span class="sxs-lookup"><span data-stu-id="7e502-117">Methods</span></span>

| <span data-ttu-id="7e502-118">方法</span><span class="sxs-lookup"><span data-stu-id="7e502-118">Method</span></span> | <span data-ttu-id="7e502-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e502-119">Return Type</span></span> | <span data-ttu-id="7e502-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e502-120">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="7e502-121">创建订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-121">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="7e502-122">订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-122">subscription</span></span>](subscription.md) | <span data-ttu-id="7e502-123">订阅侦听器应用程序，以便在 Microsoft Graph 数据发生更改时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="7e502-123">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="7e502-124">更新订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-124">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="7e502-125">订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-125">subscription</span></span>](subscription.md) | <span data-ttu-id="7e502-126">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="7e502-126">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="7e502-127">列出订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-127">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="7e502-128">订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-128">subscription</span></span>](subscription.md) | <span data-ttu-id="7e502-129">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="7e502-129">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="7e502-130">获取订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-130">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="7e502-131">订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-131">subscription</span></span>](subscription.md) | <span data-ttu-id="7e502-132">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e502-132">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="7e502-133">删除订阅</span><span class="sxs-lookup"><span data-stu-id="7e502-133">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="7e502-134">无</span><span class="sxs-lookup"><span data-stu-id="7e502-134">None</span></span> | <span data-ttu-id="7e502-135">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="7e502-135">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e502-136">属性</span><span class="sxs-lookup"><span data-stu-id="7e502-136">Properties</span></span>

| <span data-ttu-id="7e502-137">属性</span><span class="sxs-lookup"><span data-stu-id="7e502-137">Property</span></span> | <span data-ttu-id="7e502-138">类型</span><span class="sxs-lookup"><span data-stu-id="7e502-138">Type</span></span> | <span data-ttu-id="7e502-139">说明</span><span class="sxs-lookup"><span data-stu-id="7e502-139">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="7e502-140">changeType</span><span class="sxs-lookup"><span data-stu-id="7e502-140">changeType</span></span> | <span data-ttu-id="7e502-141">string</span><span class="sxs-lookup"><span data-stu-id="7e502-141">string</span></span> | <span data-ttu-id="7e502-142">指示订阅的资源中将引发更改通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="7e502-142">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="7e502-143">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="7e502-143">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="7e502-144">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="7e502-144">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="7e502-145">必填。</span><span class="sxs-lookup"><span data-stu-id="7e502-145">Required.</span></span> <br><br><span data-ttu-id="7e502-146">注意：驱动器根项和列表更改通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="7e502-146">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="7e502-147">用户和组更改通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="7e502-147">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="7e502-148">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="7e502-148">notificationUrl</span></span> | <span data-ttu-id="7e502-149">string</span><span class="sxs-lookup"><span data-stu-id="7e502-149">string</span></span> | <span data-ttu-id="7e502-150">接收更改通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="7e502-150">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="7e502-151">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="7e502-151">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="7e502-152">必填。</span><span class="sxs-lookup"><span data-stu-id="7e502-152">Required.</span></span> |
| <span data-ttu-id="7e502-153">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="7e502-153">lifecycleNotificationUrl</span></span> | <span data-ttu-id="7e502-154">string</span><span class="sxs-lookup"><span data-stu-id="7e502-154">string</span></span> | <span data-ttu-id="7e502-155">接收生命周期通知（包括和通知）的终结点的 URL `subscriptionRemoved` `missed` 。</span><span class="sxs-lookup"><span data-stu-id="7e502-155">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="7e502-156">如果未提供，这些通知将传递给**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="7e502-156">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="7e502-157">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="7e502-157">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="7e502-158">可选。</span><span class="sxs-lookup"><span data-stu-id="7e502-158">Optional.</span></span> <br><br><span data-ttu-id="7e502-159">[阅读](/graph/webhooks-outlook-authz)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7e502-159">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="7e502-160">resource</span><span class="sxs-lookup"><span data-stu-id="7e502-160">resource</span></span> | <span data-ttu-id="7e502-161">string</span><span class="sxs-lookup"><span data-stu-id="7e502-161">string</span></span> | <span data-ttu-id="7e502-162">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="7e502-162">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="7e502-163">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="7e502-163">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="7e502-164">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="7e502-164">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="7e502-165">必填。</span><span class="sxs-lookup"><span data-stu-id="7e502-165">Required.</span></span> |
| <span data-ttu-id="7e502-166">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e502-166">expirationDateTime</span></span> | <span data-ttu-id="7e502-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e502-167">DateTimeOffset</span></span> | <span data-ttu-id="7e502-168">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7e502-168">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="7e502-169">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="7e502-169">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="7e502-170">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="7e502-170">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="7e502-171">必填。</span><span class="sxs-lookup"><span data-stu-id="7e502-171">Required.</span></span> |
| <span data-ttu-id="7e502-172">clientState</span><span class="sxs-lookup"><span data-stu-id="7e502-172">clientState</span></span> | <span data-ttu-id="7e502-173">string</span><span class="sxs-lookup"><span data-stu-id="7e502-173">string</span></span> | <span data-ttu-id="7e502-174">指定在每次更改通知中由服务发送的**clientState**属性的值。</span><span class="sxs-lookup"><span data-stu-id="7e502-174">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="7e502-175">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="7e502-175">The maximum length is 255 characters.</span></span> <span data-ttu-id="7e502-176">客户端可以通过将随订阅发送的**clientState**属性的值与每个更改通知接收的**clientState**属性的值进行比较，来检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="7e502-176">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="7e502-177">可选。</span><span class="sxs-lookup"><span data-stu-id="7e502-177">Optional.</span></span> |
| <span data-ttu-id="7e502-178">id</span><span class="sxs-lookup"><span data-stu-id="7e502-178">id</span></span> | <span data-ttu-id="7e502-179">字符串</span><span class="sxs-lookup"><span data-stu-id="7e502-179">string</span></span> | <span data-ttu-id="7e502-180">Unique identifier for the subscription.</span><span class="sxs-lookup"><span data-stu-id="7e502-180">Unique identifier for the subscription.</span></span> <span data-ttu-id="7e502-181">Read-only.</span><span class="sxs-lookup"><span data-stu-id="7e502-181">Read-only.</span></span> |
| <span data-ttu-id="7e502-182">applicationId</span><span class="sxs-lookup"><span data-stu-id="7e502-182">applicationId</span></span> | <span data-ttu-id="7e502-183">string</span><span class="sxs-lookup"><span data-stu-id="7e502-183">string</span></span> | <span data-ttu-id="7e502-184">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="7e502-184">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="7e502-185">只读。</span><span class="sxs-lookup"><span data-stu-id="7e502-185">Read-only.</span></span> |
| <span data-ttu-id="7e502-186">creatorId</span><span class="sxs-lookup"><span data-stu-id="7e502-186">creatorId</span></span> | <span data-ttu-id="7e502-187">string</span><span class="sxs-lookup"><span data-stu-id="7e502-187">string</span></span> | <span data-ttu-id="7e502-188">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="7e502-188">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="7e502-189">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="7e502-189">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="7e502-190">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="7e502-190">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="7e502-191">只读。</span><span class="sxs-lookup"><span data-stu-id="7e502-191">Read-only.</span></span> |
| <span data-ttu-id="7e502-192">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="7e502-192">includeResourceData</span></span> | <span data-ttu-id="7e502-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e502-193">Boolean</span></span> | <span data-ttu-id="7e502-194">当设置为时 `true` ，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（如聊天邮件的内容）。</span><span class="sxs-lookup"><span data-stu-id="7e502-194">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="7e502-195">可选。</span><span class="sxs-lookup"><span data-stu-id="7e502-195">Optional.</span></span> | 
| <span data-ttu-id="7e502-196">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="7e502-196">encryptionCertificate</span></span> | <span data-ttu-id="7e502-197">string</span><span class="sxs-lookup"><span data-stu-id="7e502-197">string</span></span> | <span data-ttu-id="7e502-198">具有用于在更改通知中对资源数据进行加密的公钥的证书的 base64 编码表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e502-198">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="7e502-199">可选。</span><span class="sxs-lookup"><span data-stu-id="7e502-199">Optional.</span></span> <span data-ttu-id="7e502-200">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="7e502-200">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="7e502-201">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="7e502-201">encryptionCertificateId</span></span> | <span data-ttu-id="7e502-202">string</span><span class="sxs-lookup"><span data-stu-id="7e502-202">string</span></span> | <span data-ttu-id="7e502-203">自定义应用程序提供的标识符，用于帮助确定解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="7e502-203">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="7e502-204">可选。</span><span class="sxs-lookup"><span data-stu-id="7e502-204">Optional.</span></span> <span data-ttu-id="7e502-205">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="7e502-205">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="7e502-206">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="7e502-206">latestSupportedTlsVersion</span></span> | <span data-ttu-id="7e502-207">字符串</span><span class="sxs-lookup"><span data-stu-id="7e502-207">String</span></span> | <span data-ttu-id="7e502-208">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="7e502-208">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="7e502-209">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="7e502-209">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="7e502-210">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="7e502-210">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="7e502-211">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="7e502-211">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="7e502-212">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="7e502-212">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="7e502-213">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="7e502-213">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="7e502-214">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="7e502-214">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="7e502-215">Resource</span><span class="sxs-lookup"><span data-stu-id="7e502-215">Resource</span></span>            | <span data-ttu-id="7e502-216">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="7e502-216">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="7e502-217">安全**警报**</span><span class="sxs-lookup"><span data-stu-id="7e502-217">Security **alert**</span></span>     | <span data-ttu-id="7e502-218">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-218">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="7e502-219">团队**callRecord**</span><span class="sxs-lookup"><span data-stu-id="7e502-219">Teams **callRecord**</span></span>    | <span data-ttu-id="7e502-220">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-220">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="7e502-221">团队**了 chatmessage**</span><span class="sxs-lookup"><span data-stu-id="7e502-221">Teams **chatMessage**</span></span>    | <span data-ttu-id="7e502-222">60分钟（1小时）</span><span class="sxs-lookup"><span data-stu-id="7e502-222">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="7e502-223">组**对话**</span><span class="sxs-lookup"><span data-stu-id="7e502-223">Group **conversation**</span></span> | <span data-ttu-id="7e502-224">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-224">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7e502-225">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="7e502-225">OneDrive **driveItem**</span></span>    | <span data-ttu-id="7e502-226">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-226">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7e502-227">SharePoint**列表**</span><span class="sxs-lookup"><span data-stu-id="7e502-227">SharePoint **list**</span></span>    | <span data-ttu-id="7e502-228">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-228">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7e502-229">Outlook**邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="7e502-229">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="7e502-230">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-230">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7e502-231">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="7e502-231">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="7e502-232">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="7e502-232">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="7e502-233">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="7e502-233">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="7e502-234">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="7e502-234">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="7e502-235">关系</span><span class="sxs-lookup"><span data-stu-id="7e502-235">Relationships</span></span>

<span data-ttu-id="7e502-236">无。</span><span class="sxs-lookup"><span data-stu-id="7e502-236">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e502-237">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e502-237">JSON representation</span></span>

<span data-ttu-id="7e502-238">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e502-238">Here is a JSON representation of the resource.</span></span>

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
