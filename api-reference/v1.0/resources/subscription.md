# <a name="subscription-resource-type"></a><span data-ttu-id="0b943-101">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="0b943-101">Subscription resource type</span></span>

<span data-ttu-id="0b943-102">借助订阅，客户端应用可以接收 Microsoft Graph 中的数据更改的通知。</span><span class="sxs-lookup"><span data-stu-id="0b943-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="0b943-103">目前，已为下列资源启用了订阅：</span><span class="sxs-lookup"><span data-stu-id="0b943-103">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="0b943-104">Outlook 中的邮件、活动和联系人</span><span class="sxs-lookup"><span data-stu-id="0b943-104">Mail, events, and contacts from Outlook</span></span>
- <span data-ttu-id="0b943-105">来自 Office 组的对话</span><span class="sxs-lookup"><span data-stu-id="0b943-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="0b943-106">来自 OneDrive 的驱动器根项</span><span class="sxs-lookup"><span data-stu-id="0b943-106">Drive root items from OneDrive</span></span>
- <span data-ttu-id="0b943-107">来自 Azure Active Directory 用户和组</span><span class="sxs-lookup"><span data-stu-id="0b943-107">Users and Groups from Azure Active Directory</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b943-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b943-108">JSON representation</span></span>

<span data-ttu-id="0b943-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b943-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0b943-110">属性</span><span class="sxs-lookup"><span data-stu-id="0b943-110">Properties</span></span>

| <span data-ttu-id="0b943-111">属性</span><span class="sxs-lookup"><span data-stu-id="0b943-111">Property</span></span> | <span data-ttu-id="0b943-112">类型</span><span class="sxs-lookup"><span data-stu-id="0b943-112">Type</span></span> | <span data-ttu-id="0b943-113">说明</span><span class="sxs-lookup"><span data-stu-id="0b943-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="0b943-114">changeType</span><span class="sxs-lookup"><span data-stu-id="0b943-114">changeType</span></span> | <span data-ttu-id="0b943-115">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-115">string</span></span> | <span data-ttu-id="0b943-116">必需。</span><span class="sxs-lookup"><span data-stu-id="0b943-116">Required.</span></span> <span data-ttu-id="0b943-117">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="0b943-117">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="0b943-118">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="0b943-118">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="0b943-119">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="0b943-119">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="0b943-120">注意：驱动器根项通知仅支持 `updated` changeType。</span><span class="sxs-lookup"><span data-stu-id="0b943-120">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="0b943-121">用户和组通知支持 `updated` 和 `deleted` changeType。</span><span class="sxs-lookup"><span data-stu-id="0b943-121">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="0b943-122">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="0b943-122">notificationUrl</span></span> | <span data-ttu-id="0b943-123">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-123">string</span></span> | <span data-ttu-id="0b943-124">必需。</span><span class="sxs-lookup"><span data-stu-id="0b943-124">Required.</span></span> <span data-ttu-id="0b943-125">将接收通知的端点的 URL。</span><span class="sxs-lookup"><span data-stu-id="0b943-125">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="0b943-126">此 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="0b943-126">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="0b943-127">resource</span><span class="sxs-lookup"><span data-stu-id="0b943-127">resource</span></span> | <span data-ttu-id="0b943-128">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-128">string</span></span> | <span data-ttu-id="0b943-129">必需。</span><span class="sxs-lookup"><span data-stu-id="0b943-129">Required.</span></span> <span data-ttu-id="0b943-130">指定将监视其是否发生更改的资源。</span><span class="sxs-lookup"><span data-stu-id="0b943-130">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span> <span data-ttu-id="0b943-131">不包含基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="0b943-131">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="0b943-132">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b943-132">expirationDateTime</span></span> | [<span data-ttu-id="0b943-133">dateTime</span><span class="sxs-lookup"><span data-stu-id="0b943-133">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="0b943-134">必需。</span><span class="sxs-lookup"><span data-stu-id="0b943-134">Required.</span></span> <span data-ttu-id="0b943-135">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b943-135">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="0b943-136">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="0b943-136">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="0b943-137">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="0b943-137">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="0b943-138">clientState</span><span class="sxs-lookup"><span data-stu-id="0b943-138">clientState</span></span> | <span data-ttu-id="0b943-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-139">string</span></span> | <span data-ttu-id="0b943-140">可选。</span><span class="sxs-lookup"><span data-stu-id="0b943-140">Optional.</span></span> <span data-ttu-id="0b943-141">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="0b943-141">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="0b943-142">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="0b943-142">The maximum length is 128 characters.</span></span> <span data-ttu-id="0b943-143">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="0b943-143">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="0b943-144">id</span><span class="sxs-lookup"><span data-stu-id="0b943-144">id</span></span> | <span data-ttu-id="0b943-145">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-145">string</span></span> | <span data-ttu-id="0b943-p108">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0b943-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="0b943-148">applicationId</span><span class="sxs-lookup"><span data-stu-id="0b943-148">applicationId</span></span> | <span data-ttu-id="0b943-149">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-149">string</span></span> | <span data-ttu-id="0b943-150">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="0b943-150">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="0b943-151">只读。</span><span class="sxs-lookup"><span data-stu-id="0b943-151">Read-only.</span></span> |
| <span data-ttu-id="0b943-152">creatorId</span><span class="sxs-lookup"><span data-stu-id="0b943-152">creatorId</span></span> | <span data-ttu-id="0b943-153">字符串</span><span class="sxs-lookup"><span data-stu-id="0b943-153">string</span></span> | <span data-ttu-id="0b943-154">用户或创建订阅的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="0b943-154">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="0b943-155">如果应用程序使用委派权限创建订阅，此字段包含应用程序调用代表登录用户的 id。</span><span class="sxs-lookup"><span data-stu-id="0b943-155">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="0b943-156">如果应用程序使用应用程序权限，此字段包含应用程序对应的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="0b943-156">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="0b943-157">只读。</span><span class="sxs-lookup"><span data-stu-id="0b943-157">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="0b943-158">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="0b943-158">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="0b943-159">资源</span><span class="sxs-lookup"><span data-stu-id="0b943-159">Resource</span></span>            | <span data-ttu-id="0b943-160">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="0b943-160">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="0b943-161">邮件</span><span class="sxs-lookup"><span data-stu-id="0b943-161">Mail</span></span>                | <span data-ttu-id="0b943-162">4230 分钟 （3 天内）</span><span class="sxs-lookup"><span data-stu-id="0b943-162">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0b943-163">日历</span><span class="sxs-lookup"><span data-stu-id="0b943-163">Calendar</span></span>            | <span data-ttu-id="0b943-164">4230 分钟 （3 天内）</span><span class="sxs-lookup"><span data-stu-id="0b943-164">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0b943-165">联系人</span><span class="sxs-lookup"><span data-stu-id="0b943-165">Contacts</span></span>            | <span data-ttu-id="0b943-166">4230 分钟 （3 天内）</span><span class="sxs-lookup"><span data-stu-id="0b943-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0b943-167">组对话</span><span class="sxs-lookup"><span data-stu-id="0b943-167">Group conversations</span></span> | <span data-ttu-id="0b943-168">4230 分钟 （3 天内）</span><span class="sxs-lookup"><span data-stu-id="0b943-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0b943-169">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="0b943-169">Drive root items</span></span>    | <span data-ttu-id="0b943-170">4230 分钟 （3 天内）</span><span class="sxs-lookup"><span data-stu-id="0b943-170">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="0b943-171">**注意：** 现有和新的应用都不得超过支持的值。</span><span class="sxs-lookup"><span data-stu-id="0b943-171">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="0b943-172">将来，任何超出最大值的订阅创建或续订请求都将失败。</span><span class="sxs-lookup"><span data-stu-id="0b943-172">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="0b943-173">关系</span><span class="sxs-lookup"><span data-stu-id="0b943-173">Relationships</span></span>

<span data-ttu-id="0b943-174">无</span><span class="sxs-lookup"><span data-stu-id="0b943-174">None</span></span>

## <a name="methods"></a><span data-ttu-id="0b943-175">方法</span><span class="sxs-lookup"><span data-stu-id="0b943-175">Methods</span></span>

| <span data-ttu-id="0b943-176">方法</span><span class="sxs-lookup"><span data-stu-id="0b943-176">Method</span></span> | <span data-ttu-id="0b943-177">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b943-177">Return Type</span></span> | <span data-ttu-id="0b943-178">说明</span><span class="sxs-lookup"><span data-stu-id="0b943-178">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="0b943-179">创建订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-179">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="0b943-180">订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-180">subscription</span></span>](subscription.md) | <span data-ttu-id="0b943-181">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="0b943-181">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="0b943-182">更新订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-182">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="0b943-183">订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-183">subscription</span></span>](subscription.md) | <span data-ttu-id="0b943-184">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="0b943-184">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="0b943-185">订阅列表</span><span class="sxs-lookup"><span data-stu-id="0b943-185">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="0b943-186">订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-186">subscription</span></span>](subscription.md) | <span data-ttu-id="0b943-187">列出了活动订阅。</span><span class="sxs-lookup"><span data-stu-id="0b943-187">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="0b943-188">获取订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-188">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="0b943-189">订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-189">subscription</span></span>](subscription.md) | <span data-ttu-id="0b943-190">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b943-190">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="0b943-191">删除订阅</span><span class="sxs-lookup"><span data-stu-id="0b943-191">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="0b943-192">无</span><span class="sxs-lookup"><span data-stu-id="0b943-192">None</span></span> |<span data-ttu-id="0b943-193">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="0b943-193">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
