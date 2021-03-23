---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 81bb0e1b914a547b8c9fef55b446158069b77b23
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51030972"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="af3ac-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="af3ac-104">subscription resource type</span></span>

<span data-ttu-id="af3ac-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af3ac-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af3ac-106">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。</span><span class="sxs-lookup"><span data-stu-id="af3ac-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="af3ac-107">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="af3ac-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="af3ac-108">来自[][] Microsoft Graph 安全性 API 的警报。</span><span class="sxs-lookup"><span data-stu-id="af3ac-108">An [alert][] from the Microsoft Graph Security API.</span></span>
- <span data-ttu-id="af3ac-109">在 Microsoft Teams 中的通话或会议之后生成的[callRecord。][]</span><span class="sxs-lookup"><span data-stu-id="af3ac-109">A [callRecord][] produced after a call or meeting in Microsoft Teams.</span></span>
- <span data-ttu-id="af3ac-110">通过 Microsoft Teams 中的团队或频道发送的[chatMessage。][]</span><span class="sxs-lookup"><span data-stu-id="af3ac-110">A [chatMessage][] sent via teams or channels in Microsoft Teams.</span></span>
- <span data-ttu-id="af3ac-111">Microsoft [][] 365 组的对话。</span><span class="sxs-lookup"><span data-stu-id="af3ac-111">A [conversation][] in a Microsoft 365 group.</span></span>
- <span data-ttu-id="af3ac-112">OneDrive for Business 中根文件夹 [driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中根文件夹或子文件夹 [driveItem][] 的层次结构中的内容。</span><span class="sxs-lookup"><span data-stu-id="af3ac-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive.</span></span>
- <span data-ttu-id="af3ac-113">[SharePoint][]网站 下[的列表][]。</span><span class="sxs-lookup"><span data-stu-id="af3ac-113">A [list][] under a SharePoint [site][].</span></span>
- <span data-ttu-id="af3ac-114">Outlook[][]中的[邮件][]、[事件或][]联系人。</span><span class="sxs-lookup"><span data-stu-id="af3ac-114">A [message][], [event][], or [contact][] in Outlook.</span></span>
- <span data-ttu-id="af3ac-115">Microsoft [][] Teams 中的用户状态。</span><span class="sxs-lookup"><span data-stu-id="af3ac-115">The [presence][] of a user in Microsoft Teams.</span></span>
- <span data-ttu-id="af3ac-116">Azure [][] Active Directory[中的用户][]或组。</span><span class="sxs-lookup"><span data-stu-id="af3ac-116">A [user][] or [group][] in Azure Active Directory.</span></span>
- <span data-ttu-id="af3ac-117">当[ (][]的打印作业进入 JobFetchable 状态时，打印机会进行打印- 准备在通用打印中) 打印和[printTaskDefinition。][]</span><span class="sxs-lookup"><span data-stu-id="af3ac-117">A [printer][] (when a print job for the printer gets to JobFetchable state - ready to be fetched for printing) and a [printTaskDefinition][] in Universal Print.</span></span> <span data-ttu-id="af3ac-118">有关详细信息，请参阅订阅 [以从云打印 API 更改通知](https://docs.microsoft.com/en-us/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="af3ac-118">For more information, see [Subscribe to change notifications from cloud printing APIs](https://docs.microsoft.com/en-us/graph/universal-print-webhook-notifications).</span></span>
- <span data-ttu-id="af3ac-119">Microsoft To Do 中的用户的[todoTask。][]</span><span class="sxs-lookup"><span data-stu-id="af3ac-119">A [todoTask][] of a user in Microsoft To Do.</span></span>

<span data-ttu-id="af3ac-120">查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。</span><span class="sxs-lookup"><span data-stu-id="af3ac-120">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="af3ac-121">方法</span><span class="sxs-lookup"><span data-stu-id="af3ac-121">Methods</span></span>

| <span data-ttu-id="af3ac-122">方法</span><span class="sxs-lookup"><span data-stu-id="af3ac-122">Method</span></span> | <span data-ttu-id="af3ac-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="af3ac-123">Return Type</span></span> | <span data-ttu-id="af3ac-124">说明</span><span class="sxs-lookup"><span data-stu-id="af3ac-124">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="af3ac-125">创建订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-125">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="af3ac-126">订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-126">subscription</span></span>](subscription.md) | <span data-ttu-id="af3ac-127">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。</span><span class="sxs-lookup"><span data-stu-id="af3ac-127">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="af3ac-128">更新订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-128">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="af3ac-129">订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-129">subscription</span></span>](subscription.md) | <span data-ttu-id="af3ac-130">通过更新其过期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="af3ac-130">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="af3ac-131">列出订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-131">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="af3ac-132">订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-132">subscription</span></span>](subscription.md) | <span data-ttu-id="af3ac-133">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="af3ac-133">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="af3ac-134">获取订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-134">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="af3ac-135">订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-135">subscription</span></span>](subscription.md) | <span data-ttu-id="af3ac-136">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af3ac-136">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="af3ac-137">删除订阅</span><span class="sxs-lookup"><span data-stu-id="af3ac-137">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="af3ac-138">无</span><span class="sxs-lookup"><span data-stu-id="af3ac-138">None</span></span> | <span data-ttu-id="af3ac-139">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="af3ac-139">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="af3ac-140">属性</span><span class="sxs-lookup"><span data-stu-id="af3ac-140">Properties</span></span>

| <span data-ttu-id="af3ac-141">属性</span><span class="sxs-lookup"><span data-stu-id="af3ac-141">Property</span></span> | <span data-ttu-id="af3ac-142">类型</span><span class="sxs-lookup"><span data-stu-id="af3ac-142">Type</span></span> | <span data-ttu-id="af3ac-143">说明</span><span class="sxs-lookup"><span data-stu-id="af3ac-143">Description</span></span> | <span data-ttu-id="af3ac-144">支持的资源</span><span class="sxs-lookup"><span data-stu-id="af3ac-144">Supported Resources</span></span> |
|:---------|:-----|:------------|:--------------|
| <span data-ttu-id="af3ac-145">changeType</span><span class="sxs-lookup"><span data-stu-id="af3ac-145">changeType</span></span> | <span data-ttu-id="af3ac-146">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-146">string</span></span> | <span data-ttu-id="af3ac-147">指示订阅资源中将引发变更通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="af3ac-147">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="af3ac-148">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="af3ac-148">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="af3ac-149">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="af3ac-149">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="af3ac-150">必填。</span><span class="sxs-lookup"><span data-stu-id="af3ac-150">Required.</span></span> <br><br><span data-ttu-id="af3ac-151">注意：驱动器根项和列表变更通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="af3ac-151">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="af3ac-152">用户和组的变更通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="af3ac-152">User and group change notifications support `updated` and `deleted` changeType.</span></span> | <span data-ttu-id="af3ac-153">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-153">All</span></span> |
| <span data-ttu-id="af3ac-154">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="af3ac-154">notificationUrl</span></span> | <span data-ttu-id="af3ac-155">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-155">string</span></span> | <span data-ttu-id="af3ac-156">接收更改通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="af3ac-156">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="af3ac-157">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="af3ac-157">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="af3ac-158">必填。</span><span class="sxs-lookup"><span data-stu-id="af3ac-158">Required.</span></span> | <span data-ttu-id="af3ac-159">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-159">All</span></span> |
| <span data-ttu-id="af3ac-160">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="af3ac-160">lifecycleNotificationUrl</span></span> | <span data-ttu-id="af3ac-161">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-161">string</span></span> | <span data-ttu-id="af3ac-162">接收生命周期通知的终结点的 URL，包括 `subscriptionRemoved` 和 `missed` 通知。</span><span class="sxs-lookup"><span data-stu-id="af3ac-162">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="af3ac-163">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="af3ac-163">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="af3ac-164">可选。</span><span class="sxs-lookup"><span data-stu-id="af3ac-164">Optional.</span></span> <br><br><span data-ttu-id="af3ac-165">[阅读有关](/graph/webhooks-lifecycle) Outlook 资源如何使用生命周期通知的更多信息。</span><span class="sxs-lookup"><span data-stu-id="af3ac-165">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> | <span data-ttu-id="af3ac-166">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-166">All</span></span> |
| <span data-ttu-id="af3ac-167">resource</span><span class="sxs-lookup"><span data-stu-id="af3ac-167">resource</span></span> | <span data-ttu-id="af3ac-168">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-168">string</span></span> | <span data-ttu-id="af3ac-169">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="af3ac-169">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="af3ac-170">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="af3ac-170">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="af3ac-171">查看各支持资源的可能资源路径[值](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="af3ac-171">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="af3ac-172">必填。</span><span class="sxs-lookup"><span data-stu-id="af3ac-172">Required.</span></span> | <span data-ttu-id="af3ac-173">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-173">All</span></span> |
| <span data-ttu-id="af3ac-174">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="af3ac-174">expirationDateTime</span></span> | <span data-ttu-id="af3ac-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af3ac-175">DateTimeOffset</span></span> | <span data-ttu-id="af3ac-176">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af3ac-176">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="af3ac-177">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="af3ac-177">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="af3ac-178">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="af3ac-178">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="af3ac-179">必填。</span><span class="sxs-lookup"><span data-stu-id="af3ac-179">Required.</span></span> | <span data-ttu-id="af3ac-180">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-180">All</span></span> |
| <span data-ttu-id="af3ac-181">clientState</span><span class="sxs-lookup"><span data-stu-id="af3ac-181">clientState</span></span> | <span data-ttu-id="af3ac-182">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-182">string</span></span> | <span data-ttu-id="af3ac-183">指定服务在每个更改通知中发送的 **clientState** 属性的值。</span><span class="sxs-lookup"><span data-stu-id="af3ac-183">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="af3ac-184">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="af3ac-184">The maximum length is 255 characters.</span></span> <span data-ttu-id="af3ac-185">通过比较与订阅一起发送的 **clientState** 属性的值与每个更改通知一起收到的 **clientState** 属性的值，客户端可以检查更改通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="af3ac-185">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="af3ac-186">可选。</span><span class="sxs-lookup"><span data-stu-id="af3ac-186">Optional.</span></span> | <span data-ttu-id="af3ac-187">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-187">All</span></span> |
| <span data-ttu-id="af3ac-188">id</span><span class="sxs-lookup"><span data-stu-id="af3ac-188">id</span></span> | <span data-ttu-id="af3ac-189">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-189">string</span></span> | <span data-ttu-id="af3ac-p111">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="af3ac-p111">Unique identifier for the subscription. Read-only.</span></span> | <span data-ttu-id="af3ac-192">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-192">All</span></span> |
| <span data-ttu-id="af3ac-193">applicationId</span><span class="sxs-lookup"><span data-stu-id="af3ac-193">applicationId</span></span> | <span data-ttu-id="af3ac-194">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-194">string</span></span> | <span data-ttu-id="af3ac-195">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="af3ac-195">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="af3ac-196">只读。</span><span class="sxs-lookup"><span data-stu-id="af3ac-196">Read-only.</span></span> | <span data-ttu-id="af3ac-197">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-197">All</span></span> |
| <span data-ttu-id="af3ac-198">creatorId</span><span class="sxs-lookup"><span data-stu-id="af3ac-198">creatorId</span></span> | <span data-ttu-id="af3ac-199">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-199">string</span></span> | <span data-ttu-id="af3ac-200">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="af3ac-200">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="af3ac-201">如果应用使用委派权限创建订阅，则此字段包含代表应用调用的登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="af3ac-201">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="af3ac-202">如果应用程序使用应用程序权限，则此字段包含与应用程序对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="af3ac-202">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="af3ac-203">只读。</span><span class="sxs-lookup"><span data-stu-id="af3ac-203">Read-only.</span></span> | <span data-ttu-id="af3ac-204">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-204">All</span></span> |
| <span data-ttu-id="af3ac-205">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="af3ac-205">includeResourceData</span></span> | <span data-ttu-id="af3ac-206">布尔值</span><span class="sxs-lookup"><span data-stu-id="af3ac-206">Boolean</span></span> | <span data-ttu-id="af3ac-207">设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。</span><span class="sxs-lookup"><span data-stu-id="af3ac-207">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="af3ac-208">可选。</span><span class="sxs-lookup"><span data-stu-id="af3ac-208">Optional.</span></span> | <span data-ttu-id="af3ac-209">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-209">All</span></span> |
| <span data-ttu-id="af3ac-210">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="af3ac-210">encryptionCertificate</span></span> | <span data-ttu-id="af3ac-211">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-211">string</span></span> | <span data-ttu-id="af3ac-212">带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="af3ac-212">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="af3ac-213">可选。</span><span class="sxs-lookup"><span data-stu-id="af3ac-213">Optional.</span></span> <span data-ttu-id="af3ac-214">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="af3ac-214">Required when **includeResourceData** is true.</span></span> | <span data-ttu-id="af3ac-215">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-215">All</span></span> |
| <span data-ttu-id="af3ac-216">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="af3ac-216">encryptionCertificateId</span></span> | <span data-ttu-id="af3ac-217">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-217">string</span></span> | <span data-ttu-id="af3ac-218">自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="af3ac-218">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="af3ac-219">可选。</span><span class="sxs-lookup"><span data-stu-id="af3ac-219">Optional.</span></span> <span data-ttu-id="af3ac-220">**includeResourceData** 为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="af3ac-220">Required when **includeResourceData** is true.</span></span> | <span data-ttu-id="af3ac-221">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-221">All</span></span> |
| <span data-ttu-id="af3ac-222">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="af3ac-222">latestSupportedTlsVersion</span></span> | <span data-ttu-id="af3ac-223">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-223">string</span></span> | <span data-ttu-id="af3ac-224">指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。</span><span class="sxs-lookup"><span data-stu-id="af3ac-224">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="af3ac-225">可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。</span><span class="sxs-lookup"><span data-stu-id="af3ac-225">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="af3ac-226">对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="af3ac-226">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="af3ac-227">对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。</span><span class="sxs-lookup"><span data-stu-id="af3ac-227">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="af3ac-228">对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="af3ac-228">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="af3ac-229">在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。</span><span class="sxs-lookup"><span data-stu-id="af3ac-229">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> | <span data-ttu-id="af3ac-230">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-230">All</span></span> |
| <span data-ttu-id="af3ac-231">notificationContentType</span><span class="sxs-lookup"><span data-stu-id="af3ac-231">notificationContentType</span></span> | <span data-ttu-id="af3ac-232">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-232">string</span></span> | <span data-ttu-id="af3ac-233">支持的资源类型的 MS Graph 更改通知的所需内容类型。</span><span class="sxs-lookup"><span data-stu-id="af3ac-233">Desired content-type for MS Graph change notifications for supported resource types.</span></span> <span data-ttu-id="af3ac-234">默认内容类型为"application/json"内容类型。</span><span class="sxs-lookup"><span data-stu-id="af3ac-234">The default content-type is the "application/json" content-type.</span></span> | <span data-ttu-id="af3ac-235">全部</span><span class="sxs-lookup"><span data-stu-id="af3ac-235">All</span></span> |
| <span data-ttu-id="af3ac-236">notificationQueryOptions</span><span class="sxs-lookup"><span data-stu-id="af3ac-236">notificationQueryOptions</span></span> | <span data-ttu-id="af3ac-237">string</span><span class="sxs-lookup"><span data-stu-id="af3ac-237">string</span></span> | <span data-ttu-id="af3ac-238">用于指定目标资源值的 OData 查询选项。</span><span class="sxs-lookup"><span data-stu-id="af3ac-238">OData Query Options for specifying value for the targeting resource.</span></span> <span data-ttu-id="af3ac-239">当资源达到与此处提供的查询选项匹配的状态时，客户端将收到通知。</span><span class="sxs-lookup"><span data-stu-id="af3ac-239">Clients receive notifications when resource reaches the state matching the query options provided here.</span></span> <span data-ttu-id="af3ac-240">使用订阅创建有效负载中的这一新属性以及所有现有属性，Webhook 将在资源达到 notificationQueryOptions 属性中提到的所需状态（例如，打印作业完成时、打印作业资源属性值变为 true 等）时发送通知。 `isFetchable`</span><span class="sxs-lookup"><span data-stu-id="af3ac-240">With this new property in the subscription creation payload along with all existing properties, Webhooks will deliver notifications whenever a resource reaches the desired state mentioned in the notificationQueryOptions property eg  when the print job is completed, when a print job resource `isFetchable` property value becomes true etc.</span></span> | [<span data-ttu-id="af3ac-241">通用打印服务</span><span class="sxs-lookup"><span data-stu-id="af3ac-241">Universal Print Service</span></span>](https://docs.microsoft.com/en-us/graph/universal-print-webhook-notifications) |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="af3ac-242">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="af3ac-242">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="af3ac-243">Resource</span><span class="sxs-lookup"><span data-stu-id="af3ac-243">Resource</span></span>            | <span data-ttu-id="af3ac-244">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="af3ac-244">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="af3ac-245">安全 **警报**</span><span class="sxs-lookup"><span data-stu-id="af3ac-245">Security **alert**</span></span>     | <span data-ttu-id="af3ac-246">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-246">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="af3ac-247">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="af3ac-247">Teams **callRecord**</span></span>    | <span data-ttu-id="af3ac-248">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-248">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="af3ac-249">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="af3ac-249">Teams **chatMessage**</span></span>    | <span data-ttu-id="af3ac-250">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="af3ac-250">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="af3ac-251">组 **对话**</span><span class="sxs-lookup"><span data-stu-id="af3ac-251">Group **conversation**</span></span> | <span data-ttu-id="af3ac-252">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-252">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-253">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="af3ac-253">OneDrive **driveItem**</span></span>    | <span data-ttu-id="af3ac-254">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-254">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-255">SharePoint **列表**</span><span class="sxs-lookup"><span data-stu-id="af3ac-255">SharePoint **list**</span></span>    | <span data-ttu-id="af3ac-256">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-256">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-257">Outlook **邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="af3ac-257">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="af3ac-258">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-258">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-259">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="af3ac-259">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="af3ac-260">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-260">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-261">**状态**</span><span class="sxs-lookup"><span data-stu-id="af3ac-261">**presence**</span></span>        | <span data-ttu-id="af3ac-262">60 分钟（1 小时）</span><span class="sxs-lookup"><span data-stu-id="af3ac-262">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="af3ac-263">打印 **打印机**</span><span class="sxs-lookup"><span data-stu-id="af3ac-263">Print **printer**</span></span> | <span data-ttu-id="af3ac-264">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-264">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-265">Print **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="af3ac-265">Print **printTaskDefinition**</span></span> | <span data-ttu-id="af3ac-266">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-266">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af3ac-267">**todoTask**</span><span class="sxs-lookup"><span data-stu-id="af3ac-267">**todoTask**</span></span>              | <span data-ttu-id="af3ac-268">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="af3ac-268">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="af3ac-269">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="af3ac-269">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="af3ac-270">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="af3ac-270">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="af3ac-271">关系</span><span class="sxs-lookup"><span data-stu-id="af3ac-271">Relationships</span></span>

<span data-ttu-id="af3ac-272">无。</span><span class="sxs-lookup"><span data-stu-id="af3ac-272">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af3ac-273">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af3ac-273">JSON representation</span></span>

<span data-ttu-id="af3ac-274">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af3ac-274">Here is a JSON representation of the resource.</span></span>

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


