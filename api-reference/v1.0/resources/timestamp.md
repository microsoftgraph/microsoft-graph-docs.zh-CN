# <a name="timestamp-resource-type"></a><span data-ttu-id="23cf2-101">timeStamp资源类型</span><span class="sxs-lookup"><span data-stu-id="23cf2-101">timeStamp resource type</span></span>

<span data-ttu-id="23cf2-102">时间点的日期和时间信息。</span><span class="sxs-lookup"><span data-stu-id="23cf2-102">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23cf2-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23cf2-103">JSON representation</span></span>

<span data-ttu-id="23cf2-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23cf2-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="23cf2-105">属性</span><span class="sxs-lookup"><span data-stu-id="23cf2-105">Properties</span></span>
| <span data-ttu-id="23cf2-106">属性</span><span class="sxs-lookup"><span data-stu-id="23cf2-106">Property</span></span>       | <span data-ttu-id="23cf2-107">类型</span><span class="sxs-lookup"><span data-stu-id="23cf2-107">Type</span></span>    |<span data-ttu-id="23cf2-108">说明</span><span class="sxs-lookup"><span data-stu-id="23cf2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23cf2-109">date</span><span class="sxs-lookup"><span data-stu-id="23cf2-109">date</span></span>|<span data-ttu-id="23cf2-110">时间</span><span class="sxs-lookup"><span data-stu-id="23cf2-110">Date</span></span>|<span data-ttu-id="23cf2-111">时间戳的日期部分。</span><span class="sxs-lookup"><span data-stu-id="23cf2-111">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="23cf2-112">time</span><span class="sxs-lookup"><span data-stu-id="23cf2-112">time</span></span>|<span data-ttu-id="23cf2-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="23cf2-113">TimeOfDay</span></span>|<span data-ttu-id="23cf2-114">时间戳的时间部分。</span><span class="sxs-lookup"><span data-stu-id="23cf2-114">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="23cf2-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="23cf2-115">timeZone</span></span>|<span data-ttu-id="23cf2-116">字符串</span><span class="sxs-lookup"><span data-stu-id="23cf2-116">String</span></span>|<span data-ttu-id="23cf2-117">时间戳的时区部分, 它是世界上24个纵向区域之一。</span><span class="sxs-lookup"><span data-stu-id="23cf2-117">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->