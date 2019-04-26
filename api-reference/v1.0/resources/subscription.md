---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: piotrci
ms.openlocfilehash: db3a536395f327115af69f769f37c823013ec7fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563698"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="cd361-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="cd361-104">subscription resource type</span></span>

<span data-ttu-id="cd361-105">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="cd361-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="cd361-106">目前，支持订阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="cd361-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="cd361-107">Outlook 中的[消息][]、[事件][]或[联系人][]</span><span class="sxs-lookup"><span data-stu-id="cd361-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="cd361-108">Office 365 组的[对话][]</span><span class="sxs-lookup"><span data-stu-id="cd361-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="cd361-109">OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容</span><span class="sxs-lookup"><span data-stu-id="cd361-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="cd361-110">Azure Active Directory 中的[用户][]或[组][]</span><span class="sxs-lookup"><span data-stu-id="cd361-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="cd361-111">Microsoft Graph 安全性 API 中的[警报][]</span><span class="sxs-lookup"><span data-stu-id="cd361-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd361-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd361-112">JSON representation</span></span>

<span data-ttu-id="cd361-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd361-113">Here is a JSON representation of the resource.</span></span>

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
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="cd361-114">属性</span><span class="sxs-lookup"><span data-stu-id="cd361-114">Properties</span></span>

| <span data-ttu-id="cd361-115">属性</span><span class="sxs-lookup"><span data-stu-id="cd361-115">Property</span></span> | <span data-ttu-id="cd361-116">类型</span><span class="sxs-lookup"><span data-stu-id="cd361-116">Type</span></span> | <span data-ttu-id="cd361-117">说明</span><span class="sxs-lookup"><span data-stu-id="cd361-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="cd361-118">changeType</span><span class="sxs-lookup"><span data-stu-id="cd361-118">changeType</span></span> | <span data-ttu-id="cd361-119">string</span><span class="sxs-lookup"><span data-stu-id="cd361-119">string</span></span> | <span data-ttu-id="cd361-120">必需。</span><span class="sxs-lookup"><span data-stu-id="cd361-120">Required.</span></span> <span data-ttu-id="cd361-121">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="cd361-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="cd361-122">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="cd361-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="cd361-123">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="cd361-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="cd361-124">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="cd361-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="cd361-125">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="cd361-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="cd361-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="cd361-126">notificationUrl</span></span> | <span data-ttu-id="cd361-127">string</span><span class="sxs-lookup"><span data-stu-id="cd361-127">string</span></span> | <span data-ttu-id="cd361-128">必需。</span><span class="sxs-lookup"><span data-stu-id="cd361-128">Required.</span></span> <span data-ttu-id="cd361-129">将接收通知的终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="cd361-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="cd361-130">该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="cd361-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="cd361-131">resource</span><span class="sxs-lookup"><span data-stu-id="cd361-131">resource</span></span> | <span data-ttu-id="cd361-132">string</span><span class="sxs-lookup"><span data-stu-id="cd361-132">string</span></span> | <span data-ttu-id="cd361-133">必需。</span><span class="sxs-lookup"><span data-stu-id="cd361-133">Required.</span></span> <span data-ttu-id="cd361-134">指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="cd361-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="cd361-135">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="cd361-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="cd361-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cd361-136">expirationDateTime</span></span> | [<span data-ttu-id="cd361-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="cd361-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="cd361-138">必需。</span><span class="sxs-lookup"><span data-stu-id="cd361-138">Required.</span></span> <span data-ttu-id="cd361-139">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cd361-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="cd361-140">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="cd361-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="cd361-141">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="cd361-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="cd361-142">clientState</span><span class="sxs-lookup"><span data-stu-id="cd361-142">clientState</span></span> | <span data-ttu-id="cd361-143">字符串</span><span class="sxs-lookup"><span data-stu-id="cd361-143">string</span></span> | <span data-ttu-id="cd361-144">可选。</span><span class="sxs-lookup"><span data-stu-id="cd361-144">Optional.</span></span> <span data-ttu-id="cd361-145">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="cd361-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="cd361-146">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="cd361-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="cd361-147">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="cd361-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="cd361-148">id</span><span class="sxs-lookup"><span data-stu-id="cd361-148">id</span></span> | <span data-ttu-id="cd361-149">string</span><span class="sxs-lookup"><span data-stu-id="cd361-149">string</span></span> | <span data-ttu-id="cd361-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cd361-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="cd361-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="cd361-152">applicationId</span></span> | <span data-ttu-id="cd361-153">string</span><span class="sxs-lookup"><span data-stu-id="cd361-153">string</span></span> | <span data-ttu-id="cd361-154">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="cd361-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="cd361-155">只读。</span><span class="sxs-lookup"><span data-stu-id="cd361-155">Read-only.</span></span> |
| <span data-ttu-id="cd361-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="cd361-156">creatorId</span></span> | <span data-ttu-id="cd361-157">string</span><span class="sxs-lookup"><span data-stu-id="cd361-157">string</span></span> | <span data-ttu-id="cd361-158">已创建订阅的用户或服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="cd361-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="cd361-159">如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="cd361-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="cd361-160">如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="cd361-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="cd361-161">只读。</span><span class="sxs-lookup"><span data-stu-id="cd361-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="cd361-162">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="cd361-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="cd361-163">资源</span><span class="sxs-lookup"><span data-stu-id="cd361-163">Resource</span></span>            | <span data-ttu-id="cd361-164">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="cd361-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="cd361-165">邮件</span><span class="sxs-lookup"><span data-stu-id="cd361-165">Mail</span></span>                | <span data-ttu-id="cd361-166">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="cd361-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cd361-167">日历</span><span class="sxs-lookup"><span data-stu-id="cd361-167">Calendar</span></span>            | <span data-ttu-id="cd361-168">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="cd361-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cd361-169">联系人</span><span class="sxs-lookup"><span data-stu-id="cd361-169">Contacts</span></span>            | <span data-ttu-id="cd361-170">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="cd361-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cd361-171">组对话</span><span class="sxs-lookup"><span data-stu-id="cd361-171">Group conversations</span></span> | <span data-ttu-id="cd361-172">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="cd361-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cd361-173">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="cd361-173">Drive root items</span></span>    | <span data-ttu-id="cd361-174">4230 分钟（不到 3 天）</span><span class="sxs-lookup"><span data-stu-id="cd361-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cd361-175">安全警报</span><span class="sxs-lookup"><span data-stu-id="cd361-175">Security alerts</span></span>     | <span data-ttu-id="cd361-176">43200分钟（不到 30 天）</span><span class="sxs-lookup"><span data-stu-id="cd361-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="cd361-177">**注意：** 现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="cd361-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="cd361-178">今后，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="cd361-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="cd361-179">关系</span><span class="sxs-lookup"><span data-stu-id="cd361-179">Relationships</span></span>

<span data-ttu-id="cd361-180">无</span><span class="sxs-lookup"><span data-stu-id="cd361-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="cd361-181">方法</span><span class="sxs-lookup"><span data-stu-id="cd361-181">Methods</span></span>

| <span data-ttu-id="cd361-182">方法</span><span class="sxs-lookup"><span data-stu-id="cd361-182">Method</span></span> | <span data-ttu-id="cd361-183">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd361-183">Return Type</span></span> | <span data-ttu-id="cd361-184">说明</span><span class="sxs-lookup"><span data-stu-id="cd361-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="cd361-185">创建订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="cd361-186">订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-186">subscription</span></span>](subscription.md) | <span data-ttu-id="cd361-187">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="cd361-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="cd361-188">更新订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="cd361-189">订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-189">subscription</span></span>](subscription.md) | <span data-ttu-id="cd361-190">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="cd361-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="cd361-191">列出订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="cd361-192">订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-192">subscription</span></span>](subscription.md) | <span data-ttu-id="cd361-193">列出有效订阅。</span><span class="sxs-lookup"><span data-stu-id="cd361-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="cd361-194">获取订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="cd361-195">订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-195">subscription</span></span>](subscription.md) | <span data-ttu-id="cd361-196">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd361-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="cd361-197">删除订阅</span><span class="sxs-lookup"><span data-stu-id="cd361-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="cd361-198">无</span><span class="sxs-lookup"><span data-stu-id="cd361-198">None</span></span> |<span data-ttu-id="cd361-199">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="cd361-199">Deletes a subscription object.</span></span> |

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
