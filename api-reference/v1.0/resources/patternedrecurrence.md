# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="ffbe9-101">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffbe9-101">patternedRecurrence resource type</span></span>

<span data-ttu-id="ffbe9-102">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="ffbe9-102">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="ffbe9-103">属性</span><span class="sxs-lookup"><span data-stu-id="ffbe9-103">Properties</span></span>
| <span data-ttu-id="ffbe9-104">属性</span><span class="sxs-lookup"><span data-stu-id="ffbe9-104">Property</span></span>     | <span data-ttu-id="ffbe9-105">类型</span><span class="sxs-lookup"><span data-stu-id="ffbe9-105">Type</span></span>   |<span data-ttu-id="ffbe9-106">说明</span><span class="sxs-lookup"><span data-stu-id="ffbe9-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffbe9-107">模式</span><span class="sxs-lookup"><span data-stu-id="ffbe9-107">pattern</span></span>|[<span data-ttu-id="ffbe9-108">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="ffbe9-108">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="ffbe9-109">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="ffbe9-109">The frequency of an event.</span></span>|
|<span data-ttu-id="ffbe9-110">区域</span><span class="sxs-lookup"><span data-stu-id="ffbe9-110">range</span></span>|[<span data-ttu-id="ffbe9-111">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="ffbe9-111">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="ffbe9-112">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="ffbe9-112">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffbe9-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffbe9-113">JSON representation</span></span>

<span data-ttu-id="ffbe9-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffbe9-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedrecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->