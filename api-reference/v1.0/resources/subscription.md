# <a name="subscription-resource-type"></a><span data-ttu-id="7af08-101">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="7af08-101">subscription resource type</span></span>

<span data-ttu-id="7af08-102">订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。</span><span class="sxs-lookup"><span data-stu-id="7af08-102">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="7af08-103">目前，订阅启用以下资源：</span><span class="sxs-lookup"><span data-stu-id="7af08-103">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="7af08-104">邮件、 事件和 Outlook 中的联系人。</span><span class="sxs-lookup"><span data-stu-id="7af08-104">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="7af08-105">来自 Office 组的对话。</span><span class="sxs-lookup"><span data-stu-id="7af08-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="7af08-106">从 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="7af08-106">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="7af08-107">用户和 Azure Active Directory 组。</span><span class="sxs-lookup"><span data-stu-id="7af08-107">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="7af08-108">来自 Microsoft Graph 安全 API 的通知。</span><span class="sxs-lookup"><span data-stu-id="7af08-108">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7af08-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7af08-109">JSON representation</span></span>

<span data-ttu-id="7af08-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7af08-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7af08-111">属性</span><span class="sxs-lookup"><span data-stu-id="7af08-111">Properties</span></span>

| <span data-ttu-id="7af08-112">属性</span><span class="sxs-lookup"><span data-stu-id="7af08-112">Property</span></span> | <span data-ttu-id="7af08-113">类型</span><span class="sxs-lookup"><span data-stu-id="7af08-113">Type</span></span> | <span data-ttu-id="7af08-114">说明</span><span class="sxs-lookup"><span data-stu-id="7af08-114">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="7af08-115">changeType</span><span class="sxs-lookup"><span data-stu-id="7af08-115">changeType</span></span> | <span data-ttu-id="7af08-116">string</span><span class="sxs-lookup"><span data-stu-id="7af08-116">string</span></span> | <span data-ttu-id="7af08-117">必需。</span><span class="sxs-lookup"><span data-stu-id="7af08-117">Required.</span></span> <span data-ttu-id="7af08-118">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="7af08-118">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="7af08-119">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="7af08-119">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="7af08-120">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="7af08-120">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="7af08-121">注意： 驱动器根项目通知仅支持`updated`changeType。</span><span class="sxs-lookup"><span data-stu-id="7af08-121">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="7af08-122">用户和组通知支持`updated`和`deleted`changeType。</span><span class="sxs-lookup"><span data-stu-id="7af08-122">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="7af08-123">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="7af08-123">notificationUrl</span></span> | <span data-ttu-id="7af08-124">string</span><span class="sxs-lookup"><span data-stu-id="7af08-124">string</span></span> | <span data-ttu-id="7af08-125">必需。</span><span class="sxs-lookup"><span data-stu-id="7af08-125">Required.</span></span> <span data-ttu-id="7af08-126">将接收通知的终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="7af08-126">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="7af08-127">此 URL 必须进行使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="7af08-127">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="7af08-128">resource</span><span class="sxs-lookup"><span data-stu-id="7af08-128">resource</span></span> | <span data-ttu-id="7af08-129">string</span><span class="sxs-lookup"><span data-stu-id="7af08-129">string</span></span> | <span data-ttu-id="7af08-130">必需。</span><span class="sxs-lookup"><span data-stu-id="7af08-130">Required.</span></span> <span data-ttu-id="7af08-131">指定将监视的更改的资源。</span><span class="sxs-lookup"><span data-stu-id="7af08-131">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="7af08-132">不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="7af08-132">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="7af08-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7af08-133">expirationDateTime</span></span> | [<span data-ttu-id="7af08-134">dateTime</span><span class="sxs-lookup"><span data-stu-id="7af08-134">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="7af08-135">必需。</span><span class="sxs-lookup"><span data-stu-id="7af08-135">Required.</span></span> <span data-ttu-id="7af08-136">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7af08-136">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="7af08-137">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="7af08-137">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="7af08-138">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="7af08-138">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="7af08-139">clientState</span><span class="sxs-lookup"><span data-stu-id="7af08-139">clientState</span></span> | <span data-ttu-id="7af08-140">string</span><span class="sxs-lookup"><span data-stu-id="7af08-140">string</span></span> | <span data-ttu-id="7af08-141">可选。</span><span class="sxs-lookup"><span data-stu-id="7af08-141">Optional.</span></span> <span data-ttu-id="7af08-142">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="7af08-142">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="7af08-143">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="7af08-143">The maximum length is 128 characters.</span></span> <span data-ttu-id="7af08-144">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="7af08-144">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="7af08-145">id</span><span class="sxs-lookup"><span data-stu-id="7af08-145">id</span></span> | <span data-ttu-id="7af08-146">string</span><span class="sxs-lookup"><span data-stu-id="7af08-146">string</span></span> | <span data-ttu-id="7af08-p108">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7af08-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="7af08-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="7af08-149">applicationId</span></span> | <span data-ttu-id="7af08-150">string</span><span class="sxs-lookup"><span data-stu-id="7af08-150">string</span></span> | <span data-ttu-id="7af08-151">用于创建订阅的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="7af08-151">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="7af08-152">只读。</span><span class="sxs-lookup"><span data-stu-id="7af08-152">Read-only.</span></span> |
| <span data-ttu-id="7af08-153">creatorId</span><span class="sxs-lookup"><span data-stu-id="7af08-153">creatorId</span></span> | <span data-ttu-id="7af08-154">string</span><span class="sxs-lookup"><span data-stu-id="7af08-154">string</span></span> | <span data-ttu-id="7af08-155">用户或创建订阅的服务主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="7af08-155">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="7af08-156">如果应用程序使用委派权限创建订阅，此字段包含应用程序调用代表登录用户的 id。</span><span class="sxs-lookup"><span data-stu-id="7af08-156">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="7af08-157">如果应用程序使用应用程序权限，此字段包含对应于应用程序的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="7af08-157">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="7af08-158">只读。</span><span class="sxs-lookup"><span data-stu-id="7af08-158">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="7af08-159">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="7af08-159">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="7af08-160">资源</span><span class="sxs-lookup"><span data-stu-id="7af08-160">Resource</span></span>            | <span data-ttu-id="7af08-161">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="7af08-161">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="7af08-162">邮件</span><span class="sxs-lookup"><span data-stu-id="7af08-162">Mail</span></span>                | <span data-ttu-id="7af08-163">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="7af08-163">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7af08-164">日历</span><span class="sxs-lookup"><span data-stu-id="7af08-164">Calendar</span></span>            | <span data-ttu-id="7af08-165">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="7af08-165">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7af08-166">联系人</span><span class="sxs-lookup"><span data-stu-id="7af08-166">Contacts</span></span>            | <span data-ttu-id="7af08-167">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="7af08-167">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7af08-168">组对话</span><span class="sxs-lookup"><span data-stu-id="7af08-168">Group conversations</span></span> | <span data-ttu-id="7af08-169">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="7af08-169">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7af08-170">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="7af08-170">Drive root items</span></span>    | <span data-ttu-id="7af08-171">4230 分钟 （在 3 天）</span><span class="sxs-lookup"><span data-stu-id="7af08-171">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7af08-172">安全警报</span><span class="sxs-lookup"><span data-stu-id="7af08-172">Security alerts</span></span>     | <span data-ttu-id="7af08-173">43200 分钟 （在 30 天）</span><span class="sxs-lookup"><span data-stu-id="7af08-173">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="7af08-174">**注意：** 现有应用程序和新的应用程序不应超过受支持的值。</span><span class="sxs-lookup"><span data-stu-id="7af08-174">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="7af08-175">将来，任何创建或更新的最大值超出订阅已请求将失败。</span><span class="sxs-lookup"><span data-stu-id="7af08-175">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="7af08-176">Relationships</span><span class="sxs-lookup"><span data-stu-id="7af08-176">Relationships</span></span>

<span data-ttu-id="7af08-177">无</span><span class="sxs-lookup"><span data-stu-id="7af08-177">None</span></span>

## <a name="methods"></a><span data-ttu-id="7af08-178">方法</span><span class="sxs-lookup"><span data-stu-id="7af08-178">Methods</span></span>

| <span data-ttu-id="7af08-179">方法</span><span class="sxs-lookup"><span data-stu-id="7af08-179">Method</span></span> | <span data-ttu-id="7af08-180">返回类型</span><span class="sxs-lookup"><span data-stu-id="7af08-180">Return Type</span></span> | <span data-ttu-id="7af08-181">说明</span><span class="sxs-lookup"><span data-stu-id="7af08-181">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="7af08-182">创建订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-182">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="7af08-183">订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-183">subscription</span></span>](subscription.md) | <span data-ttu-id="7af08-184">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="7af08-184">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="7af08-185">更新订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-185">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="7af08-186">订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-186">subscription</span></span>](subscription.md) | <span data-ttu-id="7af08-187">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="7af08-187">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="7af08-188">列表订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-188">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="7af08-189">订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-189">subscription</span></span>](subscription.md) | <span data-ttu-id="7af08-190">列出了活动订阅。</span><span class="sxs-lookup"><span data-stu-id="7af08-190">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="7af08-191">获取订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-191">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="7af08-192">订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-192">subscription</span></span>](subscription.md) | <span data-ttu-id="7af08-193">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7af08-193">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="7af08-194">删除订阅</span><span class="sxs-lookup"><span data-stu-id="7af08-194">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="7af08-195">无</span><span class="sxs-lookup"><span data-stu-id="7af08-195">None</span></span> |<span data-ttu-id="7af08-196">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="7af08-196">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
