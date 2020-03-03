---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: fb2dd66e9e18e4951005bcda2b249235e99cd829
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394440"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="657e0-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="657e0-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657e0-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="657e0-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="657e0-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="657e0-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="657e0-107">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="657e0-107">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="657e0-108">Microsoft 团队中的呼叫或会议之后生成的[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="657e0-108">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="657e0-109">通过 Microsoft 团队中的团队或频道发送的[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="657e0-109">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="657e0-110">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="657e0-110">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="657e0-111">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="657e0-111">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="657e0-112">SharePoint[网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="657e0-112">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="657e0-113">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="657e0-113">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="657e0-114">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="657e0-114">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="657e0-115">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="657e0-115">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="657e0-116">方法</span><span class="sxs-lookup"><span data-stu-id="657e0-116">Methods</span></span>

| <span data-ttu-id="657e0-117">方法</span><span class="sxs-lookup"><span data-stu-id="657e0-117">Method</span></span> | <span data-ttu-id="657e0-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="657e0-118">Return Type</span></span> | <span data-ttu-id="657e0-119">说明</span><span class="sxs-lookup"><span data-stu-id="657e0-119">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="657e0-120">创建订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-120">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="657e0-121">订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-121">subscription</span></span>](subscription.md) | <span data-ttu-id="657e0-122">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="657e0-122">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="657e0-123">更新订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-123">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="657e0-124">订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-124">subscription</span></span>](subscription.md) | <span data-ttu-id="657e0-125">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="657e0-125">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="657e0-126">列出订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-126">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="657e0-127">订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-127">subscription</span></span>](subscription.md) | <span data-ttu-id="657e0-128">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="657e0-128">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="657e0-129">获取订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-129">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="657e0-130">订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-130">subscription</span></span>](subscription.md) | <span data-ttu-id="657e0-131">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="657e0-131">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="657e0-132">删除订阅</span><span class="sxs-lookup"><span data-stu-id="657e0-132">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="657e0-133">无</span><span class="sxs-lookup"><span data-stu-id="657e0-133">None</span></span> | <span data-ttu-id="657e0-134">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="657e0-134">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="657e0-135">属性</span><span class="sxs-lookup"><span data-stu-id="657e0-135">Properties</span></span>

| <span data-ttu-id="657e0-136">属性</span><span class="sxs-lookup"><span data-stu-id="657e0-136">Property</span></span> | <span data-ttu-id="657e0-137">类型</span><span class="sxs-lookup"><span data-stu-id="657e0-137">Type</span></span> | <span data-ttu-id="657e0-138">说明</span><span class="sxs-lookup"><span data-stu-id="657e0-138">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="657e0-139">changeType</span><span class="sxs-lookup"><span data-stu-id="657e0-139">changeType</span></span> | <span data-ttu-id="657e0-140">string</span><span class="sxs-lookup"><span data-stu-id="657e0-140">string</span></span> | <span data-ttu-id="657e0-141">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="657e0-141">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="657e0-142">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="657e0-142">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="657e0-143">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="657e0-143">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="657e0-144">必填。</span><span class="sxs-lookup"><span data-stu-id="657e0-144">Required.</span></span> <br><br><span data-ttu-id="657e0-145">注意：驱动器根项和列表通知仅支持`updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="657e0-145">Note: Drive root item and list notifications support only the `updated` changeType.</span></span> <span data-ttu-id="657e0-146">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="657e0-146">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="657e0-147">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="657e0-147">notificationUrl</span></span> | <span data-ttu-id="657e0-148">string</span><span class="sxs-lookup"><span data-stu-id="657e0-148">string</span></span> | <span data-ttu-id="657e0-149">接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="657e0-149">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="657e0-150">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="657e0-150">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="657e0-151">必填。</span><span class="sxs-lookup"><span data-stu-id="657e0-151">Required.</span></span> |
| <span data-ttu-id="657e0-152">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="657e0-152">lifecycleNotificationUrl</span></span> | <span data-ttu-id="657e0-153">string</span><span class="sxs-lookup"><span data-stu-id="657e0-153">string</span></span> | <span data-ttu-id="657e0-154">接收生命周期通知（包括`subscriptionRemoved`和`missed`通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="657e0-154">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="657e0-155">如果未提供，这些通知将传递给**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="657e0-155">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="657e0-156">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="657e0-156">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="657e0-157">可选。</span><span class="sxs-lookup"><span data-stu-id="657e0-157">Optional.</span></span> <br><br><span data-ttu-id="657e0-158">[阅读](/graph/webhooks-outlook-authz)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="657e0-158">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="657e0-159">resource</span><span class="sxs-lookup"><span data-stu-id="657e0-159">resource</span></span> | <span data-ttu-id="657e0-160">string</span><span class="sxs-lookup"><span data-stu-id="657e0-160">string</span></span> | <span data-ttu-id="657e0-161">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="657e0-161">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="657e0-162">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="657e0-162">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="657e0-163">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="657e0-163">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="657e0-164">必填。</span><span class="sxs-lookup"><span data-stu-id="657e0-164">Required.</span></span> |
| <span data-ttu-id="657e0-165">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="657e0-165">expirationDateTime</span></span> | <span data-ttu-id="657e0-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="657e0-166">DateTimeOffset</span></span> | <span data-ttu-id="657e0-167">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="657e0-167">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="657e0-168">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="657e0-168">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="657e0-169">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="657e0-169">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="657e0-170">必填。</span><span class="sxs-lookup"><span data-stu-id="657e0-170">Required.</span></span> |
| <span data-ttu-id="657e0-171">clientState</span><span class="sxs-lookup"><span data-stu-id="657e0-171">clientState</span></span> | <span data-ttu-id="657e0-172">string</span><span class="sxs-lookup"><span data-stu-id="657e0-172">string</span></span> | <span data-ttu-id="657e0-173">指定每个通知中由服务发送的**clientState**属性的值。</span><span class="sxs-lookup"><span data-stu-id="657e0-173">Specifies the value of the **clientState** property sent by the service in each notification.</span></span> <span data-ttu-id="657e0-174">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="657e0-174">The maximum length is 255 characters.</span></span> <span data-ttu-id="657e0-175">客户端可以通过将随订阅发送的**clientState**属性的值与每个通知收到的**clientState**属性的值进行比较，来检查该通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="657e0-175">The client can check that the notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each notification.</span></span> <span data-ttu-id="657e0-176">可选。</span><span class="sxs-lookup"><span data-stu-id="657e0-176">Optional.</span></span> |
| <span data-ttu-id="657e0-177">id</span><span class="sxs-lookup"><span data-stu-id="657e0-177">id</span></span> | <span data-ttu-id="657e0-178">字符串</span><span class="sxs-lookup"><span data-stu-id="657e0-178">string</span></span> | <span data-ttu-id="657e0-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="657e0-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="657e0-181">applicationId</span><span class="sxs-lookup"><span data-stu-id="657e0-181">applicationId</span></span> | <span data-ttu-id="657e0-182">string</span><span class="sxs-lookup"><span data-stu-id="657e0-182">string</span></span> | <span data-ttu-id="657e0-183">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="657e0-183">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="657e0-184">只读。</span><span class="sxs-lookup"><span data-stu-id="657e0-184">Read-only.</span></span> |
| <span data-ttu-id="657e0-185">creatorId</span><span class="sxs-lookup"><span data-stu-id="657e0-185">creatorId</span></span> | <span data-ttu-id="657e0-186">string</span><span class="sxs-lookup"><span data-stu-id="657e0-186">string</span></span> | <span data-ttu-id="657e0-187">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="657e0-187">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="657e0-188">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="657e0-188">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="657e0-189">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="657e0-189">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="657e0-190">只读。</span><span class="sxs-lookup"><span data-stu-id="657e0-190">Read-only.</span></span> |
| <span data-ttu-id="657e0-191">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="657e0-191">includeResourceData</span></span> | <span data-ttu-id="657e0-192">布尔</span><span class="sxs-lookup"><span data-stu-id="657e0-192">Boolean</span></span> | <span data-ttu-id="657e0-193">当设置为`true`时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（如聊天邮件的内容）。</span><span class="sxs-lookup"><span data-stu-id="657e0-193">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="657e0-194">可选。</span><span class="sxs-lookup"><span data-stu-id="657e0-194">Optional.</span></span> | 
| <span data-ttu-id="657e0-195">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="657e0-195">encryptionCertificate</span></span> | <span data-ttu-id="657e0-196">string</span><span class="sxs-lookup"><span data-stu-id="657e0-196">string</span></span> | <span data-ttu-id="657e0-197">具有用于在通知中对资源数据进行加密的公钥的证书的 base64 编码表示形式。</span><span class="sxs-lookup"><span data-stu-id="657e0-197">A base64-encoded representation of a certificate with a public key used to encrypt resource data in notifications.</span></span> <span data-ttu-id="657e0-198">可选。</span><span class="sxs-lookup"><span data-stu-id="657e0-198">Optional.</span></span> <span data-ttu-id="657e0-199">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="657e0-199">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="657e0-200">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="657e0-200">encryptionCertificateId</span></span> | <span data-ttu-id="657e0-201">string</span><span class="sxs-lookup"><span data-stu-id="657e0-201">string</span></span> | <span data-ttu-id="657e0-202">自定义应用程序提供的标识符，用于帮助确定解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="657e0-202">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="657e0-203">可选。</span><span class="sxs-lookup"><span data-stu-id="657e0-203">Optional.</span></span> <span data-ttu-id="657e0-204">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="657e0-204">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="657e0-205">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="657e0-205">latestSupportedTlsVersion</span></span> | <span data-ttu-id="657e0-206">字符串</span><span class="sxs-lookup"><span data-stu-id="657e0-206">String</span></span> | <span data-ttu-id="657e0-207">指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="657e0-207">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="657e0-208">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="657e0-208">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="657e0-209">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="657e0-209">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="657e0-210">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="657e0-210">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="657e0-211">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="657e0-211">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="657e0-212">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="657e0-212">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="657e0-213">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="657e0-213">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="657e0-214">Resource</span><span class="sxs-lookup"><span data-stu-id="657e0-214">Resource</span></span>            | <span data-ttu-id="657e0-215">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="657e0-215">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="657e0-216">安全**警报**</span><span class="sxs-lookup"><span data-stu-id="657e0-216">Security **alert**</span></span>     | <span data-ttu-id="657e0-217">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-217">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="657e0-218">团队**callRecord**</span><span class="sxs-lookup"><span data-stu-id="657e0-218">Teams **callRecord**</span></span>    | <span data-ttu-id="657e0-219">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-219">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="657e0-220">团队**了 chatmessage**</span><span class="sxs-lookup"><span data-stu-id="657e0-220">Teams **chatMessage**</span></span>    | <span data-ttu-id="657e0-221">60分钟（1小时）</span><span class="sxs-lookup"><span data-stu-id="657e0-221">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="657e0-222">组**对话**</span><span class="sxs-lookup"><span data-stu-id="657e0-222">Group **conversation**</span></span> | <span data-ttu-id="657e0-223">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-223">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="657e0-224">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="657e0-224">OneDrive **driveItem**</span></span>    | <span data-ttu-id="657e0-225">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-225">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="657e0-226">SharePoint**列表**</span><span class="sxs-lookup"><span data-stu-id="657e0-226">SharePoint **list**</span></span>    | <span data-ttu-id="657e0-227">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-227">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="657e0-228">Outlook**邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="657e0-228">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="657e0-229">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-229">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="657e0-230">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="657e0-230">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="657e0-231">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="657e0-231">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="657e0-232">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="657e0-232">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="657e0-233">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="657e0-233">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="657e0-234">关系</span><span class="sxs-lookup"><span data-stu-id="657e0-234">Relationships</span></span>

<span data-ttu-id="657e0-235">无。</span><span class="sxs-lookup"><span data-stu-id="657e0-235">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="657e0-236">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="657e0-236">JSON representation</span></span>

<span data-ttu-id="657e0-237">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="657e0-237">Here is a JSON representation of the resource.</span></span>

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
[网站]: ./site.md
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
