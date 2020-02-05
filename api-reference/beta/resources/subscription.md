---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d16e312037b79e550f4cf7b5c2e9aa4806e049d2
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774490"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="2580c-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="2580c-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2580c-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="2580c-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="2580c-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="2580c-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="2580c-107">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="2580c-107">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="2580c-108">通过 Microsoft 团队中的团队或频道发送的[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="2580c-108">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="2580c-109">Office 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="2580c-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="2580c-110">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="2580c-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="2580c-111">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="2580c-111">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="2580c-112">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="2580c-112">A [user][] or [group][] in Azure Active Directory</span></span>

## <a name="methods"></a><span data-ttu-id="2580c-113">方法</span><span class="sxs-lookup"><span data-stu-id="2580c-113">Methods</span></span>

| <span data-ttu-id="2580c-114">方法</span><span class="sxs-lookup"><span data-stu-id="2580c-114">Method</span></span> | <span data-ttu-id="2580c-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="2580c-115">Return Type</span></span> | <span data-ttu-id="2580c-116">说明</span><span class="sxs-lookup"><span data-stu-id="2580c-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="2580c-117">创建订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="2580c-118">订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-118">subscription</span></span>](subscription.md) | <span data-ttu-id="2580c-119">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="2580c-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="2580c-120">更新订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="2580c-121">订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-121">subscription</span></span>](subscription.md) | <span data-ttu-id="2580c-122">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="2580c-122">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="2580c-123">列出订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="2580c-124">订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-124">subscription</span></span>](subscription.md) | <span data-ttu-id="2580c-125">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="2580c-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="2580c-126">获取订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="2580c-127">订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-127">subscription</span></span>](subscription.md) | <span data-ttu-id="2580c-128">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2580c-128">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="2580c-129">删除订阅</span><span class="sxs-lookup"><span data-stu-id="2580c-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="2580c-130">无</span><span class="sxs-lookup"><span data-stu-id="2580c-130">None</span></span> | <span data-ttu-id="2580c-131">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="2580c-131">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2580c-132">属性</span><span class="sxs-lookup"><span data-stu-id="2580c-132">Properties</span></span>

| <span data-ttu-id="2580c-133">属性</span><span class="sxs-lookup"><span data-stu-id="2580c-133">Property</span></span> | <span data-ttu-id="2580c-134">类型</span><span class="sxs-lookup"><span data-stu-id="2580c-134">Type</span></span> | <span data-ttu-id="2580c-135">说明</span><span class="sxs-lookup"><span data-stu-id="2580c-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="2580c-136">changeType</span><span class="sxs-lookup"><span data-stu-id="2580c-136">changeType</span></span> | <span data-ttu-id="2580c-137">string</span><span class="sxs-lookup"><span data-stu-id="2580c-137">string</span></span> | <span data-ttu-id="2580c-138">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="2580c-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="2580c-139">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="2580c-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="2580c-140">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="2580c-140">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="2580c-141">必填。</span><span class="sxs-lookup"><span data-stu-id="2580c-141">Required.</span></span> <br><br><span data-ttu-id="2580c-142">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="2580c-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="2580c-143">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="2580c-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="2580c-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="2580c-144">notificationUrl</span></span> | <span data-ttu-id="2580c-145">string</span><span class="sxs-lookup"><span data-stu-id="2580c-145">string</span></span> | <span data-ttu-id="2580c-146">接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="2580c-146">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="2580c-147">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="2580c-147">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="2580c-148">必填。</span><span class="sxs-lookup"><span data-stu-id="2580c-148">Required.</span></span> |
| <span data-ttu-id="2580c-149">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="2580c-149">lifecycleNotificationUrl</span></span> | <span data-ttu-id="2580c-150">string</span><span class="sxs-lookup"><span data-stu-id="2580c-150">string</span></span> | <span data-ttu-id="2580c-151">接收生命周期通知（包括`subscriptionRemoved`和`missed`通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="2580c-151">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="2580c-152">如果未提供，这些通知将传递给**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="2580c-152">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="2580c-153">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="2580c-153">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="2580c-154">可选。</span><span class="sxs-lookup"><span data-stu-id="2580c-154">Optional.</span></span> <br><br><span data-ttu-id="2580c-155">[阅读](/graph/webhooks-outlook-authz)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2580c-155">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="2580c-156">resource</span><span class="sxs-lookup"><span data-stu-id="2580c-156">resource</span></span> | <span data-ttu-id="2580c-157">string</span><span class="sxs-lookup"><span data-stu-id="2580c-157">string</span></span> | <span data-ttu-id="2580c-158">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="2580c-158">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="2580c-159">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="2580c-159">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="2580c-160">必填。</span><span class="sxs-lookup"><span data-stu-id="2580c-160">Required.</span></span> |
| <span data-ttu-id="2580c-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2580c-161">expirationDateTime</span></span> | <span data-ttu-id="2580c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2580c-162">DateTimeOffset</span></span> | <span data-ttu-id="2580c-163">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2580c-163">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="2580c-164">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="2580c-164">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="2580c-165">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="2580c-165">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="2580c-166">必填。</span><span class="sxs-lookup"><span data-stu-id="2580c-166">Required.</span></span> |
| <span data-ttu-id="2580c-167">clientState</span><span class="sxs-lookup"><span data-stu-id="2580c-167">clientState</span></span> | <span data-ttu-id="2580c-168">string</span><span class="sxs-lookup"><span data-stu-id="2580c-168">string</span></span> | <span data-ttu-id="2580c-169">指定每个通知中由服务发送的**clientState**属性的值。</span><span class="sxs-lookup"><span data-stu-id="2580c-169">Specifies the value of the **clientState** property sent by the service in each notification.</span></span> <span data-ttu-id="2580c-170">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="2580c-170">The maximum length is 255 characters.</span></span> <span data-ttu-id="2580c-171">客户端可以通过将随订阅发送的**clientState**属性的值与每个通知收到的**clientState**属性的值进行比较，来检查该通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="2580c-171">The client can check that the notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each notification.</span></span> <span data-ttu-id="2580c-172">可选。</span><span class="sxs-lookup"><span data-stu-id="2580c-172">Optional.</span></span> |
| <span data-ttu-id="2580c-173">id</span><span class="sxs-lookup"><span data-stu-id="2580c-173">id</span></span> | <span data-ttu-id="2580c-174">字符串</span><span class="sxs-lookup"><span data-stu-id="2580c-174">string</span></span> | <span data-ttu-id="2580c-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2580c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="2580c-177">applicationId</span><span class="sxs-lookup"><span data-stu-id="2580c-177">applicationId</span></span> | <span data-ttu-id="2580c-178">string</span><span class="sxs-lookup"><span data-stu-id="2580c-178">string</span></span> | <span data-ttu-id="2580c-179">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="2580c-179">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="2580c-180">只读。</span><span class="sxs-lookup"><span data-stu-id="2580c-180">Read-only.</span></span> |
| <span data-ttu-id="2580c-181">creatorId</span><span class="sxs-lookup"><span data-stu-id="2580c-181">creatorId</span></span> | <span data-ttu-id="2580c-182">string</span><span class="sxs-lookup"><span data-stu-id="2580c-182">string</span></span> | <span data-ttu-id="2580c-183">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="2580c-183">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="2580c-184">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="2580c-184">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="2580c-185">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="2580c-185">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="2580c-186">只读。</span><span class="sxs-lookup"><span data-stu-id="2580c-186">Read-only.</span></span> |
| <span data-ttu-id="2580c-187">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="2580c-187">includeResourceData</span></span> | <span data-ttu-id="2580c-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="2580c-188">Boolean</span></span> | <span data-ttu-id="2580c-189">当设置为`true`时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（如聊天邮件的内容）。</span><span class="sxs-lookup"><span data-stu-id="2580c-189">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="2580c-190">可选。</span><span class="sxs-lookup"><span data-stu-id="2580c-190">Optional.</span></span> | 
| <span data-ttu-id="2580c-191">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="2580c-191">encryptionCertificate</span></span> | <span data-ttu-id="2580c-192">string</span><span class="sxs-lookup"><span data-stu-id="2580c-192">string</span></span> | <span data-ttu-id="2580c-193">具有用于在通知中对资源数据进行加密的公钥的证书的 base64 编码表示形式。</span><span class="sxs-lookup"><span data-stu-id="2580c-193">A base64-encoded representation of a certificate with a public key used to encrypt resource data in notifications.</span></span> <span data-ttu-id="2580c-194">可选。</span><span class="sxs-lookup"><span data-stu-id="2580c-194">Optional.</span></span> <span data-ttu-id="2580c-195">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="2580c-195">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="2580c-196">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="2580c-196">encryptionCertificateId</span></span> | <span data-ttu-id="2580c-197">string</span><span class="sxs-lookup"><span data-stu-id="2580c-197">string</span></span> | <span data-ttu-id="2580c-198">自定义应用程序提供的标识符，用于帮助确定解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="2580c-198">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="2580c-199">可选。</span><span class="sxs-lookup"><span data-stu-id="2580c-199">Optional.</span></span> <span data-ttu-id="2580c-200">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="2580c-200">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="2580c-201">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="2580c-201">latestSupportedTlsVersion</span></span> | <span data-ttu-id="2580c-202">String</span><span class="sxs-lookup"><span data-stu-id="2580c-202">String</span></span> | <span data-ttu-id="2580c-203">指定通知终结点支持的最新 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="2580c-203">Specifies the latest TLS version that the notification endpoint supports.</span></span> <span data-ttu-id="2580c-204">允许订阅者在有限的时间段内使用已弃用的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="2580c-204">Allows subscribers to use a deprecated version of TLS for a limited period.</span></span> <span data-ttu-id="2580c-205">可能的值： **v1_0**、 **v1_1**、 **v1_2**、 **v1_3**。</span><span class="sxs-lookup"><span data-stu-id="2580c-205">Possible values: **v1_0**, **v1_1**, **v1_2**, **v1_3**.</span></span> <span data-ttu-id="2580c-206">可选，默认值为 v1_2。</span><span class="sxs-lookup"><span data-stu-id="2580c-206">Optional, defaults to v1_2.</span></span> <span data-ttu-id="2580c-207">如果客户端终结点支持 TLS 1.2 或更高，则此属性不是必需的。</span><span class="sxs-lookup"><span data-stu-id="2580c-207">If the client endpoint supports TLS 1.2 or above this property is not needed.</span></span> <span data-ttu-id="2580c-208">如果客户端终结点仅支持 TLS 1.0 或1.1，则应将此属性设置为相应的版本，否则操作将失败。</span><span class="sxs-lookup"><span data-stu-id="2580c-208">If the client endpoint supports only TLS 1.0 or 1.1, this property should be set to the corresponding version or the operation will fail.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="2580c-209">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="2580c-209">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="2580c-210">资源</span><span class="sxs-lookup"><span data-stu-id="2580c-210">Resource</span></span>            | <span data-ttu-id="2580c-211">最长过期时间</span><span class="sxs-lookup"><span data-stu-id="2580c-211">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="2580c-212">安全**警报**</span><span class="sxs-lookup"><span data-stu-id="2580c-212">Security **alert**</span></span>     | <span data-ttu-id="2580c-213">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="2580c-213">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="2580c-214">团队**了 chatmessage**</span><span class="sxs-lookup"><span data-stu-id="2580c-214">Teams **chatMessage**</span></span>    | <span data-ttu-id="2580c-215">60分钟（1小时）</span><span class="sxs-lookup"><span data-stu-id="2580c-215">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="2580c-216">组**对话**</span><span class="sxs-lookup"><span data-stu-id="2580c-216">Group **conversation**</span></span> | <span data-ttu-id="2580c-217">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2580c-217">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2580c-218">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="2580c-218">OneDrive **driveItem**</span></span>    | <span data-ttu-id="2580c-219">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2580c-219">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2580c-220">Outlook**邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="2580c-220">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="2580c-221">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2580c-221">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2580c-222">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="2580c-222">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="2580c-223">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="2580c-223">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="2580c-224">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="2580c-224">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="2580c-225">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="2580c-225">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="2580c-226">关系</span><span class="sxs-lookup"><span data-stu-id="2580c-226">Relationships</span></span>

<span data-ttu-id="2580c-227">无。</span><span class="sxs-lookup"><span data-stu-id="2580c-227">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2580c-228">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2580c-228">JSON representation</span></span>

<span data-ttu-id="2580c-229">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2580c-229">Here is a JSON representation of the resource.</span></span>

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

[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
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
