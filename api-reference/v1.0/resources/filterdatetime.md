# <a name="filterdatetime-resource-type"></a><span data-ttu-id="93258-101">FilterDatetime 资源类型</span><span class="sxs-lookup"><span data-stu-id="93258-101">FilterDatetime resource type</span></span>

<span data-ttu-id="93258-102">表示在筛选值时如何筛选日期。</span><span class="sxs-lookup"><span data-stu-id="93258-102">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="93258-103">属性</span><span class="sxs-lookup"><span data-stu-id="93258-103">Properties</span></span>
| <span data-ttu-id="93258-104">属性</span><span class="sxs-lookup"><span data-stu-id="93258-104">Property</span></span>     | <span data-ttu-id="93258-105">类型</span><span class="sxs-lookup"><span data-stu-id="93258-105">Type</span></span>   |<span data-ttu-id="93258-106">说明</span><span class="sxs-lookup"><span data-stu-id="93258-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93258-107">date</span><span class="sxs-lookup"><span data-stu-id="93258-107">date</span></span>|<span data-ttu-id="93258-108">string</span><span class="sxs-lookup"><span data-stu-id="93258-108">string</span></span>|<span data-ttu-id="93258-109">用于筛选数据的采用 ISO8601 格式的日期。</span><span class="sxs-lookup"><span data-stu-id="93258-109">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="93258-110">specificity</span><span class="sxs-lookup"><span data-stu-id="93258-110">specificity</span></span>|<span data-ttu-id="93258-111">string</span><span class="sxs-lookup"><span data-stu-id="93258-111">string</span></span>|<span data-ttu-id="93258-112">用于保留数据的日期的具体程度。</span><span class="sxs-lookup"><span data-stu-id="93258-112">How specific the date should be used to keep data.</span></span> <span data-ttu-id="93258-113">例如，如果日期是 2005 年 4 月 2 日并将特殊性设置为“月”，则筛选操作将保留包含 2009 年 4 月日期的所有行。</span><span class="sxs-lookup"><span data-stu-id="93258-113">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: , , , , , .</span></span> <span data-ttu-id="93258-114">可取值为：`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。</span><span class="sxs-lookup"><span data-stu-id="93258-114">The possible values are `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="93258-115">关系</span><span class="sxs-lookup"><span data-stu-id="93258-115">Relationships</span></span>
<span data-ttu-id="93258-116">无</span><span class="sxs-lookup"><span data-stu-id="93258-116">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="93258-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93258-117">JSON representation</span></span>

<span data-ttu-id="93258-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93258-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->