# <a name="workinghours-resource-type"></a><span data-ttu-id="96cf6-101">workingHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="96cf6-101">workingHours resource type</span></span>

<span data-ttu-id="96cf6-102">表示特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="96cf6-102">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="96cf6-103">在处理活动或资源规划应用场景中，访问用户的工作时间会有所帮助。</span><span class="sxs-lookup"><span data-stu-id="96cf6-103">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="96cf6-104">可以[获取](../api/user_get_mailboxsettings.md#request-3)用户的工作时间，并将其[设置](../api/user_update_mailboxsettings.md#request-2)为用户[邮箱设置](mailboxSettings.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="96cf6-104">You can [get](../api/user_get_mailboxsettings.md#request-3) and [set](../api/user_update_mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxSettings.md).</span></span> 

<span data-ttu-id="96cf6-105">可以选择以不同于在 Outlook 客户端设置时区的方式，为你的工作时间设置时区。</span><span class="sxs-lookup"><span data-stu-id="96cf6-105">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="96cf6-106">在某些情况下这很有用，比如当你在一个与平常工作时区不同的地方旅行时。</span><span class="sxs-lookup"><span data-stu-id="96cf6-106">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="96cf6-107">可以将 Outlook 客户端设置</span><span class="sxs-lookup"><span data-stu-id="96cf6-107">You can set the Outlook client</span></span>  
<span data-ttu-id="96cf6-108">为目标时区，以便在你访问时 Outlook 时间值显示为本地时间。</span><span class="sxs-lookup"><span data-stu-id="96cf6-108">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="96cf6-109">当其他人在你通常的工作地点申请与你进行工作会议时，他们仍然可以在相应的时区遵守你的工作时间。</span><span class="sxs-lookup"><span data-stu-id="96cf6-109">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="96cf6-110">属性</span><span class="sxs-lookup"><span data-stu-id="96cf6-110">Properties</span></span>
| <span data-ttu-id="96cf6-111">属性</span><span class="sxs-lookup"><span data-stu-id="96cf6-111">Property</span></span>     | <span data-ttu-id="96cf6-112">类型</span><span class="sxs-lookup"><span data-stu-id="96cf6-112">Type</span></span>   |<span data-ttu-id="96cf6-113">说明</span><span class="sxs-lookup"><span data-stu-id="96cf6-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96cf6-114">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="96cf6-114">daysOfWeek</span></span> | <span data-ttu-id="96cf6-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="96cf6-115">String collection</span></span> | <span data-ttu-id="96cf6-116">用户一周工作的天数。</span><span class="sxs-lookup"><span data-stu-id="96cf6-116">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="96cf6-117">startTime</span><span class="sxs-lookup"><span data-stu-id="96cf6-117"><starttime></span></span> | <span data-ttu-id="96cf6-118">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="96cf6-118">Edm.TimeOfDay</span></span> | <span data-ttu-id="96cf6-119">一天中用户开始工作的时间。</span><span class="sxs-lookup"><span data-stu-id="96cf6-119">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="96cf6-120">endTime</span><span class="sxs-lookup"><span data-stu-id="96cf6-120"><endtime></span></span> | <span data-ttu-id="96cf6-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="96cf6-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="96cf6-122">一天中用户停止工作的时间。</span><span class="sxs-lookup"><span data-stu-id="96cf6-122">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="96cf6-123">timeZone</span><span class="sxs-lookup"><span data-stu-id="96cf6-123">timeZone</span></span> | [<span data-ttu-id="96cf6-124">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="96cf6-124">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="96cf6-125">工作时间应用的时区。</span><span class="sxs-lookup"><span data-stu-id="96cf6-125">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="96cf6-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96cf6-126">JSON representation</span></span>

<span data-ttu-id="96cf6-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96cf6-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->