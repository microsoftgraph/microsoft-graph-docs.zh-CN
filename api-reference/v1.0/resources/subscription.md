---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ebd12c5876ae9bb580ac8466eeb88341bb1a0ae4
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774917"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="55b7e-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="55b7e-104">subscription resource type</span></span>

<span data-ttu-id="55b7e-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="55b7e-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="55b7e-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="55b7e-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="55b7e-107">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="55b7e-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="55b7e-108">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="55b7e-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="55b7e-109">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="55b7e-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="55b7e-110">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="55b7e-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="55b7e-111">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="55b7e-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="methods"></a><span data-ttu-id="55b7e-112">方法</span><span class="sxs-lookup"><span data-stu-id="55b7e-112">Methods</span></span>

| <span data-ttu-id="55b7e-113">方法</span><span class="sxs-lookup"><span data-stu-id="55b7e-113">Method</span></span> | <span data-ttu-id="55b7e-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="55b7e-114">Return Type</span></span> | <span data-ttu-id="55b7e-115">说明</span><span class="sxs-lookup"><span data-stu-id="55b7e-115">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="55b7e-116">创建订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-116">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="55b7e-117">订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-117">subscription</span></span>](subscription.md) | <span data-ttu-id="55b7e-118">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="55b7e-118">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="55b7e-119">更新订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-119">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="55b7e-120">订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-120">subscription</span></span>](subscription.md) | <span data-ttu-id="55b7e-121">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="55b7e-121">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="55b7e-122">列出订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-122">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="55b7e-123">订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-123">subscription</span></span>](subscription.md) | <span data-ttu-id="55b7e-124">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="55b7e-124">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="55b7e-125">获取订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-125">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="55b7e-126">订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-126">subscription</span></span>](subscription.md) | <span data-ttu-id="55b7e-127">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55b7e-127">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="55b7e-128">删除订阅</span><span class="sxs-lookup"><span data-stu-id="55b7e-128">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="55b7e-129">无</span><span class="sxs-lookup"><span data-stu-id="55b7e-129">None</span></span> | <span data-ttu-id="55b7e-130">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="55b7e-130">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="55b7e-131">属性</span><span class="sxs-lookup"><span data-stu-id="55b7e-131">Properties</span></span>

| <span data-ttu-id="55b7e-132">属性</span><span class="sxs-lookup"><span data-stu-id="55b7e-132">Property</span></span> | <span data-ttu-id="55b7e-133">类型</span><span class="sxs-lookup"><span data-stu-id="55b7e-133">Type</span></span> | <span data-ttu-id="55b7e-134">说明</span><span class="sxs-lookup"><span data-stu-id="55b7e-134">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="55b7e-135">changeType</span><span class="sxs-lookup"><span data-stu-id="55b7e-135">changeType</span></span> | <span data-ttu-id="55b7e-136">string</span><span class="sxs-lookup"><span data-stu-id="55b7e-136">string</span></span> | <span data-ttu-id="55b7e-137">必需。</span><span class="sxs-lookup"><span data-stu-id="55b7e-137">Required.</span></span> <span data-ttu-id="55b7e-138">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="55b7e-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="55b7e-139">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="55b7e-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="55b7e-140">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="55b7e-140">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="55b7e-141">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="55b7e-141">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="55b7e-142">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="55b7e-142">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="55b7e-143">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="55b7e-143">notificationUrl</span></span> | <span data-ttu-id="55b7e-144">string</span><span class="sxs-lookup"><span data-stu-id="55b7e-144">string</span></span> | <span data-ttu-id="55b7e-145">必需。</span><span class="sxs-lookup"><span data-stu-id="55b7e-145">Required.</span></span> <span data-ttu-id="55b7e-146">将接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="55b7e-146">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="55b7e-147">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="55b7e-147">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="55b7e-148">resource</span><span class="sxs-lookup"><span data-stu-id="55b7e-148">resource</span></span> | <span data-ttu-id="55b7e-149">string</span><span class="sxs-lookup"><span data-stu-id="55b7e-149">string</span></span> | <span data-ttu-id="55b7e-150">必需。</span><span class="sxs-lookup"><span data-stu-id="55b7e-150">Required.</span></span> <span data-ttu-id="55b7e-151">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="55b7e-151">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="55b7e-152">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="55b7e-152">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="55b7e-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="55b7e-153">expirationDateTime</span></span> | [<span data-ttu-id="55b7e-154">dateTime</span><span class="sxs-lookup"><span data-stu-id="55b7e-154">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="55b7e-155">必需。</span><span class="sxs-lookup"><span data-stu-id="55b7e-155">Required.</span></span> <span data-ttu-id="55b7e-156">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55b7e-156">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="55b7e-157">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="55b7e-157">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="55b7e-158">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="55b7e-158">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="55b7e-159">clientState</span><span class="sxs-lookup"><span data-stu-id="55b7e-159">clientState</span></span> | <span data-ttu-id="55b7e-160">字符串</span><span class="sxs-lookup"><span data-stu-id="55b7e-160">string</span></span> | <span data-ttu-id="55b7e-161">可选。</span><span class="sxs-lookup"><span data-stu-id="55b7e-161">Optional.</span></span> <span data-ttu-id="55b7e-162">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="55b7e-162">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="55b7e-163">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="55b7e-163">The maximum length is 128 characters.</span></span> <span data-ttu-id="55b7e-164">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="55b7e-164">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="55b7e-165">id</span><span class="sxs-lookup"><span data-stu-id="55b7e-165">id</span></span> | <span data-ttu-id="55b7e-166">string</span><span class="sxs-lookup"><span data-stu-id="55b7e-166">string</span></span> | <span data-ttu-id="55b7e-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="55b7e-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="55b7e-169">applicationId</span><span class="sxs-lookup"><span data-stu-id="55b7e-169">applicationId</span></span> | <span data-ttu-id="55b7e-170">string</span><span class="sxs-lookup"><span data-stu-id="55b7e-170">string</span></span> | <span data-ttu-id="55b7e-171">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="55b7e-171">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="55b7e-172">只读。</span><span class="sxs-lookup"><span data-stu-id="55b7e-172">Read-only.</span></span> |
| <span data-ttu-id="55b7e-173">creatorId</span><span class="sxs-lookup"><span data-stu-id="55b7e-173">creatorId</span></span> | <span data-ttu-id="55b7e-174">string</span><span class="sxs-lookup"><span data-stu-id="55b7e-174">string</span></span> | <span data-ttu-id="55b7e-175">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="55b7e-175">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="55b7e-176">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="55b7e-176">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="55b7e-177">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="55b7e-177">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="55b7e-178">只读。</span><span class="sxs-lookup"><span data-stu-id="55b7e-178">Read-only.</span></span> |
| <span data-ttu-id="55b7e-179">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="55b7e-179">latestSupportedTlsVersion</span></span> | <span data-ttu-id="55b7e-180">字符串</span><span class="sxs-lookup"><span data-stu-id="55b7e-180">String</span></span> | <span data-ttu-id="55b7e-181">指定通知终结点支持的最新 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="55b7e-181">Specifies the latest TLS version that the notification endpoint supports.</span></span> <span data-ttu-id="55b7e-182">允许订阅者在有限的时间段内使用过时的 TLS 版本。允许订阅者在有限的时间段内使用过时的 TLS 版本。</span><span class="sxs-lookup"><span data-stu-id="55b7e-182">Allows subscribers to use a deprecated version of TLS for a limited period.</span></span> <span data-ttu-id="55b7e-183">可能的数值：**v1_0**、**v1_1**、**v1_2**、**v1_3**。</span><span class="sxs-lookup"><span data-stu-id="55b7e-183">Possible values: **v1_0**, **v1_1**, **v1_2**, **v1_3**.</span></span> <span data-ttu-id="55b7e-184">可选，默认为 v1_2。</span><span class="sxs-lookup"><span data-stu-id="55b7e-184">Optional, defaults to v1_2.</span></span> <span data-ttu-id="55b7e-185">如果客户端终结点支持 TLS 1.2 或更高版本，则不需要此属性。</span><span class="sxs-lookup"><span data-stu-id="55b7e-185">If the client endpoint supports TLS 1.2 or above this property is not needed.</span></span> <span data-ttu-id="55b7e-186">如果客户端终结点仅支持 TLS 1.0 或1.1，则应将此属性设置为相应的版本，否则操作将失败。</span><span class="sxs-lookup"><span data-stu-id="55b7e-186">If the client endpoint supports only TLS 1.0 or 1.1, this property should be set to the corresponding version or the operation will fail.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="55b7e-187">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="55b7e-187">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="55b7e-188">Resource</span><span class="sxs-lookup"><span data-stu-id="55b7e-188">Resource</span></span>            | <span data-ttu-id="55b7e-189">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="55b7e-189">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="55b7e-190">用户、组和其他目录资源</span><span class="sxs-lookup"><span data-stu-id="55b7e-190">User, group, other directory resources</span></span>   | <span data-ttu-id="55b7e-191">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-191">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="55b7e-192">邮件</span><span class="sxs-lookup"><span data-stu-id="55b7e-192">Mail</span></span>                | <span data-ttu-id="55b7e-193">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-193">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="55b7e-194">日历</span><span class="sxs-lookup"><span data-stu-id="55b7e-194">Calendar</span></span>            | <span data-ttu-id="55b7e-195">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-195">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="55b7e-196">联系人</span><span class="sxs-lookup"><span data-stu-id="55b7e-196">Contacts</span></span>            | <span data-ttu-id="55b7e-197">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-197">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="55b7e-198">组对话</span><span class="sxs-lookup"><span data-stu-id="55b7e-198">Group conversations</span></span> | <span data-ttu-id="55b7e-199">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-199">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="55b7e-200">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="55b7e-200">Drive root items</span></span>    | <span data-ttu-id="55b7e-201">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-201">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="55b7e-202">安全警报</span><span class="sxs-lookup"><span data-stu-id="55b7e-202">Security alerts</span></span>     | <span data-ttu-id="55b7e-203">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="55b7e-203">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="55b7e-204">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="55b7e-204">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="55b7e-205">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="55b7e-205">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="55b7e-206">关系</span><span class="sxs-lookup"><span data-stu-id="55b7e-206">Relationships</span></span>

<span data-ttu-id="55b7e-207">无</span><span class="sxs-lookup"><span data-stu-id="55b7e-207">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b7e-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55b7e-208">JSON representation</span></span>

<span data-ttu-id="55b7e-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55b7e-209">Here is a JSON representation of the resource.</span></span>

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
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "latestSupportedTlsVersion": "string"
}
```

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
