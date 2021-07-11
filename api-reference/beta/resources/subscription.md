---
title: 订阅资源类型
description: 订阅允许客户端应用接收有关 Microsoft Graph 数据更改的通知。目前，支持订阅以下资源：
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 183812b655aa62ce48b405fccfaf3b4b8841117f
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366960"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="dbdda-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="dbdda-104">subscription resource type</span></span>

<span data-ttu-id="dbdda-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbdda-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbdda-p102">订阅允许客户端应用接收有关 Microsoft Graph 数据更改的通知。目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="dbdda-p102">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph. Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="dbdda-108">Microsoft Graph 安全性 API 中的[警报][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-108">An [alert][] from the Microsoft Graph Security API.</span></span>
- <span data-ttu-id="dbdda-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-109">A [callRecord][] produced after a call or meeting in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-110">频道[中的](./channel.md)Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="dbdda-110">A [channel](./channel.md) in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-111">聊天[中的](./chat.md)Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="dbdda-111">A [chat](./chat.md) in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-112">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-112">A [chatMessage][] sent via teams or channels in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-113">Microsoft 365 组中的[对话][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-113">A [conversation][] in a Microsoft 365 group.</span></span>
- <span data-ttu-id="dbdda-114">团队、频道或聊天中的[conversationMember](./conversationmember.md) Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="dbdda-114">A [conversationMember](./conversationmember.md) in a team, channel, or chat in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-115">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容。</span><span class="sxs-lookup"><span data-stu-id="dbdda-115">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive.</span></span>
- <span data-ttu-id="dbdda-116">SharePoint [site][]下的[list][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-116">A [list][] under a SharePoint [site][].</span></span>
- <span data-ttu-id="dbdda-117">Outlook 中的[邮件][]、[事件][]或[联系人][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-117">A [message][], [event][], or [contact][] in Outlook.</span></span>
- <span data-ttu-id="dbdda-118">[用户][]状态Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="dbdda-118">The [presence][] of a user in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-119">[Microsoft Teams。](./team.md)</span><span class="sxs-lookup"><span data-stu-id="dbdda-119">A [team](./team.md) in Microsoft Teams.</span></span>
- <span data-ttu-id="dbdda-120">Azure Active Directory 中的[用户][]或[组][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-120">A [user][] or [group][] in Azure Active Directory.</span></span>
- <span data-ttu-id="dbdda-121">[打印机][] (当打印机的打印作业进入”JobFetchable”状态时 - 准备好提取打印) 和通用打印中的 [printTaskDefinition][]。</span><span class="sxs-lookup"><span data-stu-id="dbdda-121">A [printer][] (when a print job for the printer gets to JobFetchable state - ready to be fetched for printing) and a [printTaskDefinition][] in Universal Print.</span></span> <span data-ttu-id="dbdda-122">有关详细信息，请参阅 [订阅云打印 API 中的更改通知](/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="dbdda-122">For more information, see [Subscribe to change notifications from cloud printing APIs](/graph/universal-print-webhook-notifications).</span></span>
- <span data-ttu-id="dbdda-123">用户[在任务][]中的微软待办。</span><span class="sxs-lookup"><span data-stu-id="dbdda-123">A [todoTask][] of a user in Microsoft To Do.</span></span>

<span data-ttu-id="dbdda-124">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="dbdda-124">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="dbdda-125">方法</span><span class="sxs-lookup"><span data-stu-id="dbdda-125">Methods</span></span>

| <span data-ttu-id="dbdda-126">方法</span><span class="sxs-lookup"><span data-stu-id="dbdda-126">Method</span></span> | <span data-ttu-id="dbdda-127">返回类型</span><span class="sxs-lookup"><span data-stu-id="dbdda-127">Return Type</span></span> | <span data-ttu-id="dbdda-128">说明</span><span class="sxs-lookup"><span data-stu-id="dbdda-128">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="dbdda-129">创建订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-129">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="dbdda-130">订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-130">subscription</span></span>](subscription.md) | <span data-ttu-id="dbdda-131">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="dbdda-131">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="dbdda-132">更新订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-132">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="dbdda-133">订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-133">subscription</span></span>](subscription.md) | <span data-ttu-id="dbdda-134">通过更新其过期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="dbdda-134">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="dbdda-135">列出订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-135">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="dbdda-136">订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-136">subscription</span></span>](subscription.md) | <span data-ttu-id="dbdda-137">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="dbdda-137">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="dbdda-138">获取订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-138">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="dbdda-139">订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-139">subscription</span></span>](subscription.md) | <span data-ttu-id="dbdda-140">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dbdda-140">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="dbdda-141">删除订阅</span><span class="sxs-lookup"><span data-stu-id="dbdda-141">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="dbdda-142">无</span><span class="sxs-lookup"><span data-stu-id="dbdda-142">None</span></span> | <span data-ttu-id="dbdda-143">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="dbdda-143">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dbdda-144">属性</span><span class="sxs-lookup"><span data-stu-id="dbdda-144">Properties</span></span>

| <span data-ttu-id="dbdda-145">属性</span><span class="sxs-lookup"><span data-stu-id="dbdda-145">Property</span></span> | <span data-ttu-id="dbdda-146">类型</span><span class="sxs-lookup"><span data-stu-id="dbdda-146">Type</span></span> | <span data-ttu-id="dbdda-147">说明</span><span class="sxs-lookup"><span data-stu-id="dbdda-147">Description</span></span> | <span data-ttu-id="dbdda-148">支持的资源</span><span class="sxs-lookup"><span data-stu-id="dbdda-148">Supported Resources</span></span> |
|:---------|:-----|:------------|:--------------|
| <span data-ttu-id="dbdda-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="dbdda-149">applicationId</span></span> | <span data-ttu-id="dbdda-150">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-150">string</span></span> | <span data-ttu-id="dbdda-p104">用于创建订阅的应用程序的标识符。 只读。</span><span class="sxs-lookup"><span data-stu-id="dbdda-p104">Identifier of the application used to create the subscription. Read-only.</span></span> | <span data-ttu-id="dbdda-153">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-153">All</span></span> |
| <span data-ttu-id="dbdda-154">changeType</span><span class="sxs-lookup"><span data-stu-id="dbdda-154">changeType</span></span> | <span data-ttu-id="dbdda-155">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-155">string</span></span> | <span data-ttu-id="dbdda-156">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="dbdda-156">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="dbdda-157">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="dbdda-157">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="dbdda-158">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="dbdda-158">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="dbdda-159">必填。</span><span class="sxs-lookup"><span data-stu-id="dbdda-159">Required.</span></span> <br><br><span data-ttu-id="dbdda-160">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="dbdda-160">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="dbdda-161">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="dbdda-161">User and group change notifications support `updated` and `deleted` changeType.</span></span> | <span data-ttu-id="dbdda-162">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-162">All</span></span> |
| <span data-ttu-id="dbdda-163">clientState</span><span class="sxs-lookup"><span data-stu-id="dbdda-163">clientState</span></span> | <span data-ttu-id="dbdda-164">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-164">string</span></span> | <span data-ttu-id="dbdda-165">指定服务在每个更改通知中发送的 **clientState** 属性的值。</span><span class="sxs-lookup"><span data-stu-id="dbdda-165">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="dbdda-166">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="dbdda-166">The maximum length is 255 characters.</span></span> <span data-ttu-id="dbdda-167">通过比较与订阅一起发送的 **clientState** 属性的值与每个更改通知一起收到的 **clientState** 属性的值，客户端可以检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="dbdda-167">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="dbdda-168">可选。</span><span class="sxs-lookup"><span data-stu-id="dbdda-168">Optional.</span></span> | <span data-ttu-id="dbdda-169">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-169">All</span></span> |
| <span data-ttu-id="dbdda-170">creatorId</span><span class="sxs-lookup"><span data-stu-id="dbdda-170">creatorId</span></span> | <span data-ttu-id="dbdda-171">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-171">string</span></span> | <span data-ttu-id="dbdda-172">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="dbdda-172">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="dbdda-173">如果应用使用委派权限创建订阅，则此字段包含代表应用调用的登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="dbdda-173">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="dbdda-174">如果应用程序使用应用程序权限，则此字段包含与应用程序对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="dbdda-174">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="dbdda-175">只读。</span><span class="sxs-lookup"><span data-stu-id="dbdda-175">Read-only.</span></span> | <span data-ttu-id="dbdda-176">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-176">All</span></span> |
| <span data-ttu-id="dbdda-177">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="dbdda-177">encryptionCertificate</span></span> | <span data-ttu-id="dbdda-178">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-178">string</span></span> | <span data-ttu-id="dbdda-179">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="dbdda-179">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="dbdda-180">可选。</span><span class="sxs-lookup"><span data-stu-id="dbdda-180">Optional.</span></span> <span data-ttu-id="dbdda-181">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="dbdda-181">Required when **includeResourceData** is true.</span></span> | <span data-ttu-id="dbdda-182">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-182">All</span></span> |
| <span data-ttu-id="dbdda-183">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="dbdda-183">encryptionCertificateId</span></span> | <span data-ttu-id="dbdda-184">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-184">string</span></span> | <span data-ttu-id="dbdda-185">自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="dbdda-185">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="dbdda-186">可选。</span><span class="sxs-lookup"><span data-stu-id="dbdda-186">Optional.</span></span> <span data-ttu-id="dbdda-187">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="dbdda-187">Required when **includeResourceData** is true.</span></span> | <span data-ttu-id="dbdda-188">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-188">All</span></span> |
| <span data-ttu-id="dbdda-189">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dbdda-189">expirationDateTime</span></span> | <span data-ttu-id="dbdda-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbdda-190">DateTimeOffset</span></span> | <span data-ttu-id="dbdda-191">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dbdda-191">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="dbdda-192">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="dbdda-192">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="dbdda-193">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="dbdda-193">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="dbdda-194">必填。</span><span class="sxs-lookup"><span data-stu-id="dbdda-194">Required.</span></span> | <span data-ttu-id="dbdda-195">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-195">All</span></span> |
| <span data-ttu-id="dbdda-196">id</span><span class="sxs-lookup"><span data-stu-id="dbdda-196">id</span></span> | <span data-ttu-id="dbdda-197">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-197">string</span></span> | <span data-ttu-id="dbdda-p112">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="dbdda-p112">Unique identifier for the subscription. Read-only.</span></span> | <span data-ttu-id="dbdda-200">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-200">All</span></span> |
| <span data-ttu-id="dbdda-201">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="dbdda-201">includeResourceData</span></span> | <span data-ttu-id="dbdda-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="dbdda-202">Boolean</span></span> | <span data-ttu-id="dbdda-203">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="dbdda-203">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="dbdda-204">可选。</span><span class="sxs-lookup"><span data-stu-id="dbdda-204">Optional.</span></span> | <span data-ttu-id="dbdda-205">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-205">All</span></span> |
| <span data-ttu-id="dbdda-206">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="dbdda-206">latestSupportedTlsVersion</span></span> | <span data-ttu-id="dbdda-207">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-207">string</span></span> | <span data-ttu-id="dbdda-208">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="dbdda-208">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="dbdda-209">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="dbdda-209">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="dbdda-210">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="dbdda-210">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="dbdda-211">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="dbdda-211">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="dbdda-212">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="dbdda-212">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="dbdda-213">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="dbdda-213">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> | <span data-ttu-id="dbdda-214">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-214">All</span></span> |
| <span data-ttu-id="dbdda-215">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="dbdda-215">lifecycleNotificationUrl</span></span> | <span data-ttu-id="dbdda-216">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-216">string</span></span> | <span data-ttu-id="dbdda-217">接收生命周期通知（包括 `subscriptionRemoved` 和 `missed` 通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="dbdda-217">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="dbdda-218">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="dbdda-218">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="dbdda-219">可选。</span><span class="sxs-lookup"><span data-stu-id="dbdda-219">Optional.</span></span> <br><br><span data-ttu-id="dbdda-220">[阅读](/graph/webhooks-lifecycle)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dbdda-220">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> | <span data-ttu-id="dbdda-221">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-221">All</span></span> |
| <span data-ttu-id="dbdda-222">notificationContentType</span><span class="sxs-lookup"><span data-stu-id="dbdda-222">notificationContentType</span></span> | <span data-ttu-id="dbdda-223">字符串</span><span class="sxs-lookup"><span data-stu-id="dbdda-223">string</span></span> | <span data-ttu-id="dbdda-224">MS Graph 所需的内容类型为更改支持的资源类型变更通知。</span><span class="sxs-lookup"><span data-stu-id="dbdda-224">Desired content-type for MS Graph change notifications for supported resource types.</span></span> <span data-ttu-id="dbdda-225">默认内容类型为“application/json”内容类型。</span><span class="sxs-lookup"><span data-stu-id="dbdda-225">The default content-type is the "application/json" content-type.</span></span> | <span data-ttu-id="dbdda-226">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-226">All</span></span> |
| <span data-ttu-id="dbdda-227">notificationQueryOptions</span><span class="sxs-lookup"><span data-stu-id="dbdda-227">notificationQueryOptions</span></span> | <span data-ttu-id="dbdda-228">字符串</span><span class="sxs-lookup"><span data-stu-id="dbdda-228">string</span></span> | <span data-ttu-id="dbdda-229">用于指定目标资源值的 OData 查询选项。</span><span class="sxs-lookup"><span data-stu-id="dbdda-229">OData Query Options for specifying value for the targeting resource.</span></span> <span data-ttu-id="dbdda-230">当资源达到与此处所提供的查询选项相匹配的状态时，客户端会收到通知。</span><span class="sxs-lookup"><span data-stu-id="dbdda-230">Clients receive notifications when resource reaches the state matching the query options provided here.</span></span> <span data-ttu-id="dbdda-231">有了订阅创建有效负载中的新属性以及所有现有属性后，每当资源达到 “notificationQueryOptions” 属性中提到的所需状态时，Webhook 就会发送通知，例如当打印作业完成时、当打印作业资源 `isFetchable` 属性值变为 true 时，等等。</span><span class="sxs-lookup"><span data-stu-id="dbdda-231">With this new property in the subscription creation payload along with all existing properties, Webhooks will deliver notifications whenever a resource reaches the desired state mentioned in the notificationQueryOptions property eg  when the print job is completed, when a print job resource `isFetchable` property value becomes true etc.</span></span> | [<span data-ttu-id="dbdda-232">通用打印服务</span><span class="sxs-lookup"><span data-stu-id="dbdda-232">Universal Print Service</span></span>](/graph/universal-print-webhook-notifications) |
| <span data-ttu-id="dbdda-233">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="dbdda-233">notificationUrl</span></span> | <span data-ttu-id="dbdda-234">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-234">string</span></span> | <span data-ttu-id="dbdda-235">接收更改通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="dbdda-235">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="dbdda-236">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="dbdda-236">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="dbdda-237">必填。</span><span class="sxs-lookup"><span data-stu-id="dbdda-237">Required.</span></span> | <span data-ttu-id="dbdda-238">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-238">All</span></span> |
| <span data-ttu-id="dbdda-239">resource</span><span class="sxs-lookup"><span data-stu-id="dbdda-239">resource</span></span> | <span data-ttu-id="dbdda-240">string</span><span class="sxs-lookup"><span data-stu-id="dbdda-240">string</span></span> | <span data-ttu-id="dbdda-241">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="dbdda-241">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="dbdda-242">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="dbdda-242">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="dbdda-243">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="dbdda-243">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="dbdda-244">必填。</span><span class="sxs-lookup"><span data-stu-id="dbdda-244">Required.</span></span> | <span data-ttu-id="dbdda-245">全部</span><span class="sxs-lookup"><span data-stu-id="dbdda-245">All</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="dbdda-246">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="dbdda-246">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="dbdda-247">Resource</span><span class="sxs-lookup"><span data-stu-id="dbdda-247">Resource</span></span>            | <span data-ttu-id="dbdda-248">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="dbdda-248">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="dbdda-249">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="dbdda-249">Security **alert**</span></span>     | <span data-ttu-id="dbdda-250">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-250">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="dbdda-251">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="dbdda-251">Teams **callRecord**</span></span>    | <span data-ttu-id="dbdda-252">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-252">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="dbdda-253">Teams **频道**</span><span class="sxs-lookup"><span data-stu-id="dbdda-253">Teams **channel**</span></span>    | <span data-ttu-id="dbdda-254">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="dbdda-254">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="dbdda-255">Teams **聊天**</span><span class="sxs-lookup"><span data-stu-id="dbdda-255">Teams **chat**</span></span> | <span data-ttu-id="dbdda-256">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="dbdda-256">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="dbdda-257">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="dbdda-257">Teams **chatMessage**</span></span>    | <span data-ttu-id="dbdda-258">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="dbdda-258">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="dbdda-259">Teams **conversationMember**</span><span class="sxs-lookup"><span data-stu-id="dbdda-259">Teams **conversationMember**</span></span>    | <span data-ttu-id="dbdda-260">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="dbdda-260">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="dbdda-261">Teams **团队**</span><span class="sxs-lookup"><span data-stu-id="dbdda-261">Teams **team**</span></span>    | <span data-ttu-id="dbdda-262">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="dbdda-262">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="dbdda-263">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="dbdda-263">Group **conversation**</span></span> | <span data-ttu-id="dbdda-264">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-264">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dbdda-265">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="dbdda-265">OneDrive **driveItem**</span></span>    | <span data-ttu-id="dbdda-266">42300 分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-266">42300 minutes (under 30 days)</span></span>    |
| <span data-ttu-id="dbdda-267">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="dbdda-267">SharePoint **list**</span></span>    | <span data-ttu-id="dbdda-268">42300 分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-268">42300 minutes (under 30 days)</span></span>    |
| <span data-ttu-id="dbdda-269">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="dbdda-269">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="dbdda-270">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-270">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dbdda-271">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="dbdda-271">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="dbdda-272">4230 分钟（不到 29 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-272">41760 minutes (under 29 days)</span></span>    |
| <span data-ttu-id="dbdda-273">**状态**</span><span class="sxs-lookup"><span data-stu-id="dbdda-273">**presence**</span></span>        | <span data-ttu-id="dbdda-274">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="dbdda-274">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="dbdda-275">打印 **打印机**</span><span class="sxs-lookup"><span data-stu-id="dbdda-275">Print **printer**</span></span> | <span data-ttu-id="dbdda-276">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-276">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dbdda-277">打印 **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="dbdda-277">Print **printTaskDefinition**</span></span> | <span data-ttu-id="dbdda-278">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-278">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dbdda-279">**todoTask**</span><span class="sxs-lookup"><span data-stu-id="dbdda-279">**todoTask**</span></span>              | <span data-ttu-id="dbdda-280">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="dbdda-280">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="dbdda-281">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="dbdda-281">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="dbdda-282">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="dbdda-282">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="dbdda-283">关系</span><span class="sxs-lookup"><span data-stu-id="dbdda-283">Relationships</span></span>

<span data-ttu-id="dbdda-284">无。</span><span class="sxs-lookup"><span data-stu-id="dbdda-284">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbdda-285">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dbdda-285">JSON representation</span></span>

<span data-ttu-id="dbdda-286">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbdda-286">Here is a JSON representation of the resource.</span></span>

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
  "latestSupportedTlsVersion": "string",
  "notificationContentType": "string",
  "notificationQueryOptions": "string"
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
[打印机]: ./printer.md
[printer]: ./printer.md
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


