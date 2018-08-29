# <a name="customtimezone-resource-type"></a><span data-ttu-id="9cb15-101">customTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cb15-101">customTimeZone resource type</span></span>

<span data-ttu-id="9cb15-102">表示从标准时间到夏令时的切换不标准（反之亦然）的时区。</span><span class="sxs-lookup"><span data-stu-id="9cb15-102">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="9cb15-103">属性</span><span class="sxs-lookup"><span data-stu-id="9cb15-103">Properties</span></span>
| <span data-ttu-id="9cb15-104">属性</span><span class="sxs-lookup"><span data-stu-id="9cb15-104">Property</span></span>     | <span data-ttu-id="9cb15-105">类型</span><span class="sxs-lookup"><span data-stu-id="9cb15-105">Type</span></span>   |<span data-ttu-id="9cb15-106">说明</span><span class="sxs-lookup"><span data-stu-id="9cb15-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cb15-107">bias</span><span class="sxs-lookup"><span data-stu-id="9cb15-107">bias</span></span> | <span data-ttu-id="9cb15-108">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9cb15-108">Edm.Int32</span></span> | <span data-ttu-id="9cb15-109">时区与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="9cb15-109">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="9cb15-110">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="9cb15-110">This value is in minutes.</span></span> <span data-ttu-id="9cb15-111">早于 UTC 的时区为正偏移；晚于 UTC 的时区为负偏移。</span><span class="sxs-lookup"><span data-stu-id="9cb15-111">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="9cb15-112">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="9cb15-112">daylightOffset</span></span> | [<span data-ttu-id="9cb15-113">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="9cb15-113">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="9cb15-114">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="9cb15-114">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="9cb15-115">name</span><span class="sxs-lookup"><span data-stu-id="9cb15-115">name</span></span> | <span data-ttu-id="9cb15-116">string</span><span class="sxs-lookup"><span data-stu-id="9cb15-116">string</span></span> | <span data-ttu-id="9cb15-117">自定义时区的名称。</span><span class="sxs-lookup"><span data-stu-id="9cb15-117">The name of the custom time zone.</span></span> |
| <span data-ttu-id="9cb15-118">standardOffset</span><span class="sxs-lookup"><span data-stu-id="9cb15-118">standardOffset</span></span> | [<span data-ttu-id="9cb15-119">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="9cb15-119">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="9cb15-120">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="9cb15-120">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9cb15-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cb15-121">JSON representation</span></span>

<span data-ttu-id="9cb15-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cb15-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->