# <a name="chartfont-resource-type"></a><span data-ttu-id="336a6-101">ChartFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="336a6-101">ChartFont resource type</span></span>

<span data-ttu-id="336a6-102">此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="336a6-102">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="336a6-103">方法</span><span class="sxs-lookup"><span data-stu-id="336a6-103">Methods</span></span>

| <span data-ttu-id="336a6-104">方法</span><span class="sxs-lookup"><span data-stu-id="336a6-104">Method</span></span>           | <span data-ttu-id="336a6-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="336a6-105">Return Type</span></span>    |<span data-ttu-id="336a6-106">说明</span><span class="sxs-lookup"><span data-stu-id="336a6-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="336a6-107">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="336a6-107">Get ChartFont</span></span>](../api/chartfont_get.md) | [<span data-ttu-id="336a6-108">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="336a6-108">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="336a6-109">读取 chartFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="336a6-109">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="336a6-110">更新</span><span class="sxs-lookup"><span data-stu-id="336a6-110">Update</span></span>](../api/chartfont_update.md) | [<span data-ttu-id="336a6-111">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="336a6-111">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="336a6-112">更新 ChartFont 对象。</span><span class="sxs-lookup"><span data-stu-id="336a6-112">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="336a6-113">属性</span><span class="sxs-lookup"><span data-stu-id="336a6-113">Properties</span></span>
| <span data-ttu-id="336a6-114">属性</span><span class="sxs-lookup"><span data-stu-id="336a6-114">Property</span></span>     | <span data-ttu-id="336a6-115">类型</span><span class="sxs-lookup"><span data-stu-id="336a6-115">Type</span></span>   |<span data-ttu-id="336a6-116">说明</span><span class="sxs-lookup"><span data-stu-id="336a6-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="336a6-117">bold</span><span class="sxs-lookup"><span data-stu-id="336a6-117">bold</span></span>|<span data-ttu-id="336a6-118">boolean</span><span class="sxs-lookup"><span data-stu-id="336a6-118">boolean</span></span>|<span data-ttu-id="336a6-119">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="336a6-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="336a6-120">color</span><span class="sxs-lookup"><span data-stu-id="336a6-120">color</span></span>|<span data-ttu-id="336a6-121">string</span><span class="sxs-lookup"><span data-stu-id="336a6-121">string</span></span>|<span data-ttu-id="336a6-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="336a6-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="336a6-125">italic</span><span class="sxs-lookup"><span data-stu-id="336a6-125">italic</span></span>|<span data-ttu-id="336a6-126">boolean</span><span class="sxs-lookup"><span data-stu-id="336a6-126">boolean</span></span>|<span data-ttu-id="336a6-127">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="336a6-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="336a6-128">name</span><span class="sxs-lookup"><span data-stu-id="336a6-128">name</span></span>|<span data-ttu-id="336a6-129">string</span><span class="sxs-lookup"><span data-stu-id="336a6-129">string</span></span>|<span data-ttu-id="336a6-130">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="336a6-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="336a6-131">大小</span><span class="sxs-lookup"><span data-stu-id="336a6-131">size</span></span>|<span data-ttu-id="336a6-132">double</span><span class="sxs-lookup"><span data-stu-id="336a6-132">double</span></span>|<span data-ttu-id="336a6-133">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="336a6-133">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="336a6-134">underline</span><span class="sxs-lookup"><span data-stu-id="336a6-134">underline</span></span>|<span data-ttu-id="336a6-135">string</span><span class="sxs-lookup"><span data-stu-id="336a6-135">string</span></span>|<span data-ttu-id="336a6-136">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="336a6-136">Returns or sets the type of underline applied to the font.</span></span> <span data-ttu-id="336a6-137">可取值为：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="336a6-137">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="336a6-138">关系</span><span class="sxs-lookup"><span data-stu-id="336a6-138">Relationships</span></span>
<span data-ttu-id="336a6-139">无</span><span class="sxs-lookup"><span data-stu-id="336a6-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="336a6-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="336a6-140">JSON representation</span></span>

<span data-ttu-id="336a6-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="336a6-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->