---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: resourcePageType
ms.openlocfilehash: c47c4d7df11599a5983f5610ef3bfd29c80eee5b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911289"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="35658-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="35658-104">subscription resource type</span></span>

<span data-ttu-id="35658-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35658-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35658-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="35658-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="35658-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="35658-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="35658-108">Microsoft Graph 安全性 API 中的[警报][]。</span><span class="sxs-lookup"><span data-stu-id="35658-108">An [alert][] from the Microsoft Graph Security API.</span></span>
- <span data-ttu-id="35658-109">Microsoft Teams 中的通话或会议后生成的 [callRecord][]。</span><span class="sxs-lookup"><span data-stu-id="35658-109">A [callRecord][] produced after a call or meeting in Microsoft Teams.</span></span>
- <span data-ttu-id="35658-110">通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]。</span><span class="sxs-lookup"><span data-stu-id="35658-110">A [chatMessage][] sent via teams or channels in Microsoft Teams.</span></span>
- <span data-ttu-id="35658-111">Microsoft 365 组中的[对话][]。</span><span class="sxs-lookup"><span data-stu-id="35658-111">A [conversation][] in a Microsoft 365 group.</span></span>
- <span data-ttu-id="35658-112">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容。</span><span class="sxs-lookup"><span data-stu-id="35658-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive.</span></span>
- <span data-ttu-id="35658-113">SharePoint [site][]下的[list][]。</span><span class="sxs-lookup"><span data-stu-id="35658-113">A [list][] under a SharePoint [site][].</span></span>
- <span data-ttu-id="35658-114">Outlook 中的[邮件][]、[事件][]或[联系人][]。</span><span class="sxs-lookup"><span data-stu-id="35658-114">A [message][], [event][], or [contact][] in Outlook.</span></span>
- <span data-ttu-id="35658-115">[打印机][] (当打印机的打印作业进入”JobFetchable”状态时 - 准备好提取打印) 和通用打印中的 [printTaskDefinition][]。</span><span class="sxs-lookup"><span data-stu-id="35658-115">A [printer][] (when a print job for the printer gets to JobFetchable state - ready to be fetched for printing) and a [printTaskDefinition][] in Universal Print.</span></span> <span data-ttu-id="35658-116">有关详细信息，请参阅 [订阅云打印 API 中的更改通知](/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="35658-116">For more information, see [Subscribe to change notifications from cloud printing APIs](/graph/universal-print-webhook-notifications).</span></span>
- <span data-ttu-id="35658-117">Azure Active Directory 中的[用户][]或[组][]。</span><span class="sxs-lookup"><span data-stu-id="35658-117">A [user][] or [group][] in Azure Active Directory.</span></span>

<span data-ttu-id="35658-118">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="35658-118">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="35658-119">方法</span><span class="sxs-lookup"><span data-stu-id="35658-119">Methods</span></span>

| <span data-ttu-id="35658-120">方法</span><span class="sxs-lookup"><span data-stu-id="35658-120">Method</span></span> | <span data-ttu-id="35658-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="35658-121">Return Type</span></span> | <span data-ttu-id="35658-122">说明</span><span class="sxs-lookup"><span data-stu-id="35658-122">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="35658-123">创建订阅</span><span class="sxs-lookup"><span data-stu-id="35658-123">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="35658-124">订阅</span><span class="sxs-lookup"><span data-stu-id="35658-124">subscription</span></span>](subscription.md) | <span data-ttu-id="35658-125">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="35658-125">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="35658-126">更新订阅</span><span class="sxs-lookup"><span data-stu-id="35658-126">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="35658-127">订阅</span><span class="sxs-lookup"><span data-stu-id="35658-127">subscription</span></span>](subscription.md) | <span data-ttu-id="35658-128">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="35658-128">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="35658-129">列出订阅</span><span class="sxs-lookup"><span data-stu-id="35658-129">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="35658-130">订阅</span><span class="sxs-lookup"><span data-stu-id="35658-130">subscription</span></span>](subscription.md) | <span data-ttu-id="35658-131">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="35658-131">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="35658-132">获取订阅</span><span class="sxs-lookup"><span data-stu-id="35658-132">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="35658-133">订阅</span><span class="sxs-lookup"><span data-stu-id="35658-133">subscription</span></span>](subscription.md) | <span data-ttu-id="35658-134">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35658-134">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="35658-135">删除订阅</span><span class="sxs-lookup"><span data-stu-id="35658-135">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="35658-136">无</span><span class="sxs-lookup"><span data-stu-id="35658-136">None</span></span> | <span data-ttu-id="35658-137">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="35658-137">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35658-138">属性</span><span class="sxs-lookup"><span data-stu-id="35658-138">Properties</span></span>

| <span data-ttu-id="35658-139">属性</span><span class="sxs-lookup"><span data-stu-id="35658-139">Property</span></span> | <span data-ttu-id="35658-140">类型</span><span class="sxs-lookup"><span data-stu-id="35658-140">Type</span></span> | <span data-ttu-id="35658-141">说明</span><span class="sxs-lookup"><span data-stu-id="35658-141">Description</span></span> | <span data-ttu-id="35658-142">支持的资源</span><span class="sxs-lookup"><span data-stu-id="35658-142">Supported Resources</span></span> |
|:---------|:-----|:------------|:--------------|
| <span data-ttu-id="35658-143">changeType</span><span class="sxs-lookup"><span data-stu-id="35658-143">changeType</span></span> | <span data-ttu-id="35658-144">string</span><span class="sxs-lookup"><span data-stu-id="35658-144">string</span></span> | <span data-ttu-id="35658-145">必填。</span><span class="sxs-lookup"><span data-stu-id="35658-145">Required.</span></span> <span data-ttu-id="35658-146">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="35658-146">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="35658-147">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="35658-147">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="35658-148">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="35658-148">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="35658-149">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="35658-149">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="35658-150">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="35658-150">User and group change notifications support `updated` and `deleted` changeType.</span></span> | <span data-ttu-id="35658-151">全部</span><span class="sxs-lookup"><span data-stu-id="35658-151">All</span></span> |
| <span data-ttu-id="35658-152">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="35658-152">notificationUrl</span></span> | <span data-ttu-id="35658-153">string</span><span class="sxs-lookup"><span data-stu-id="35658-153">string</span></span> | <span data-ttu-id="35658-154">必填。</span><span class="sxs-lookup"><span data-stu-id="35658-154">Required.</span></span> <span data-ttu-id="35658-155">将接收变更通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="35658-155">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="35658-156">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="35658-156">This URL must make use of the HTTPS protocol.</span></span> | <span data-ttu-id="35658-157">全部</span><span class="sxs-lookup"><span data-stu-id="35658-157">All</span></span> |
| <span data-ttu-id="35658-158">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="35658-158">lifecycleNotificationUrl</span></span> | <span data-ttu-id="35658-159">string</span><span class="sxs-lookup"><span data-stu-id="35658-159">string</span></span> | <span data-ttu-id="35658-160">接收生命周期通知（包括 `subscriptionRemoved` 和 `missed` 通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="35658-160">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="35658-161">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="35658-161">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="35658-162">可选。</span><span class="sxs-lookup"><span data-stu-id="35658-162">Optional.</span></span> <br><br><span data-ttu-id="35658-163">[阅读](/graph/webhooks-lifecycle)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="35658-163">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> | <span data-ttu-id="35658-164">全部</span><span class="sxs-lookup"><span data-stu-id="35658-164">All</span></span> |
| <span data-ttu-id="35658-165">resource</span><span class="sxs-lookup"><span data-stu-id="35658-165">resource</span></span> | <span data-ttu-id="35658-166">string</span><span class="sxs-lookup"><span data-stu-id="35658-166">string</span></span> | <span data-ttu-id="35658-167">必需。</span><span class="sxs-lookup"><span data-stu-id="35658-167">Required.</span></span> <span data-ttu-id="35658-168">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="35658-168">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="35658-169">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="35658-169">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="35658-170">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="35658-170">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>| <span data-ttu-id="35658-171">全部</span><span class="sxs-lookup"><span data-stu-id="35658-171">All</span></span> |
| <span data-ttu-id="35658-172">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="35658-172">expirationDateTime</span></span> | [<span data-ttu-id="35658-173">dateTime</span><span class="sxs-lookup"><span data-stu-id="35658-173">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="35658-174">必需。</span><span class="sxs-lookup"><span data-stu-id="35658-174">Required.</span></span> <span data-ttu-id="35658-175">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35658-175">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="35658-176">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="35658-176">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="35658-177">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="35658-177">See the table below for maximum supported subscription length of time.</span></span> | <span data-ttu-id="35658-178">全部</span><span class="sxs-lookup"><span data-stu-id="35658-178">All</span></span> |
| <span data-ttu-id="35658-179">clientState</span><span class="sxs-lookup"><span data-stu-id="35658-179">clientState</span></span> | <span data-ttu-id="35658-180">string</span><span class="sxs-lookup"><span data-stu-id="35658-180">string</span></span> | <span data-ttu-id="35658-181">可选。</span><span class="sxs-lookup"><span data-stu-id="35658-181">Optional.</span></span> <span data-ttu-id="35658-182">指定服务为每个变更通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="35658-182">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="35658-183">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="35658-183">The maximum length is 128 characters.</span></span> <span data-ttu-id="35658-184">通过对比与订阅一起发送的 `clientState` 属性值和与每个变更通知一起接收的 `clientState` 属性值，客户端可以检查变更通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="35658-184">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> | <span data-ttu-id="35658-185">全部</span><span class="sxs-lookup"><span data-stu-id="35658-185">All</span></span> |
| <span data-ttu-id="35658-186">id</span><span class="sxs-lookup"><span data-stu-id="35658-186">id</span></span> | <span data-ttu-id="35658-187">string</span><span class="sxs-lookup"><span data-stu-id="35658-187">string</span></span> | <span data-ttu-id="35658-p111">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="35658-p111">Unique identifier for the subscription. Read-only.</span></span> | <span data-ttu-id="35658-190">全部</span><span class="sxs-lookup"><span data-stu-id="35658-190">All</span></span> |
| <span data-ttu-id="35658-191">applicationId</span><span class="sxs-lookup"><span data-stu-id="35658-191">applicationId</span></span> | <span data-ttu-id="35658-192">string</span><span class="sxs-lookup"><span data-stu-id="35658-192">string</span></span> | <span data-ttu-id="35658-p112">用于创建订阅的应用程序的标识符。 只读。</span><span class="sxs-lookup"><span data-stu-id="35658-p112">Identifier of the application used to create the subscription. Read-only.</span></span> | <span data-ttu-id="35658-195">全部</span><span class="sxs-lookup"><span data-stu-id="35658-195">All</span></span> |
| <span data-ttu-id="35658-196">creatorId</span><span class="sxs-lookup"><span data-stu-id="35658-196">creatorId</span></span> | <span data-ttu-id="35658-197">string</span><span class="sxs-lookup"><span data-stu-id="35658-197">string</span></span> | <span data-ttu-id="35658-198">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="35658-198">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="35658-199">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="35658-199">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="35658-200">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="35658-200">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="35658-201">只读。</span><span class="sxs-lookup"><span data-stu-id="35658-201">Read-only.</span></span> | <span data-ttu-id="35658-202">全部</span><span class="sxs-lookup"><span data-stu-id="35658-202">All</span></span> |
| <span data-ttu-id="35658-203">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="35658-203">includeResourceData</span></span> | <span data-ttu-id="35658-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="35658-204">Boolean</span></span> | <span data-ttu-id="35658-205">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="35658-205">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="35658-206">可选。</span><span class="sxs-lookup"><span data-stu-id="35658-206">Optional.</span></span> | <span data-ttu-id="35658-207">全部</span><span class="sxs-lookup"><span data-stu-id="35658-207">All</span></span> |
| <span data-ttu-id="35658-208">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="35658-208">encryptionCertificate</span></span> | <span data-ttu-id="35658-209">string</span><span class="sxs-lookup"><span data-stu-id="35658-209">string</span></span> | <span data-ttu-id="35658-210">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="35658-210">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="35658-211">可选。</span><span class="sxs-lookup"><span data-stu-id="35658-211">Optional.</span></span> <span data-ttu-id="35658-212">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="35658-212">Required when **includeResourceData** is true.</span></span> | <span data-ttu-id="35658-213">全部</span><span class="sxs-lookup"><span data-stu-id="35658-213">All</span></span> |
| <span data-ttu-id="35658-214">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="35658-214">encryptionCertificateId</span></span> | <span data-ttu-id="35658-215">string</span><span class="sxs-lookup"><span data-stu-id="35658-215">string</span></span> | <span data-ttu-id="35658-p116">应用程序提供的自定义标识符，以帮助识别解密资源数据所需的证书。 可选的。</span><span class="sxs-lookup"><span data-stu-id="35658-p116">A custom app-provided identifier to help identify the certificate needed to decrypt resource data. Optional.</span></span>| <span data-ttu-id="35658-218">全部</span><span class="sxs-lookup"><span data-stu-id="35658-218">All</span></span> |
| <span data-ttu-id="35658-219">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="35658-219">latestSupportedTlsVersion</span></span> | <span data-ttu-id="35658-220">字符串</span><span class="sxs-lookup"><span data-stu-id="35658-220">String</span></span> | <span data-ttu-id="35658-221">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="35658-221">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="35658-222">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="35658-222">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="35658-223">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="35658-223">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="35658-224">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="35658-224">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="35658-225">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="35658-225">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="35658-226">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="35658-226">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> | <span data-ttu-id="35658-227">全部</span><span class="sxs-lookup"><span data-stu-id="35658-227">All</span></span> |
| <span data-ttu-id="35658-228">notificationContentType</span><span class="sxs-lookup"><span data-stu-id="35658-228">notificationContentType</span></span> | <span data-ttu-id="35658-229">字符串</span><span class="sxs-lookup"><span data-stu-id="35658-229">string</span></span> | <span data-ttu-id="35658-230">MS Graph 所需的内容类型为更改支持的资源类型变更通知。</span><span class="sxs-lookup"><span data-stu-id="35658-230">Desired content-type for MS Graph change notifications for supported resource types.</span></span> <span data-ttu-id="35658-231">默认内容类型为“application/json”内容类型。</span><span class="sxs-lookup"><span data-stu-id="35658-231">The default content-type is the "application/json" content-type.</span></span> | <span data-ttu-id="35658-232">全部</span><span class="sxs-lookup"><span data-stu-id="35658-232">All</span></span> |
| <span data-ttu-id="35658-233">notificationQueryOptions</span><span class="sxs-lookup"><span data-stu-id="35658-233">notificationQueryOptions</span></span> | <span data-ttu-id="35658-234">字符串</span><span class="sxs-lookup"><span data-stu-id="35658-234">string</span></span> | <span data-ttu-id="35658-235">用于指定目标资源值的 OData 查询选项。</span><span class="sxs-lookup"><span data-stu-id="35658-235">OData Query Options for specifying value for the targeting resource.</span></span> <span data-ttu-id="35658-236">当资源达到与此处所提供的查询选项相匹配的状态时，客户端会收到通知。</span><span class="sxs-lookup"><span data-stu-id="35658-236">Clients receive notifications when resource reaches the state matching the query options provided here.</span></span> <span data-ttu-id="35658-237">有了订阅创建有效负载中的新属性以及所有现有属性后，每当资源达到 “notificationQueryOptions” 属性中提到的所需状态时，Webhook 就会发送通知，例如当打印作业完成时、当打印作业资源 `isFetchable` 属性值变为 true 时，等等。</span><span class="sxs-lookup"><span data-stu-id="35658-237">With this new property in the subscription creation payload along with all existing properties, Webhooks will deliver notifications whenever a resource reaches the desired state mentioned in the notificationQueryOptions property eg  when the print job is completed, when a print job resource `isFetchable` property value becomes true etc.</span></span> | [<span data-ttu-id="35658-238">通用打印服务</span><span class="sxs-lookup"><span data-stu-id="35658-238">Universal Print Service</span></span>](/graph/universal-print-webhook-notifications) |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="35658-239">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="35658-239">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="35658-240">Resource</span><span class="sxs-lookup"><span data-stu-id="35658-240">Resource</span></span>            | <span data-ttu-id="35658-241">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="35658-241">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="35658-242">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="35658-242">Security **alert**</span></span>     | <span data-ttu-id="35658-243">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="35658-243">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="35658-244">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="35658-244">Teams **callRecord**</span></span>    | <span data-ttu-id="35658-245">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="35658-245">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="35658-246">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="35658-246">Teams **chatMessage**</span></span>    | <span data-ttu-id="35658-247">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="35658-247">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="35658-248">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="35658-248">Group **conversation**</span></span> | <span data-ttu-id="35658-249">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="35658-249">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="35658-250">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="35658-250">OneDrive **driveItem**</span></span>    | <span data-ttu-id="35658-251">42300 分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="35658-251">42300 minutes (under 30 days)</span></span>    |
| <span data-ttu-id="35658-252">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="35658-252">SharePoint **list**</span></span>    | <span data-ttu-id="35658-253">42300 分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="35658-253">42300 minutes (under 30 days)</span></span>    |
| <span data-ttu-id="35658-254">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="35658-254">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="35658-255">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="35658-255">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="35658-256">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="35658-256">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="35658-257">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="35658-257">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="35658-258">打印 **打印机**</span><span class="sxs-lookup"><span data-stu-id="35658-258">Print **printer**</span></span> | <span data-ttu-id="35658-259">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="35658-259">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="35658-260">打印 **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="35658-260">Print **printTaskDefinition**</span></span> | <span data-ttu-id="35658-261">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="35658-261">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="35658-262">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="35658-262">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="35658-263">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="35658-263">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="35658-264">关系</span><span class="sxs-lookup"><span data-stu-id="35658-264">Relationships</span></span>

<span data-ttu-id="35658-265">无</span><span class="sxs-lookup"><span data-stu-id="35658-265">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35658-266">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35658-266">JSON representation</span></span>

<span data-ttu-id="35658-267">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35658-267">Here is a JSON representation of the resource.</span></span>

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

