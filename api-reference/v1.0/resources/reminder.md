# <a name="reminder-resource-type"></a><span data-ttu-id="dd7bf-101">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="dd7bf-101">reminder resource type</span></span>

<span data-ttu-id="dd7bf-102">用户 [日历](calendar.md)中的 [事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-102">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dd7bf-103">属性</span><span class="sxs-lookup"><span data-stu-id="dd7bf-103">Properties</span></span>
| <span data-ttu-id="dd7bf-104">属性</span><span class="sxs-lookup"><span data-stu-id="dd7bf-104">Property</span></span>     | <span data-ttu-id="dd7bf-105">类型</span><span class="sxs-lookup"><span data-stu-id="dd7bf-105">Type</span></span>   |<span data-ttu-id="dd7bf-106">说明</span><span class="sxs-lookup"><span data-stu-id="dd7bf-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd7bf-107">changeKey</span><span class="sxs-lookup"><span data-stu-id="dd7bf-107">changeKey</span></span>|<span data-ttu-id="dd7bf-108">字符串</span><span class="sxs-lookup"><span data-stu-id="dd7bf-108">String</span></span>|<span data-ttu-id="dd7bf-p101">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="dd7bf-112">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="dd7bf-112">eventEndTime</span></span>|[<span data-ttu-id="dd7bf-113">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dd7bf-113">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="dd7bf-114">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-114">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="dd7bf-115">eventId</span><span class="sxs-lookup"><span data-stu-id="dd7bf-115">eventId</span></span>|<span data-ttu-id="dd7bf-116">字符串</span><span class="sxs-lookup"><span data-stu-id="dd7bf-116">String</span></span>|<span data-ttu-id="dd7bf-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="dd7bf-119">eventLocation</span><span class="sxs-lookup"><span data-stu-id="dd7bf-119">eventLocation</span></span>|[<span data-ttu-id="dd7bf-120">位置</span><span class="sxs-lookup"><span data-stu-id="dd7bf-120">Location</span></span>](location.md)|<span data-ttu-id="dd7bf-121">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-121">The location of the event.</span></span>|
|<span data-ttu-id="dd7bf-122">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="dd7bf-122">eventStartTime</span></span>|[<span data-ttu-id="dd7bf-123">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dd7bf-123">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="dd7bf-124">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-124">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="dd7bf-125">eventSubject</span><span class="sxs-lookup"><span data-stu-id="dd7bf-125">eventSubject</span></span>|<span data-ttu-id="dd7bf-126">字符串</span><span class="sxs-lookup"><span data-stu-id="dd7bf-126">String</span></span>|<span data-ttu-id="dd7bf-127">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-127">The text of the event's subject line.</span></span>|
|<span data-ttu-id="dd7bf-128">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="dd7bf-128">eventWebLink</span></span>|<span data-ttu-id="dd7bf-129">字符串</span><span class="sxs-lookup"><span data-stu-id="dd7bf-129">String</span></span>|<span data-ttu-id="dd7bf-130">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-130">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="dd7bf-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="dd7bf-133">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-133">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="dd7bf-134">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="dd7bf-134">reminderFireTime</span></span>|[<span data-ttu-id="dd7bf-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dd7bf-135">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="dd7bf-136">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-136">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd7bf-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd7bf-137">JSON representation</span></span>

<span data-ttu-id="dd7bf-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd7bf-138">Here is a JSON representation of the resource</span></span>

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