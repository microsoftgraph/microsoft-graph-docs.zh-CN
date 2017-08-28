# <a name="recurrencerange-resource-type"></a><span data-ttu-id="1d092-101">recurrenceRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d092-101">recurrenceRange resource type</span></span>

<span data-ttu-id="1d092-102">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="1d092-102">The duration of an event.</span></span>

## <a name="properties"></a><span data-ttu-id="1d092-103">属性</span><span class="sxs-lookup"><span data-stu-id="1d092-103">Properties</span></span>

| <span data-ttu-id="1d092-104">属性</span><span class="sxs-lookup"><span data-stu-id="1d092-104">Property</span></span>     | <span data-ttu-id="1d092-105">类型</span><span class="sxs-lookup"><span data-stu-id="1d092-105">Type</span></span>   |<span data-ttu-id="1d092-106">说明</span><span class="sxs-lookup"><span data-stu-id="1d092-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d092-107">endDate</span><span class="sxs-lookup"><span data-stu-id="1d092-107">endDate</span></span>|<span data-ttu-id="1d092-108">日期</span><span class="sxs-lookup"><span data-stu-id="1d092-108">Date</span></span>|<span data-ttu-id="1d092-109">系列的结束日期。</span><span class="sxs-lookup"><span data-stu-id="1d092-109">The end date of the series.</span></span>|
|<span data-ttu-id="1d092-110">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="1d092-110">numberOfOccurrences</span></span>|<span data-ttu-id="1d092-111">Int32</span><span class="sxs-lookup"><span data-stu-id="1d092-111">Int32</span></span>|<span data-ttu-id="1d092-112">事件重复发生的次数。</span><span class="sxs-lookup"><span data-stu-id="1d092-112">How many times to repeat the event.</span></span>|
|<span data-ttu-id="1d092-113">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="1d092-113">recurrenceTimeZone</span></span>|<span data-ttu-id="1d092-114">String</span><span class="sxs-lookup"><span data-stu-id="1d092-114">String</span></span> |<span data-ttu-id="1d092-115">**startDate** 和 **endDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="1d092-115">Time zone for the **startDate** and **endDate** properties.</span></span> |
|<span data-ttu-id="1d092-116">startDate</span><span class="sxs-lookup"><span data-stu-id="1d092-116">startDate</span></span>|<span data-ttu-id="1d092-117">日期</span><span class="sxs-lookup"><span data-stu-id="1d092-117">Date</span></span>|<span data-ttu-id="1d092-118">序列的开始日期。</span><span class="sxs-lookup"><span data-stu-id="1d092-118">The start date of the series.</span></span>|
|<span data-ttu-id="1d092-119">type</span><span class="sxs-lookup"><span data-stu-id="1d092-119">type</span></span>|<span data-ttu-id="1d092-120">String</span><span class="sxs-lookup"><span data-stu-id="1d092-120">String</span></span>|<span data-ttu-id="1d092-p101">定期区域：EndDate = 0，NoEnd = 1，Numbered = 2。可能的值是：`EndDate`、`NoEnd`、`Numbered`。</span><span class="sxs-lookup"><span data-stu-id="1d092-p101">The recurrence range: EndDate = 0, NoEnd = 1, Numbered = 2. Possible values are: `EndDate`, `NoEnd`, `Numbered`.</span></span>||

## <a name="json-representation"></a><span data-ttu-id="1d092-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d092-123">JSON representation</span></span>

<span data-ttu-id="1d092-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d092-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
