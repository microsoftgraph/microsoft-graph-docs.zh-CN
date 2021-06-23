---
title: 订阅资源类型
description: 订阅允许客户端应用接收有关 Microsoft Graph 数据更改的通知。目前，支持订阅以下资源：
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: resourcePageType
ms.openlocfilehash: 8debe063c768c66061e16fd89a2e46f6bc7b6d9b
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082284"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="ee2b8-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="ee2b8-104">subscription resource type</span></span>

<span data-ttu-id="ee2b8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee2b8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee2b8-p102">订阅允许客户端应用接收有关 Microsoft Graph 数据更改的通知。目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="ee2b8-p102">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph. Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="ee2b8-108">Microsoft Graph 安全性 API 中的[警报][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-108">An [alert][] from the Microsoft Graph Security API.</span></span>
- <span data-ttu-id="ee2b8-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-109">A [callRecord][] produced after a call or meeting in Microsoft Teams.</span></span>
- <span data-ttu-id="ee2b8-110">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-110">A [chatMessage][] sent via teams or channels in Microsoft Teams.</span></span>
- <span data-ttu-id="ee2b8-111">Microsoft 365 组中的[对话][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-111">A [conversation][] in a Microsoft 365 group.</span></span>
- <span data-ttu-id="ee2b8-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive.</span></span>
- <span data-ttu-id="ee2b8-113">SharePoint [site][]下的[list][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-113">A [list][] under a SharePoint [site][].</span></span>
- <span data-ttu-id="ee2b8-114">Outlook 中的[邮件][]、[事件][]或[联系人][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-114">A [message][], [event][], or [contact][] in Outlook.</span></span>
- <span data-ttu-id="ee2b8-115">[打印机][] (当打印机的打印作业进入”JobFetchable”状态时 - 准备好提取打印) 和通用打印中的 [printTaskDefinition][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-115">A [printer][] (when a print job for the printer gets to JobFetchable state - ready to be fetched for printing) and a [printTaskDefinition][] in Universal Print.</span></span> <span data-ttu-id="ee2b8-116">有关详细信息，请参阅 [订阅云打印 API 中的更改通知](/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-116">For more information, see [Subscribe to change notifications from cloud printing APIs](/graph/universal-print-webhook-notifications).</span></span>
- <span data-ttu-id="ee2b8-117">Azure Active Directory 中的[用户][]或[组][]。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-117">A [user][] or [group][] in Azure Active Directory.</span></span>

<span data-ttu-id="ee2b8-118">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-118">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="ee2b8-119">方法</span><span class="sxs-lookup"><span data-stu-id="ee2b8-119">Methods</span></span>

| <span data-ttu-id="ee2b8-120">方法</span><span class="sxs-lookup"><span data-stu-id="ee2b8-120">Method</span></span> | <span data-ttu-id="ee2b8-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="ee2b8-121">Return Type</span></span> | <span data-ttu-id="ee2b8-122">说明</span><span class="sxs-lookup"><span data-stu-id="ee2b8-122">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="ee2b8-123">创建订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-123">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="ee2b8-124">订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-124">subscription</span></span>](subscription.md) | <span data-ttu-id="ee2b8-125">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-125">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="ee2b8-126">更新订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-126">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="ee2b8-127">订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-127">subscription</span></span>](subscription.md) | <span data-ttu-id="ee2b8-128">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-128">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="ee2b8-129">列出订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-129">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="ee2b8-130">订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-130">subscription</span></span>](subscription.md) | <span data-ttu-id="ee2b8-131">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-131">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="ee2b8-132">获取订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-132">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="ee2b8-133">订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-133">subscription</span></span>](subscription.md) | <span data-ttu-id="ee2b8-134">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-134">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="ee2b8-135">删除订阅</span><span class="sxs-lookup"><span data-stu-id="ee2b8-135">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="ee2b8-136">无</span><span class="sxs-lookup"><span data-stu-id="ee2b8-136">None</span></span> | <span data-ttu-id="ee2b8-137">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-137">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ee2b8-138">属性</span><span class="sxs-lookup"><span data-stu-id="ee2b8-138">Properties</span></span>

| <span data-ttu-id="ee2b8-139">属性</span><span class="sxs-lookup"><span data-stu-id="ee2b8-139">Property</span></span> | <span data-ttu-id="ee2b8-140">类型</span><span class="sxs-lookup"><span data-stu-id="ee2b8-140">Type</span></span> | <span data-ttu-id="ee2b8-141">说明</span><span class="sxs-lookup"><span data-stu-id="ee2b8-141">Description</span></span> | <span data-ttu-id="ee2b8-142">支持的资源</span><span class="sxs-lookup"><span data-stu-id="ee2b8-142">Supported Resources</span></span> |
|:---------|:-----|:------------|:--------------|
| <span data-ttu-id="ee2b8-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="ee2b8-143">applicationId</span></span> | <span data-ttu-id="ee2b8-144">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-144">string</span></span> | <span data-ttu-id="ee2b8-p104">用于创建订阅的应用程序的标识符。 只读。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-p104">Identifier of the application used to create the subscription. Read-only.</span></span> | <span data-ttu-id="ee2b8-147">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-147">All</span></span> |
| <span data-ttu-id="ee2b8-148">changeType</span><span class="sxs-lookup"><span data-stu-id="ee2b8-148">changeType</span></span> | <span data-ttu-id="ee2b8-149">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-149">string</span></span> | <span data-ttu-id="ee2b8-150">必填。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-150">Required.</span></span> <span data-ttu-id="ee2b8-151">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-151">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="ee2b8-152">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-152">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="ee2b8-153">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-153">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="ee2b8-154">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-154">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="ee2b8-155">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-155">User and group change notifications support `updated` and `deleted` changeType.</span></span> | <span data-ttu-id="ee2b8-156">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-156">All</span></span> |
| <span data-ttu-id="ee2b8-157">clientState</span><span class="sxs-lookup"><span data-stu-id="ee2b8-157">clientState</span></span> | <span data-ttu-id="ee2b8-158">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-158">string</span></span> | <span data-ttu-id="ee2b8-159">可选。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-159">Optional.</span></span> <span data-ttu-id="ee2b8-160">指定服务为每个变更通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-160">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="ee2b8-161">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-161">The maximum length is 128 characters.</span></span> <span data-ttu-id="ee2b8-162">通过对比与订阅一起发送的 `clientState` 属性值和与每个变更通知一起接收的 `clientState` 属性值，客户端可以检查变更通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-162">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> | <span data-ttu-id="ee2b8-163">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-163">All</span></span> |
| <span data-ttu-id="ee2b8-164">creatorId</span><span class="sxs-lookup"><span data-stu-id="ee2b8-164">creatorId</span></span> | <span data-ttu-id="ee2b8-165">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-165">string</span></span> | <span data-ttu-id="ee2b8-166">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-166">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="ee2b8-167">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-167">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="ee2b8-168">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-168">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="ee2b8-169">只读。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-169">Read-only.</span></span> | <span data-ttu-id="ee2b8-170">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-170">All</span></span> |
| <span data-ttu-id="ee2b8-171">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="ee2b8-171">encryptionCertificate</span></span> | <span data-ttu-id="ee2b8-172">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-172">string</span></span> | <span data-ttu-id="ee2b8-173">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-173">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="ee2b8-174">可选。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-174">Optional.</span></span> <span data-ttu-id="ee2b8-175">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-175">Required when **includeResourceData** is true.</span></span> | <span data-ttu-id="ee2b8-176">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-176">All</span></span> |
| <span data-ttu-id="ee2b8-177">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="ee2b8-177">encryptionCertificateId</span></span> | <span data-ttu-id="ee2b8-178">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-178">string</span></span> | <span data-ttu-id="ee2b8-p110">应用程序提供的自定义标识符，以帮助识别解密资源数据所需的证书。 可选的。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-p110">A custom app-provided identifier to help identify the certificate needed to decrypt resource data. Optional.</span></span>| <span data-ttu-id="ee2b8-181">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-181">All</span></span> |
| <span data-ttu-id="ee2b8-182">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee2b8-182">expirationDateTime</span></span> | <span data-ttu-id="ee2b8-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee2b8-183">DateTimeOffset</span></span> | <span data-ttu-id="ee2b8-p111">必填。指定 webhook 订阅过期的日期和时间。时间使用 UTC 格式，也可以是从订阅创建（因订阅资源不同而异）开始的一段时间。请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-p111">Required. Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.  See the table below for maximum supported subscription length of time.</span></span> | <span data-ttu-id="ee2b8-188">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-188">All</span></span> |
| <span data-ttu-id="ee2b8-189">id</span><span class="sxs-lookup"><span data-stu-id="ee2b8-189">id</span></span> | <span data-ttu-id="ee2b8-190">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-190">string</span></span> | <span data-ttu-id="ee2b8-p112">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-p112">Unique identifier for the subscription. Read-only.</span></span> | <span data-ttu-id="ee2b8-193">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-193">All</span></span> |
| <span data-ttu-id="ee2b8-194">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="ee2b8-194">includeResourceData</span></span> | <span data-ttu-id="ee2b8-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="ee2b8-195">Boolean</span></span> | <span data-ttu-id="ee2b8-196">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-196">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="ee2b8-197">可选。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-197">Optional.</span></span> | <span data-ttu-id="ee2b8-198">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-198">All</span></span> |
| <span data-ttu-id="ee2b8-199">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="ee2b8-199">latestSupportedTlsVersion</span></span> | <span data-ttu-id="ee2b8-200">字符串</span><span class="sxs-lookup"><span data-stu-id="ee2b8-200">String</span></span> | <span data-ttu-id="ee2b8-201">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-201">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="ee2b8-202">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-202">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="ee2b8-203">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-203">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="ee2b8-204">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-204">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="ee2b8-205">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-205">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="ee2b8-206">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-206">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> | <span data-ttu-id="ee2b8-207">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-207">All</span></span> |
| <span data-ttu-id="ee2b8-208">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="ee2b8-208">lifecycleNotificationUrl</span></span> | <span data-ttu-id="ee2b8-209">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-209">string</span></span> | <span data-ttu-id="ee2b8-210">接收生命周期通知（包括 `subscriptionRemoved` 和 `missed` 通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-210">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="ee2b8-211">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-211">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="ee2b8-212">可选。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-212">Optional.</span></span> <br><br><span data-ttu-id="ee2b8-213">[阅读](/graph/webhooks-lifecycle)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-213">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> | <span data-ttu-id="ee2b8-214">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-214">All</span></span> |
| <span data-ttu-id="ee2b8-215">notificationContentType</span><span class="sxs-lookup"><span data-stu-id="ee2b8-215">notificationContentType</span></span> | <span data-ttu-id="ee2b8-216">字符串</span><span class="sxs-lookup"><span data-stu-id="ee2b8-216">string</span></span> | <span data-ttu-id="ee2b8-217">MS Graph 所需的内容类型为更改支持的资源类型变更通知。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-217">Desired content-type for MS Graph change notifications for supported resource types.</span></span> <span data-ttu-id="ee2b8-218">默认内容类型为“application/json”内容类型。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-218">The default content-type is the "application/json" content-type.</span></span> | <span data-ttu-id="ee2b8-219">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-219">All</span></span> |
| <span data-ttu-id="ee2b8-220">notificationQueryOptions</span><span class="sxs-lookup"><span data-stu-id="ee2b8-220">notificationQueryOptions</span></span> | <span data-ttu-id="ee2b8-221">字符串</span><span class="sxs-lookup"><span data-stu-id="ee2b8-221">string</span></span> | <span data-ttu-id="ee2b8-222">用于指定目标资源值的 OData 查询选项。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-222">OData Query Options for specifying value for the targeting resource.</span></span> <span data-ttu-id="ee2b8-223">当资源达到与此处所提供的查询选项相匹配的状态时，客户端会收到通知。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-223">Clients receive notifications when resource reaches the state matching the query options provided here.</span></span> <span data-ttu-id="ee2b8-224">有了订阅创建有效负载中的新属性以及所有现有属性后，每当资源达到 “notificationQueryOptions” 属性中提到的所需状态时，Webhook 就会发送通知，例如当打印作业完成时、当打印作业资源 `isFetchable` 属性值变为 true 时，等等。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-224">With this new property in the subscription creation payload along with all existing properties, Webhooks will deliver notifications whenever a resource reaches the desired state mentioned in the notificationQueryOptions property eg  when the print job is completed, when a print job resource `isFetchable` property value becomes true etc.</span></span> | [<span data-ttu-id="ee2b8-225">通用打印服务</span><span class="sxs-lookup"><span data-stu-id="ee2b8-225">Universal Print Service</span></span>](/graph/universal-print-webhook-notifications) |
| <span data-ttu-id="ee2b8-226">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="ee2b8-226">notificationUrl</span></span> | <span data-ttu-id="ee2b8-227">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-227">string</span></span> | <span data-ttu-id="ee2b8-p120">必填。将接收变更通知的终结点 URL。该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-p120">Required. The URL of the endpoint that will receive the change notifications. This URL must make use of the HTTPS protocol.</span></span> | <span data-ttu-id="ee2b8-231">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-231">All</span></span> |
| <span data-ttu-id="ee2b8-232">resource</span><span class="sxs-lookup"><span data-stu-id="ee2b8-232">resource</span></span> | <span data-ttu-id="ee2b8-233">string</span><span class="sxs-lookup"><span data-stu-id="ee2b8-233">string</span></span> | <span data-ttu-id="ee2b8-234">必需。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-234">Required.</span></span> <span data-ttu-id="ee2b8-235">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-235">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="ee2b8-236">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-236">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="ee2b8-237">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-237">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>| <span data-ttu-id="ee2b8-238">全部</span><span class="sxs-lookup"><span data-stu-id="ee2b8-238">All</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="ee2b8-239">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="ee2b8-239">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="ee2b8-240">Resource</span><span class="sxs-lookup"><span data-stu-id="ee2b8-240">Resource</span></span>            | <span data-ttu-id="ee2b8-241">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="ee2b8-241">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="ee2b8-242">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-242">Security **alert**</span></span>     | <span data-ttu-id="ee2b8-243">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-243">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="ee2b8-244">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-244">Teams **callRecord**</span></span>    | <span data-ttu-id="ee2b8-245">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-245">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="ee2b8-246">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-246">Teams **chatMessage**</span></span>    | <span data-ttu-id="ee2b8-247">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-247">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="ee2b8-248">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-248">Group **conversation**</span></span> | <span data-ttu-id="ee2b8-249">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-249">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ee2b8-250">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-250">OneDrive **driveItem**</span></span>    | <span data-ttu-id="ee2b8-251">42300 分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-251">42300 minutes (under 30 days)</span></span>    |
| <span data-ttu-id="ee2b8-252">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-252">SharePoint **list**</span></span>    | <span data-ttu-id="ee2b8-253">42300 分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-253">42300 minutes (under 30 days)</span></span>    |
| <span data-ttu-id="ee2b8-254">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-254">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="ee2b8-255">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-255">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ee2b8-256">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="ee2b8-256">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="ee2b8-257">4230 分钟（不到 29 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-257">41760 minutes (under 29 days)</span></span>    |
| <span data-ttu-id="ee2b8-258">打印 **打印机**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-258">Print **printer**</span></span> | <span data-ttu-id="ee2b8-259">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-259">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ee2b8-260">打印 **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="ee2b8-260">Print **printTaskDefinition**</span></span> | <span data-ttu-id="ee2b8-261">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="ee2b8-261">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="ee2b8-262">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-262">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="ee2b8-263">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-263">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="ee2b8-264">关系</span><span class="sxs-lookup"><span data-stu-id="ee2b8-264">Relationships</span></span>

<span data-ttu-id="ee2b8-265">无</span><span class="sxs-lookup"><span data-stu-id="ee2b8-265">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee2b8-266">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee2b8-266">JSON representation</span></span>

<span data-ttu-id="ee2b8-267">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee2b8-267">Here is a JSON representation of the resource.</span></span>

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
[打印机]: ./printer.md
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;"
}-->

