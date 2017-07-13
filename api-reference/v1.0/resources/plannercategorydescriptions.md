<span data-ttu-id="2759d-p101">**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。</span><span class="sxs-lookup"><span data-stu-id="2759d-p101">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span>

**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。 


## <span data-ttu-id="2759d-105">属性</span><span class="sxs-lookup"><span data-stu-id="2759d-105">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="2759d-106">属性</span><span class="sxs-lookup"><span data-stu-id="2759d-106">Property</span></span>     | <span data-ttu-id="2759d-107">类型</span><span class="sxs-lookup"><span data-stu-id="2759d-107">Type</span></span>   |<span data-ttu-id="2759d-108">说明</span><span class="sxs-lookup"><span data-stu-id="2759d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2759d-109">category1</span><span class="sxs-lookup"><span data-stu-id="2759d-109">category1</span></span>|<span data-ttu-id="2759d-110">String</span><span class="sxs-lookup"><span data-stu-id="2759d-110">String</span></span>|<span data-ttu-id="2759d-111">与类别 1 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2759d-111">The label associated with Category 1</span></span>|
|<span data-ttu-id="2759d-112">category2</span><span class="sxs-lookup"><span data-stu-id="2759d-112">category2</span></span>|<span data-ttu-id="2759d-113">String</span><span class="sxs-lookup"><span data-stu-id="2759d-113">String</span></span>|<span data-ttu-id="2759d-114">与类别 2 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2759d-114">The label associated with Category 2</span></span>|
|<span data-ttu-id="2759d-115">category3</span><span class="sxs-lookup"><span data-stu-id="2759d-115">category3</span></span>|<span data-ttu-id="2759d-116">String</span><span class="sxs-lookup"><span data-stu-id="2759d-116">String</span></span>|<span data-ttu-id="2759d-117">与类别 3 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2759d-117">The label associated with Category 3</span></span>|
|<span data-ttu-id="2759d-118">category4</span><span class="sxs-lookup"><span data-stu-id="2759d-118">category4</span></span>|<span data-ttu-id="2759d-119">String</span><span class="sxs-lookup"><span data-stu-id="2759d-119">String</span></span>|<span data-ttu-id="2759d-120">与类别 4 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2759d-120">The label associated with Category 4</span></span>|
|<span data-ttu-id="2759d-121">category5</span><span class="sxs-lookup"><span data-stu-id="2759d-121">category5</span></span>|<span data-ttu-id="2759d-122">String</span><span class="sxs-lookup"><span data-stu-id="2759d-122">String</span></span>|<span data-ttu-id="2759d-123">与类别 5 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2759d-123">The label associated with Category 5</span></span>|
|<span data-ttu-id="2759d-124">category6</span><span class="sxs-lookup"><span data-stu-id="2759d-124">category6</span></span>|<span data-ttu-id="2759d-125">String</span><span class="sxs-lookup"><span data-stu-id="2759d-125">String</span></span>|<span data-ttu-id="2759d-126">与类别 6 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2759d-126">The label associated with Category 6</span></span>|

## <span data-ttu-id="2759d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2759d-127">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="2759d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2759d-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->