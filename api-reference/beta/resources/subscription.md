---
title: 订阅资源类型
description: '订阅允许客户端应用在 Microsoft Graph 中接收有关数据更改的通知。 当前为以下资源启用了订阅:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163936"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="22c4e-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="22c4e-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22c4e-105">订阅允许客户端应用在 Microsoft Graph 中接收有关数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="22c4e-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="22c4e-106">当前为以下资源启用了订阅:</span><span class="sxs-lookup"><span data-stu-id="22c4e-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="22c4e-107">Outlook 中的[邮件][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="22c4e-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="22c4e-108">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="22c4e-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="22c4e-109">OneDrive for business 中根文件夹[driveItem][]的层次结构中的内容, 或用户个人 OneDrive 中的根文件夹或子文件夹[driveItem][]的内容</span><span class="sxs-lookup"><span data-stu-id="22c4e-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="22c4e-110">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="22c4e-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="22c4e-111">来自 Microsoft Graph 安全性 API 的[警报][]</span><span class="sxs-lookup"><span data-stu-id="22c4e-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="22c4e-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22c4e-112">JSON representation</span></span>

<span data-ttu-id="22c4e-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22c4e-113">Here is a JSON representation of the resource.</span></span>

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
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="22c4e-114">属性</span><span class="sxs-lookup"><span data-stu-id="22c4e-114">Properties</span></span>

| <span data-ttu-id="22c4e-115">属性</span><span class="sxs-lookup"><span data-stu-id="22c4e-115">Property</span></span> | <span data-ttu-id="22c4e-116">类型</span><span class="sxs-lookup"><span data-stu-id="22c4e-116">Type</span></span> | <span data-ttu-id="22c4e-117">说明</span><span class="sxs-lookup"><span data-stu-id="22c4e-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="22c4e-118">changeType</span><span class="sxs-lookup"><span data-stu-id="22c4e-118">changeType</span></span> | <span data-ttu-id="22c4e-119">string</span><span class="sxs-lookup"><span data-stu-id="22c4e-119">string</span></span> | <span data-ttu-id="22c4e-120">必需。</span><span class="sxs-lookup"><span data-stu-id="22c4e-120">Required.</span></span> <span data-ttu-id="22c4e-121">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="22c4e-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="22c4e-122">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="22c4e-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="22c4e-123">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="22c4e-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="22c4e-124">注意: 驱动器根项通知仅支持`updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="22c4e-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="22c4e-125">用户和组通知支持`updated`和`deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="22c4e-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="22c4e-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="22c4e-126">notificationUrl</span></span> | <span data-ttu-id="22c4e-127">string</span><span class="sxs-lookup"><span data-stu-id="22c4e-127">string</span></span> | <span data-ttu-id="22c4e-128">必需。</span><span class="sxs-lookup"><span data-stu-id="22c4e-128">Required.</span></span> <span data-ttu-id="22c4e-129">将接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="22c4e-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="22c4e-130">此 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="22c4e-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="22c4e-131">resource</span><span class="sxs-lookup"><span data-stu-id="22c4e-131">resource</span></span> | <span data-ttu-id="22c4e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="22c4e-132">string</span></span> | <span data-ttu-id="22c4e-133">必需。</span><span class="sxs-lookup"><span data-stu-id="22c4e-133">Required.</span></span> <span data-ttu-id="22c4e-134">指定将监视其更改的资源。</span><span class="sxs-lookup"><span data-stu-id="22c4e-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="22c4e-135">不包括基 URL (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="22c4e-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="22c4e-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="22c4e-136">expirationDateTime</span></span> | <span data-ttu-id="22c4e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22c4e-137">DateTimeOffset</span></span> | <span data-ttu-id="22c4e-138">必需。</span><span class="sxs-lookup"><span data-stu-id="22c4e-138">Required.</span></span> <span data-ttu-id="22c4e-139">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22c4e-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="22c4e-140">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="22c4e-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="22c4e-141">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="22c4e-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="22c4e-142">clientState</span><span class="sxs-lookup"><span data-stu-id="22c4e-142">clientState</span></span> | <span data-ttu-id="22c4e-143">string</span><span class="sxs-lookup"><span data-stu-id="22c4e-143">string</span></span> | <span data-ttu-id="22c4e-144">可选。</span><span class="sxs-lookup"><span data-stu-id="22c4e-144">Optional.</span></span> <span data-ttu-id="22c4e-145">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="22c4e-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="22c4e-146">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="22c4e-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="22c4e-147">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="22c4e-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="22c4e-148">id</span><span class="sxs-lookup"><span data-stu-id="22c4e-148">id</span></span> | <span data-ttu-id="22c4e-149">string</span><span class="sxs-lookup"><span data-stu-id="22c4e-149">string</span></span> | <span data-ttu-id="22c4e-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="22c4e-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="22c4e-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="22c4e-152">applicationId</span></span> | <span data-ttu-id="22c4e-153">string</span><span class="sxs-lookup"><span data-stu-id="22c4e-153">string</span></span> | <span data-ttu-id="22c4e-154">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="22c4e-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="22c4e-155">只读。</span><span class="sxs-lookup"><span data-stu-id="22c4e-155">Read-only.</span></span> |
| <span data-ttu-id="22c4e-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="22c4e-156">creatorId</span></span> | <span data-ttu-id="22c4e-157">string</span><span class="sxs-lookup"><span data-stu-id="22c4e-157">string</span></span> | <span data-ttu-id="22c4e-158">创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="22c4e-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="22c4e-159">如果应用程序使用委派权限来创建订阅, 则此字段包含代表已登录的用户的 id, 该应用代表。</span><span class="sxs-lookup"><span data-stu-id="22c4e-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="22c4e-160">如果应用程序使用的是应用程序权限, 则此字段包含与该应用对应的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="22c4e-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="22c4e-161">只读。</span><span class="sxs-lookup"><span data-stu-id="22c4e-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="22c4e-162">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="22c4e-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="22c4e-163">资源</span><span class="sxs-lookup"><span data-stu-id="22c4e-163">Resource</span></span>            | <span data-ttu-id="22c4e-164">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="22c4e-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="22c4e-165">邮件</span><span class="sxs-lookup"><span data-stu-id="22c4e-165">Mail</span></span>                | <span data-ttu-id="22c4e-166">4230分钟 (3 天内)</span><span class="sxs-lookup"><span data-stu-id="22c4e-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="22c4e-167">日历</span><span class="sxs-lookup"><span data-stu-id="22c4e-167">Calendar</span></span>            | <span data-ttu-id="22c4e-168">4230分钟 (3 天内)</span><span class="sxs-lookup"><span data-stu-id="22c4e-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="22c4e-169">联系人</span><span class="sxs-lookup"><span data-stu-id="22c4e-169">Contacts</span></span>            | <span data-ttu-id="22c4e-170">4230分钟 (3 天内)</span><span class="sxs-lookup"><span data-stu-id="22c4e-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="22c4e-171">组对话</span><span class="sxs-lookup"><span data-stu-id="22c4e-171">Group conversations</span></span> | <span data-ttu-id="22c4e-172">4230分钟 (3 天内)</span><span class="sxs-lookup"><span data-stu-id="22c4e-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="22c4e-173">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="22c4e-173">Drive root items</span></span>    | <span data-ttu-id="22c4e-174">4230分钟 (3 天内)</span><span class="sxs-lookup"><span data-stu-id="22c4e-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="22c4e-175">安全警报</span><span class="sxs-lookup"><span data-stu-id="22c4e-175">Security alerts</span></span>     | <span data-ttu-id="22c4e-176">43200分钟 (30 天内)</span><span class="sxs-lookup"><span data-stu-id="22c4e-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="22c4e-177">**注意:** 现有应用程序和新应用程序不应超过支持的值。</span><span class="sxs-lookup"><span data-stu-id="22c4e-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="22c4e-178">将来, 创建或续订超出最大值的订阅的任何请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="22c4e-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="22c4e-179">关系</span><span class="sxs-lookup"><span data-stu-id="22c4e-179">Relationships</span></span>

<span data-ttu-id="22c4e-180">无</span><span class="sxs-lookup"><span data-stu-id="22c4e-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="22c4e-181">方法</span><span class="sxs-lookup"><span data-stu-id="22c4e-181">Methods</span></span>

| <span data-ttu-id="22c4e-182">方法</span><span class="sxs-lookup"><span data-stu-id="22c4e-182">Method</span></span> | <span data-ttu-id="22c4e-183">返回类型</span><span class="sxs-lookup"><span data-stu-id="22c4e-183">Return Type</span></span> | <span data-ttu-id="22c4e-184">说明</span><span class="sxs-lookup"><span data-stu-id="22c4e-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="22c4e-185">创建订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="22c4e-186">订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-186">subscription</span></span>](subscription.md) | <span data-ttu-id="22c4e-187">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="22c4e-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="22c4e-188">更新订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="22c4e-189">订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-189">subscription</span></span>](subscription.md) | <span data-ttu-id="22c4e-190">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="22c4e-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="22c4e-191">列出订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="22c4e-192">订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-192">subscription</span></span>](subscription.md) | <span data-ttu-id="22c4e-193">列出活动订阅。</span><span class="sxs-lookup"><span data-stu-id="22c4e-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="22c4e-194">获取订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="22c4e-195">订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-195">subscription</span></span>](subscription.md) | <span data-ttu-id="22c4e-196">读取订阅对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22c4e-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="22c4e-197">删除订阅</span><span class="sxs-lookup"><span data-stu-id="22c4e-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="22c4e-198">无</span><span class="sxs-lookup"><span data-stu-id="22c4e-198">None</span></span> | <span data-ttu-id="22c4e-199">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="22c4e-199">Delete a subscription object.</span></span> |

[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[用户]: ./user.md
[user]: ./user.md
[警报]: ./alert.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
