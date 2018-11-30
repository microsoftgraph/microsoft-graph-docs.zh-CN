---
title: 订阅资源类型
description: 订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。 目前，订阅启用以下资源：
ms.openlocfilehash: 5ece39954d661c6b7ef948d0ed7d514782fbceae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011451"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="bda93-104">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="bda93-104">subscription resource type</span></span>

<span data-ttu-id="bda93-105">订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。</span><span class="sxs-lookup"><span data-stu-id="bda93-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="bda93-106">目前，订阅启用以下资源：</span><span class="sxs-lookup"><span data-stu-id="bda93-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="bda93-107">邮件、 事件和 Outlook 中的联系人。</span><span class="sxs-lookup"><span data-stu-id="bda93-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="bda93-108">来自 Office 组的对话。</span><span class="sxs-lookup"><span data-stu-id="bda93-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="bda93-109">从 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="bda93-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="bda93-110">用户和 Azure Active Directory 组。</span><span class="sxs-lookup"><span data-stu-id="bda93-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="bda93-111">来自 Microsoft Graph 安全 API 的通知。</span><span class="sxs-lookup"><span data-stu-id="bda93-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bda93-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bda93-112">JSON representation</span></span>

<span data-ttu-id="bda93-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bda93-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bda93-114">属性</span><span class="sxs-lookup"><span data-stu-id="bda93-114">Properties</span></span>

| <span data-ttu-id="bda93-115">属性</span><span class="sxs-lookup"><span data-stu-id="bda93-115">Property</span></span> | <span data-ttu-id="bda93-116">类型</span><span class="sxs-lookup"><span data-stu-id="bda93-116">Type</span></span> | <span data-ttu-id="bda93-117">说明</span><span class="sxs-lookup"><span data-stu-id="bda93-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="bda93-118">changeType</span><span class="sxs-lookup"><span data-stu-id="bda93-118">changeType</span></span> | <span data-ttu-id="bda93-119">string</span><span class="sxs-lookup"><span data-stu-id="bda93-119">string</span></span> | <span data-ttu-id="bda93-120">必需。</span><span class="sxs-lookup"><span data-stu-id="bda93-120">Required.</span></span> <span data-ttu-id="bda93-121">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="bda93-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="bda93-122">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="bda93-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="bda93-123">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="bda93-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="bda93-124">注意： 驱动器根项目通知仅支持`updated`changeType。</span><span class="sxs-lookup"><span data-stu-id="bda93-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="bda93-125">用户和组通知支持`updated`和`deleted`changeType。</span><span class="sxs-lookup"><span data-stu-id="bda93-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="bda93-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="bda93-126">notificationUrl</span></span> | <span data-ttu-id="bda93-127">string</span><span class="sxs-lookup"><span data-stu-id="bda93-127">string</span></span> | <span data-ttu-id="bda93-128">必需。</span><span class="sxs-lookup"><span data-stu-id="bda93-128">Required.</span></span> <span data-ttu-id="bda93-129">将接收通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="bda93-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="bda93-130">此 URL 必须进行使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="bda93-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="bda93-131">resource</span><span class="sxs-lookup"><span data-stu-id="bda93-131">resource</span></span> | <span data-ttu-id="bda93-132">string</span><span class="sxs-lookup"><span data-stu-id="bda93-132">string</span></span> | <span data-ttu-id="bda93-133">必需。</span><span class="sxs-lookup"><span data-stu-id="bda93-133">Required.</span></span> <span data-ttu-id="bda93-134">指定将监视的更改的资源。</span><span class="sxs-lookup"><span data-stu-id="bda93-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="bda93-135">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="bda93-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="bda93-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bda93-136">expirationDateTime</span></span> | [<span data-ttu-id="bda93-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="bda93-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="bda93-138">必需。</span><span class="sxs-lookup"><span data-stu-id="bda93-138">Required.</span></span> <span data-ttu-id="bda93-139">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bda93-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="bda93-140">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="bda93-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="bda93-141">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="bda93-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="bda93-142">clientState</span><span class="sxs-lookup"><span data-stu-id="bda93-142">clientState</span></span> | <span data-ttu-id="bda93-143">string</span><span class="sxs-lookup"><span data-stu-id="bda93-143">string</span></span> | <span data-ttu-id="bda93-144">可选。</span><span class="sxs-lookup"><span data-stu-id="bda93-144">Optional.</span></span> <span data-ttu-id="bda93-145">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="bda93-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="bda93-146">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="bda93-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="bda93-147">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="bda93-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="bda93-148">id</span><span class="sxs-lookup"><span data-stu-id="bda93-148">id</span></span> | <span data-ttu-id="bda93-149">string</span><span class="sxs-lookup"><span data-stu-id="bda93-149">string</span></span> | <span data-ttu-id="bda93-p109">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bda93-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="bda93-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="bda93-152">applicationId</span></span> | <span data-ttu-id="bda93-153">string</span><span class="sxs-lookup"><span data-stu-id="bda93-153">string</span></span> | <span data-ttu-id="bda93-154">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="bda93-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="bda93-155">只读。</span><span class="sxs-lookup"><span data-stu-id="bda93-155">Read-only.</span></span> |
| <span data-ttu-id="bda93-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="bda93-156">creatorId</span></span> | <span data-ttu-id="bda93-157">string</span><span class="sxs-lookup"><span data-stu-id="bda93-157">string</span></span> | <span data-ttu-id="bda93-158">用户或创建订阅的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="bda93-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="bda93-159">如果应用程序使用委派权限创建订阅，此字段包含应用程序调用代表登录用户的 id。</span><span class="sxs-lookup"><span data-stu-id="bda93-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="bda93-160">如果应用程序使用应用程序权限，此字段包含对应于应用程序的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="bda93-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="bda93-161">只读。</span><span class="sxs-lookup"><span data-stu-id="bda93-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="bda93-162">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="bda93-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="bda93-163">资源</span><span class="sxs-lookup"><span data-stu-id="bda93-163">Resource</span></span>            | <span data-ttu-id="bda93-164">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="bda93-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="bda93-165">邮件</span><span class="sxs-lookup"><span data-stu-id="bda93-165">Mail</span></span>                | <span data-ttu-id="bda93-166">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="bda93-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bda93-167">日历</span><span class="sxs-lookup"><span data-stu-id="bda93-167">Calendar</span></span>            | <span data-ttu-id="bda93-168">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="bda93-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bda93-169">联系人</span><span class="sxs-lookup"><span data-stu-id="bda93-169">Contacts</span></span>            | <span data-ttu-id="bda93-170">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="bda93-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bda93-171">组对话</span><span class="sxs-lookup"><span data-stu-id="bda93-171">Group conversations</span></span> | <span data-ttu-id="bda93-172">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="bda93-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bda93-173">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="bda93-173">Drive root items</span></span>    | <span data-ttu-id="bda93-174">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="bda93-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bda93-175">安全警报</span><span class="sxs-lookup"><span data-stu-id="bda93-175">Security alerts</span></span>     | <span data-ttu-id="bda93-176">43200 分钟 （在 30 天）</span><span class="sxs-lookup"><span data-stu-id="bda93-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="bda93-177">**注意：** 现有应用程序和新的应用程序不应超过受支持的值。</span><span class="sxs-lookup"><span data-stu-id="bda93-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="bda93-178">将来，任何创建或更新的最大值超出订阅已请求将失败。</span><span class="sxs-lookup"><span data-stu-id="bda93-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="bda93-179">Relationships</span><span class="sxs-lookup"><span data-stu-id="bda93-179">Relationships</span></span>

<span data-ttu-id="bda93-180">无</span><span class="sxs-lookup"><span data-stu-id="bda93-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="bda93-181">方法</span><span class="sxs-lookup"><span data-stu-id="bda93-181">Methods</span></span>

| <span data-ttu-id="bda93-182">方法</span><span class="sxs-lookup"><span data-stu-id="bda93-182">Method</span></span> | <span data-ttu-id="bda93-183">返回类型</span><span class="sxs-lookup"><span data-stu-id="bda93-183">Return Type</span></span> | <span data-ttu-id="bda93-184">说明</span><span class="sxs-lookup"><span data-stu-id="bda93-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="bda93-185">创建订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="bda93-186">订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-186">subscription</span></span>](subscription.md) | <span data-ttu-id="bda93-187">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="bda93-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="bda93-188">更新订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="bda93-189">订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-189">subscription</span></span>](subscription.md) | <span data-ttu-id="bda93-190">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="bda93-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="bda93-191">列表订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="bda93-192">订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-192">subscription</span></span>](subscription.md) | <span data-ttu-id="bda93-193">列出了活动订阅。</span><span class="sxs-lookup"><span data-stu-id="bda93-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="bda93-194">获取订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="bda93-195">订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-195">subscription</span></span>](subscription.md) | <span data-ttu-id="bda93-196">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bda93-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="bda93-197">删除订阅</span><span class="sxs-lookup"><span data-stu-id="bda93-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="bda93-198">无</span><span class="sxs-lookup"><span data-stu-id="bda93-198">None</span></span> |<span data-ttu-id="bda93-199">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="bda93-199">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
