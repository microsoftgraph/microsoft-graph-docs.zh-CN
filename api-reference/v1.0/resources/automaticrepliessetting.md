# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="69a3b-101">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="69a3b-101">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="69a3b-p101">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="69a3b-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="69a3b-104">属性</span><span class="sxs-lookup"><span data-stu-id="69a3b-104">Properties</span></span>
| <span data-ttu-id="69a3b-105">属性</span><span class="sxs-lookup"><span data-stu-id="69a3b-105">Property</span></span>     | <span data-ttu-id="69a3b-106">类型</span><span class="sxs-lookup"><span data-stu-id="69a3b-106">Type</span></span>   |<span data-ttu-id="69a3b-107">说明</span><span class="sxs-lookup"><span data-stu-id="69a3b-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69a3b-108">externalAudience</span><span class="sxs-lookup"><span data-stu-id="69a3b-108">externalAudience</span></span>|<span data-ttu-id="69a3b-109">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="69a3b-109">ExternalAudienceScope</span></span>| <span data-ttu-id="69a3b-110">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示将接收 **ExternalReplyMessage** 的已登录用户组织外部的受众组。</span><span class="sxs-lookup"><span data-stu-id="69a3b-110">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or . Possible values are: , , `Scheduled`.</span></span> <span data-ttu-id="69a3b-111">可取值为：`none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="69a3b-111">The possible values are `none`, `contactsOnly`, `all`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="69a3b-112">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="69a3b-112">externalReplyMessage</span></span>|<span data-ttu-id="69a3b-113">string</span><span class="sxs-lookup"><span data-stu-id="69a3b-113">string</span></span>|<span data-ttu-id="69a3b-114">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="69a3b-114">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="69a3b-115">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="69a3b-115">internalReplyMessage</span></span>|<span data-ttu-id="69a3b-116">string</span><span class="sxs-lookup"><span data-stu-id="69a3b-116">string</span></span>|<span data-ttu-id="69a3b-117">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="69a3b-117">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="69a3b-118">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="69a3b-118">scheduledEndDateTime</span></span>|[<span data-ttu-id="69a3b-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="69a3b-119">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="69a3b-120">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="69a3b-120">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="69a3b-121">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="69a3b-121">scheduledStartDateTime</span></span>|[<span data-ttu-id="69a3b-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="69a3b-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="69a3b-123">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="69a3b-123">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="69a3b-124">status</span><span class="sxs-lookup"><span data-stu-id="69a3b-124">status</span></span>|<span data-ttu-id="69a3b-125">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="69a3b-125">AutomaticRepliesStatus</span></span>|<span data-ttu-id="69a3b-126">自动答复的配置状态。</span><span class="sxs-lookup"><span data-stu-id="69a3b-126">Configurations status for automatic replies. Possible values are: , , .</span></span> <span data-ttu-id="69a3b-127">可取值为：`disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="69a3b-127">The possible values are `disabled`, `alwaysEnabled`, `scheduled`, , , , , , , , , or .</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69a3b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69a3b-128">JSON representation</span></span>

<span data-ttu-id="69a3b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69a3b-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
