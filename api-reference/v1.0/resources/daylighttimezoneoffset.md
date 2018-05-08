# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="8b9ea-101">daylightTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b9ea-101">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="8b9ea-102">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-102">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="8b9ea-103">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="8b9ea-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="8b9ea-104">**bias** 为 300</span><span class="sxs-lookup"><span data-stu-id="8b9ea-104">**bias** is 300</span></span>
- <span data-ttu-id="8b9ea-105">**daylightBias** 为 -100</span><span class="sxs-lookup"><span data-stu-id="8b9ea-105">**daylightBias** is -100</span></span>
- <span data-ttu-id="8b9ea-106">**dayOccurrence** 为 4</span><span class="sxs-lookup"><span data-stu-id="8b9ea-106">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="8b9ea-107">**dayOfWeek** 为“sunday”</span><span class="sxs-lookup"><span data-stu-id="8b9ea-107">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="8b9ea-108">**month** 为 5</span><span class="sxs-lookup"><span data-stu-id="8b9ea-108">**month** is 5</span></span>
- <span data-ttu-id="8b9ea-109">**time** 为 02:00:00 _ **year** 为 0，意味着夏令时的时长比 UTC 早 +300-100=200 分钟。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-109">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="8b9ea-110">从夏令时到标准时间的时区切换出现在每年五月第四个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-110">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="8b9ea-111">属性</span><span class="sxs-lookup"><span data-stu-id="8b9ea-111">Properties</span></span>
| <span data-ttu-id="8b9ea-112">属性</span><span class="sxs-lookup"><span data-stu-id="8b9ea-112">Property</span></span>     | <span data-ttu-id="8b9ea-113">类型</span><span class="sxs-lookup"><span data-stu-id="8b9ea-113">Type</span></span>   |<span data-ttu-id="8b9ea-114">说明</span><span class="sxs-lookup"><span data-stu-id="8b9ea-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8b9ea-115">daylightBias</span><span class="sxs-lookup"><span data-stu-id="8b9ea-115">daylightBias</span></span> | <span data-ttu-id="8b9ea-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="8b9ea-116">Edm.Int32</span></span> | <span data-ttu-id="8b9ea-117">夏时制与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-117">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="8b9ea-118">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-118">This value is in points.</span></span>  |
| <span data-ttu-id="8b9ea-119">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="8b9ea-119">dayOccurrence</span></span> | <span data-ttu-id="8b9ea-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="8b9ea-120">Edm.Int32</span></span> | <span data-ttu-id="8b9ea-121">表示从标准时间到夏令时的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-121">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="8b9ea-122">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="8b9ea-122">DAYOFWEEK</span></span> | <span data-ttu-id="8b9ea-123">string</span><span class="sxs-lookup"><span data-stu-id="8b9ea-123">string</span></span> | <span data-ttu-id="8b9ea-124">表示从标准时间到夏令时的切换出现时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-124">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="8b9ea-125">month</span><span class="sxs-lookup"><span data-stu-id="8b9ea-125">month</span></span> | <span data-ttu-id="8b9ea-126">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="8b9ea-126">Edm.Int32</span></span> | <span data-ttu-id="8b9ea-127">表示从标准时间到夏令时的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-127">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="8b9ea-128">time</span><span class="sxs-lookup"><span data-stu-id="8b9ea-128">time</span></span> | <span data-ttu-id="8b9ea-129">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8b9ea-129">Edm.TimeOfDay</span></span> | <span data-ttu-id="8b9ea-130">表示从标准时间到夏令时的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-130">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="8b9ea-131">year</span><span class="sxs-lookup"><span data-stu-id="8b9ea-131">year</span></span> | <span data-ttu-id="8b9ea-132">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="8b9ea-132">Edm.Int32</span></span> | <span data-ttu-id="8b9ea-133">表示从标准时间到夏令时的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-133">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="8b9ea-134">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-134">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8b9ea-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b9ea-135">JSON representation</span></span>

<span data-ttu-id="8b9ea-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b9ea-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->