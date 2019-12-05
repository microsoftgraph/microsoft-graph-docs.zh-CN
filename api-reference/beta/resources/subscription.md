---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: piotrci
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 70af093b6ed782ba7bf447c339e5187439849970
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844265"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="29f7b-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="29f7b-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f7b-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="29f7b-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="29f7b-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="29f7b-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="29f7b-107">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="29f7b-107">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="29f7b-108">通过 Microsoft 团队中的团队或频道发送的[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="29f7b-108">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="29f7b-109">Office 365 组中的[对话][]</span><span class="sxs-lookup"><span data-stu-id="29f7b-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="29f7b-110">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="29f7b-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="29f7b-111">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="29f7b-111">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="29f7b-112">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="29f7b-112">A [user][] or [group][] in Azure Active Directory</span></span>

## <a name="methods"></a><span data-ttu-id="29f7b-113">方法</span><span class="sxs-lookup"><span data-stu-id="29f7b-113">Methods</span></span>

| <span data-ttu-id="29f7b-114">方法</span><span class="sxs-lookup"><span data-stu-id="29f7b-114">Method</span></span> | <span data-ttu-id="29f7b-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="29f7b-115">Return Type</span></span> | <span data-ttu-id="29f7b-116">说明</span><span class="sxs-lookup"><span data-stu-id="29f7b-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="29f7b-117">创建订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="29f7b-118">订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-118">subscription</span></span>](subscription.md) | <span data-ttu-id="29f7b-119">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="29f7b-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="29f7b-120">更新订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="29f7b-121">订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-121">subscription</span></span>](subscription.md) | <span data-ttu-id="29f7b-122">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="29f7b-122">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="29f7b-123">列出订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="29f7b-124">订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-124">subscription</span></span>](subscription.md) | <span data-ttu-id="29f7b-125">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="29f7b-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="29f7b-126">获取订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="29f7b-127">订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-127">subscription</span></span>](subscription.md) | <span data-ttu-id="29f7b-128">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29f7b-128">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="29f7b-129">删除订阅</span><span class="sxs-lookup"><span data-stu-id="29f7b-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="29f7b-130">无</span><span class="sxs-lookup"><span data-stu-id="29f7b-130">None</span></span> | <span data-ttu-id="29f7b-131">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="29f7b-131">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29f7b-132">属性</span><span class="sxs-lookup"><span data-stu-id="29f7b-132">Properties</span></span>

| <span data-ttu-id="29f7b-133">属性</span><span class="sxs-lookup"><span data-stu-id="29f7b-133">Property</span></span> | <span data-ttu-id="29f7b-134">类型</span><span class="sxs-lookup"><span data-stu-id="29f7b-134">Type</span></span> | <span data-ttu-id="29f7b-135">说明</span><span class="sxs-lookup"><span data-stu-id="29f7b-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="29f7b-136">changeType</span><span class="sxs-lookup"><span data-stu-id="29f7b-136">changeType</span></span> | <span data-ttu-id="29f7b-137">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-137">string</span></span> | <span data-ttu-id="29f7b-138">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="29f7b-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="29f7b-139">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="29f7b-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="29f7b-140">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="29f7b-140">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="29f7b-141">必需。</span><span class="sxs-lookup"><span data-stu-id="29f7b-141">Required.</span></span> <br><br><span data-ttu-id="29f7b-142">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="29f7b-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="29f7b-143">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="29f7b-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="29f7b-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="29f7b-144">notificationUrl</span></span> | <span data-ttu-id="29f7b-145">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-145">string</span></span> | <span data-ttu-id="29f7b-146">接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="29f7b-146">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="29f7b-147">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="29f7b-147">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="29f7b-148">必需。</span><span class="sxs-lookup"><span data-stu-id="29f7b-148">Required.</span></span> |
| <span data-ttu-id="29f7b-149">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="29f7b-149">lifecycleNotificationUrl</span></span> | <span data-ttu-id="29f7b-150">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-150">string</span></span> | <span data-ttu-id="29f7b-151">接收生命周期通知（包括`subscriptionRemoved`和`missed`通知）的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="29f7b-151">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="29f7b-152">如果未提供，这些通知将传递给**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="29f7b-152">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="29f7b-153">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="29f7b-153">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="29f7b-154">可选。</span><span class="sxs-lookup"><span data-stu-id="29f7b-154">Optional.</span></span> <br><br><span data-ttu-id="29f7b-155">[阅读](/graph/webhooks-outlook-authz)有关 Outlook 资源如何使用生命周期通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="29f7b-155">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="29f7b-156">resource</span><span class="sxs-lookup"><span data-stu-id="29f7b-156">resource</span></span> | <span data-ttu-id="29f7b-157">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-157">string</span></span> | <span data-ttu-id="29f7b-158">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="29f7b-158">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="29f7b-159">不包含的基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="29f7b-159">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="29f7b-160">必需。</span><span class="sxs-lookup"><span data-stu-id="29f7b-160">Required.</span></span> |
| <span data-ttu-id="29f7b-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="29f7b-161">expirationDateTime</span></span> | <span data-ttu-id="29f7b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f7b-162">DateTimeOffset</span></span> | <span data-ttu-id="29f7b-163">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29f7b-163">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="29f7b-164">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="29f7b-164">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="29f7b-165">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="29f7b-165">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="29f7b-166">必需。</span><span class="sxs-lookup"><span data-stu-id="29f7b-166">Required.</span></span> |
| <span data-ttu-id="29f7b-167">clientState</span><span class="sxs-lookup"><span data-stu-id="29f7b-167">clientState</span></span> | <span data-ttu-id="29f7b-168">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-168">string</span></span> | <span data-ttu-id="29f7b-169">指定每个通知中由服务发送的**clientState**属性的值。</span><span class="sxs-lookup"><span data-stu-id="29f7b-169">Specifies the value of the **clientState** property sent by the service in each notification.</span></span> <span data-ttu-id="29f7b-170">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="29f7b-170">The maximum length is 255 characters.</span></span> <span data-ttu-id="29f7b-171">客户端可以通过将随订阅发送的**clientState**属性的值与每个通知收到的**clientState**属性的值进行比较，来检查该通知是否来自服务。</span><span class="sxs-lookup"><span data-stu-id="29f7b-171">The client can check that the notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each notification.</span></span> <span data-ttu-id="29f7b-172">可选。</span><span class="sxs-lookup"><span data-stu-id="29f7b-172">Optional.</span></span> |
| <span data-ttu-id="29f7b-173">id</span><span class="sxs-lookup"><span data-stu-id="29f7b-173">id</span></span> | <span data-ttu-id="29f7b-174">字符串</span><span class="sxs-lookup"><span data-stu-id="29f7b-174">string</span></span> | <span data-ttu-id="29f7b-p110">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="29f7b-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="29f7b-177">applicationId</span><span class="sxs-lookup"><span data-stu-id="29f7b-177">applicationId</span></span> | <span data-ttu-id="29f7b-178">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-178">string</span></span> | <span data-ttu-id="29f7b-179">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="29f7b-179">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="29f7b-180">只读。</span><span class="sxs-lookup"><span data-stu-id="29f7b-180">Read-only.</span></span> |
| <span data-ttu-id="29f7b-181">creatorId</span><span class="sxs-lookup"><span data-stu-id="29f7b-181">creatorId</span></span> | <span data-ttu-id="29f7b-182">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-182">string</span></span> | <span data-ttu-id="29f7b-183">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="29f7b-183">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="29f7b-184">如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。</span><span class="sxs-lookup"><span data-stu-id="29f7b-184">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="29f7b-185">如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="29f7b-185">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="29f7b-186">只读。</span><span class="sxs-lookup"><span data-stu-id="29f7b-186">Read-only.</span></span> |
| <span data-ttu-id="29f7b-187">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="29f7b-187">includeResourceData</span></span> | <span data-ttu-id="29f7b-188">布尔</span><span class="sxs-lookup"><span data-stu-id="29f7b-188">Boolean</span></span> | <span data-ttu-id="29f7b-189">当设置为`true`时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（如聊天邮件的内容）。</span><span class="sxs-lookup"><span data-stu-id="29f7b-189">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="29f7b-190">可选。</span><span class="sxs-lookup"><span data-stu-id="29f7b-190">Optional.</span></span> | 
| <span data-ttu-id="29f7b-191">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="29f7b-191">encryptionCertificate</span></span> | <span data-ttu-id="29f7b-192">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-192">string</span></span> | <span data-ttu-id="29f7b-193">具有用于在通知中对资源数据进行加密的公钥的证书的 base64 编码表示形式。</span><span class="sxs-lookup"><span data-stu-id="29f7b-193">A base64-encoded representation of a certificate with a public key used to encrypt resource data in notifications.</span></span> <span data-ttu-id="29f7b-194">可选。</span><span class="sxs-lookup"><span data-stu-id="29f7b-194">Optional.</span></span> <span data-ttu-id="29f7b-195">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="29f7b-195">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="29f7b-196">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="29f7b-196">encryptionCertificateId</span></span> | <span data-ttu-id="29f7b-197">string</span><span class="sxs-lookup"><span data-stu-id="29f7b-197">string</span></span> | <span data-ttu-id="29f7b-198">自定义应用程序提供的标识符，用于帮助确定解密资源数据所需的证书。</span><span class="sxs-lookup"><span data-stu-id="29f7b-198">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="29f7b-199">可选。</span><span class="sxs-lookup"><span data-stu-id="29f7b-199">Optional.</span></span> <span data-ttu-id="29f7b-200">当**includeResourceData**为 true 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="29f7b-200">Required when **includeResourceData** is true.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="29f7b-201">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="29f7b-201">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="29f7b-202">资源</span><span class="sxs-lookup"><span data-stu-id="29f7b-202">Resource</span></span>            | <span data-ttu-id="29f7b-203">最长过期时间</span><span class="sxs-lookup"><span data-stu-id="29f7b-203">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="29f7b-204">安全**警报**</span><span class="sxs-lookup"><span data-stu-id="29f7b-204">Security **alert**</span></span>     | <span data-ttu-id="29f7b-205">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="29f7b-205">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="29f7b-206">团队**了 chatmessage**</span><span class="sxs-lookup"><span data-stu-id="29f7b-206">Teams **chatMessage**</span></span>    | <span data-ttu-id="29f7b-207">60分钟（1小时）</span><span class="sxs-lookup"><span data-stu-id="29f7b-207">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="29f7b-208">组**对话**</span><span class="sxs-lookup"><span data-stu-id="29f7b-208">Group **conversation**</span></span> | <span data-ttu-id="29f7b-209">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="29f7b-209">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="29f7b-210">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="29f7b-210">OneDrive **driveItem**</span></span>    | <span data-ttu-id="29f7b-211">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="29f7b-211">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="29f7b-212">Outlook**邮件**、**事件**、**联系人**</span><span class="sxs-lookup"><span data-stu-id="29f7b-212">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="29f7b-213">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="29f7b-213">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="29f7b-214">**用户**、**组**、其他目录资源</span><span class="sxs-lookup"><span data-stu-id="29f7b-214">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="29f7b-215">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="29f7b-215">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="29f7b-216">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="29f7b-216">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="29f7b-217">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="29f7b-217">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="29f7b-218">关系</span><span class="sxs-lookup"><span data-stu-id="29f7b-218">Relationships</span></span>

<span data-ttu-id="29f7b-219">无。</span><span class="sxs-lookup"><span data-stu-id="29f7b-219">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29f7b-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29f7b-220">JSON representation</span></span>

<span data-ttu-id="29f7b-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29f7b-221">Here is a JSON representation of the resource.</span></span>

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
  "encryptionCertificateId": "string"
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
