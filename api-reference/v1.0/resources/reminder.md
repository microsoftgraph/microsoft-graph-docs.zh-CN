# <a name="reminder-resource-type"></a><span data-ttu-id="3e74d-101">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="3e74d-101">reminder resource type</span></span>



## <a name="properties"></a><span data-ttu-id="3e74d-102">属性</span><span class="sxs-lookup"><span data-stu-id="3e74d-102">Properties</span></span>
| <span data-ttu-id="3e74d-103">属性</span><span class="sxs-lookup"><span data-stu-id="3e74d-103">Property</span></span>     | <span data-ttu-id="3e74d-104">类型</span><span class="sxs-lookup"><span data-stu-id="3e74d-104">Type</span></span>   |<span data-ttu-id="3e74d-105">说明</span><span class="sxs-lookup"><span data-stu-id="3e74d-105">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e74d-106">changeKey</span><span class="sxs-lookup"><span data-stu-id="3e74d-106">changeKey</span></span>|<span data-ttu-id="3e74d-107">String</span><span class="sxs-lookup"><span data-stu-id="3e74d-107">String</span></span>|<span data-ttu-id="3e74d-p101">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="3e74d-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="3e74d-111">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="3e74d-111">eventEndTime</span></span>|[<span data-ttu-id="3e74d-112">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e74d-112">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e74d-113">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3e74d-113">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="3e74d-114">eventId</span><span class="sxs-lookup"><span data-stu-id="3e74d-114">eventId</span></span>|<span data-ttu-id="3e74d-115">String</span><span class="sxs-lookup"><span data-stu-id="3e74d-115">String</span></span>|<span data-ttu-id="3e74d-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="3e74d-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="3e74d-118">eventLocation</span><span class="sxs-lookup"><span data-stu-id="3e74d-118">eventLocation</span></span>|[<span data-ttu-id="3e74d-119">位置</span><span class="sxs-lookup"><span data-stu-id="3e74d-119">Location</span></span>](location.md)|<span data-ttu-id="3e74d-120">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="3e74d-120">The location of the event.</span></span>|
|<span data-ttu-id="3e74d-121">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="3e74d-121">eventStartTime</span></span>|[<span data-ttu-id="3e74d-122">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e74d-122">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e74d-123">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3e74d-123">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="3e74d-124">eventSubject</span><span class="sxs-lookup"><span data-stu-id="3e74d-124">eventSubject</span></span>|<span data-ttu-id="3e74d-125">String</span><span class="sxs-lookup"><span data-stu-id="3e74d-125">String</span></span>|<span data-ttu-id="3e74d-126">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="3e74d-126">The text of the event's subject line.</span></span>|
|<span data-ttu-id="3e74d-127">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="3e74d-127">eventWebLink</span></span>|<span data-ttu-id="3e74d-128">String</span><span class="sxs-lookup"><span data-stu-id="3e74d-128">String</span></span>|<span data-ttu-id="3e74d-129">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="3e74d-129">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="3e74d-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="3e74d-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="3e74d-132">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="3e74d-132">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="3e74d-133">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="3e74d-133">reminderFireTime</span></span>|[<span data-ttu-id="3e74d-134">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e74d-134">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e74d-135">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3e74d-135">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e74d-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e74d-136">JSON representation</span></span>

<span data-ttu-id="3e74d-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e74d-137">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->