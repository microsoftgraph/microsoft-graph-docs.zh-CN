# <a name="subscription-resource-type"></a><span data-ttu-id="6cf0c-101">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="6cf0c-101">Subscription Resource Type</span></span>
<span data-ttu-id="6cf0c-102">借助订阅，客户端应用可以接收有关 Microsoft Graph 数据的通知。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph. Currently subscriptions are enabled for the following datasets:</span></span> <span data-ttu-id="6cf0c-103">目前，已为下列数据集启用了订阅：</span><span class="sxs-lookup"><span data-stu-id="6cf0c-103">Currently, subscriptions are enabled for the following datasets:</span></span>

1. <span data-ttu-id="6cf0c-104">Outlook 中的邮件、活动和联系人</span><span class="sxs-lookup"><span data-stu-id="6cf0c-104">Mail, events, and contacts from Outlook</span></span>
1. <span data-ttu-id="6cf0c-105">来自 Office 组的对话。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-105">Conversations from Office Groups.</span></span>
1. <span data-ttu-id="6cf0c-106">来自 OneDrive 的驱动器根项</span><span class="sxs-lookup"><span data-stu-id="6cf0c-106">Drive root items from OneDrive</span></span> 


## <a name="json-representation"></a><span data-ttu-id="6cf0c-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cf0c-107">JSON representation</span></span>

<span data-ttu-id="6cf0c-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-108">Here is a JSON representation of the resource.</span></span>

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
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6cf0c-109">属性</span><span class="sxs-lookup"><span data-stu-id="6cf0c-109">Properties</span></span>
| <span data-ttu-id="6cf0c-110">属性</span><span class="sxs-lookup"><span data-stu-id="6cf0c-110">Property</span></span>     | <span data-ttu-id="6cf0c-111">类型</span><span class="sxs-lookup"><span data-stu-id="6cf0c-111">Type</span></span>   |<span data-ttu-id="6cf0c-112">说明</span><span class="sxs-lookup"><span data-stu-id="6cf0c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cf0c-113">changeType</span><span class="sxs-lookup"><span data-stu-id="6cf0c-113">changeType</span></span>|<span data-ttu-id="6cf0c-114">string</span><span class="sxs-lookup"><span data-stu-id="6cf0c-114">string</span></span>|<span data-ttu-id="6cf0c-115">指示订阅资源中将引发通知的更改类型。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-115">Indicates the type of change in the subscribed resource that will raise a notification. The supported values are: , , . Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="6cf0c-116">支持的值是：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="6cf0c-117">可以使用以逗号分隔的列表组合多个值。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-117">Multiple values can be combined using a comma-separated list.</span></span>|
|<span data-ttu-id="6cf0c-118">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="6cf0c-118">notificationUrl</span></span>|<span data-ttu-id="6cf0c-119">string</span><span class="sxs-lookup"><span data-stu-id="6cf0c-119">string</span></span>|<span data-ttu-id="6cf0c-p103">将接收通知的端点的 URL。该 URL 必须使用 HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-p103">The URL of the endpoint that will receive the notifications. This URL has to make use of the HTTPS protocol.</span></span>|
|<span data-ttu-id="6cf0c-122">资源</span><span class="sxs-lookup"><span data-stu-id="6cf0c-122">resource</span></span>|<span data-ttu-id="6cf0c-123">string</span><span class="sxs-lookup"><span data-stu-id="6cf0c-123">string</span></span>|<span data-ttu-id="6cf0c-p104">指定要被监视以进行更改的资源。不包含基本 URL（“https://graph.microsoft.com/v1.0/”）。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-p104">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span>|
|<span data-ttu-id="6cf0c-126">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf0c-126">expirationDateTime</span></span>|[<span data-ttu-id="6cf0c-127">dateTime</span><span class="sxs-lookup"><span data-stu-id="6cf0c-127">dateTime</span></span>](http://tools.ietf.org/html/rfc3339)|<span data-ttu-id="6cf0c-128">指定 webhook 订阅过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-128">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="6cf0c-129">时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-129">Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.  See the table below for maximum values.</span></span>  <span data-ttu-id="6cf0c-130">请参阅下表，了解支持的最长订阅有效期。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-130">See the table below for maximum supported subscription length of time.</span></span> |
|<span data-ttu-id="6cf0c-131">clientState</span><span class="sxs-lookup"><span data-stu-id="6cf0c-131">clientState</span></span>|<span data-ttu-id="6cf0c-132">string</span><span class="sxs-lookup"><span data-stu-id="6cf0c-132">string</span></span>|<span data-ttu-id="6cf0c-133">指定服务为每个通知发送的 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-133">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="6cf0c-134">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-134">The maximum length is 255 characters.</span></span> <span data-ttu-id="6cf0c-135">通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-135">Specifies the value of the  property sent by the service in each notification. The maximum length is 128 characters. The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span>|
|<span data-ttu-id="6cf0c-136">id</span><span class="sxs-lookup"><span data-stu-id="6cf0c-136">id</span></span>|<span data-ttu-id="6cf0c-137">string</span><span class="sxs-lookup"><span data-stu-id="6cf0c-137">string</span></span>|<span data-ttu-id="6cf0c-p107">订阅的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-p107">Unique identifier for the subscription. Read-only.</span></span>|

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="6cf0c-140">每个资源类型的最长订阅有效期</span><span class="sxs-lookup"><span data-stu-id="6cf0c-140">Maximum length of subscription per resource type</span></span>
| <span data-ttu-id="6cf0c-141">资源</span><span class="sxs-lookup"><span data-stu-id="6cf0c-141">Resource</span></span> | <span data-ttu-id="6cf0c-142">最大过期时间</span><span class="sxs-lookup"><span data-stu-id="6cf0c-142">Maximum Expiration Time</span></span> |
|:---------------------|:--------------------|
|<span data-ttu-id="6cf0c-143">邮件</span><span class="sxs-lookup"><span data-stu-id="6cf0c-143">Mail</span></span>| <span data-ttu-id="6cf0c-144">4230 分钟。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-144">4230 minutes.</span></span>|
|<span data-ttu-id="6cf0c-145">日历</span><span class="sxs-lookup"><span data-stu-id="6cf0c-145">Calendar</span></span>| <span data-ttu-id="6cf0c-146">4230 分钟。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-146">4230 minutes.</span></span>|
|<span data-ttu-id="6cf0c-147">联系人</span><span class="sxs-lookup"><span data-stu-id="6cf0c-147">Contacts</span></span>| <span data-ttu-id="6cf0c-148">4230 分钟。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-148">4230 minutes.</span></span>|
|<span data-ttu-id="6cf0c-149">群组对话</span><span class="sxs-lookup"><span data-stu-id="6cf0c-149">Group conversations</span></span>| <span data-ttu-id="6cf0c-150">4230 分钟。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-150">4230 minutes.</span></span>|
|<span data-ttu-id="6cf0c-151">驱动器根项</span><span class="sxs-lookup"><span data-stu-id="6cf0c-151">Drive root items</span></span>| <span data-ttu-id="6cf0c-152">43200 分钟。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-152">43200 minutes.</span></span> <span data-ttu-id="6cf0c-153">现有和新的应用都不得超过支持的这一上限值。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-153">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="6cf0c-154">即将发布的版本也不允许超过此值。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-154">Higher values won't be permitted in upcoming releases.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6cf0c-155">关系</span><span class="sxs-lookup"><span data-stu-id="6cf0c-155">Relationships</span></span>
<span data-ttu-id="6cf0c-156">无</span><span class="sxs-lookup"><span data-stu-id="6cf0c-156">None</span></span>


## <a name="methods"></a><span data-ttu-id="6cf0c-157">方法</span><span class="sxs-lookup"><span data-stu-id="6cf0c-157">Methods</span></span>

| <span data-ttu-id="6cf0c-158">方法</span><span class="sxs-lookup"><span data-stu-id="6cf0c-158">Method</span></span>           | <span data-ttu-id="6cf0c-159">返回类型</span><span class="sxs-lookup"><span data-stu-id="6cf0c-159">Return Type</span></span>    |<span data-ttu-id="6cf0c-160">说明</span><span class="sxs-lookup"><span data-stu-id="6cf0c-160">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cf0c-161">创建订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-161">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="6cf0c-162">订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-162">subscription</span></span>](subscription.md) |<span data-ttu-id="6cf0c-163">订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-163">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span>|
|[<span data-ttu-id="6cf0c-164">更新订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-164">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="6cf0c-165">订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-165">subscription</span></span>](subscription.md) |<span data-ttu-id="6cf0c-166">通过更新其过期时间来续订订阅。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-166">Renews a subscription by updating its expiration time.</span></span>|
|[<span data-ttu-id="6cf0c-167">获取订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-167">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="6cf0c-168">订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-168">subscription</span></span>](subscription.md) |<span data-ttu-id="6cf0c-169">读取 subscription 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-169">Reads properties and relationships of subscription object.</span></span>|
|[<span data-ttu-id="6cf0c-170">删除订阅</span><span class="sxs-lookup"><span data-stu-id="6cf0c-170">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="6cf0c-171">无</span><span class="sxs-lookup"><span data-stu-id="6cf0c-171">None</span></span> |<span data-ttu-id="6cf0c-172">删除订阅对象。</span><span class="sxs-lookup"><span data-stu-id="6cf0c-172">Deletes a subscription object.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
