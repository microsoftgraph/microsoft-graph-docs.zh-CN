# <a name="formatprotection-resource-type"></a><span data-ttu-id="4cd6f-101">FormatProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cd6f-101">FormatProtection resource type</span></span>

<span data-ttu-id="4cd6f-102">表示对 range 对象的格式保护。</span><span class="sxs-lookup"><span data-stu-id="4cd6f-102">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="4cd6f-103">方法</span><span class="sxs-lookup"><span data-stu-id="4cd6f-103">Methods</span></span>

| <span data-ttu-id="4cd6f-104">方法</span><span class="sxs-lookup"><span data-stu-id="4cd6f-104">Method</span></span>           | <span data-ttu-id="4cd6f-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="4cd6f-105">Return Type</span></span>    |<span data-ttu-id="4cd6f-106">说明</span><span class="sxs-lookup"><span data-stu-id="4cd6f-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4cd6f-107">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="4cd6f-107">Get FormatProtection</span></span>](../api/formatprotection_get.md) | [<span data-ttu-id="4cd6f-108">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="4cd6f-108">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="4cd6f-109">读取 formatProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4cd6f-109">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="4cd6f-110">Update</span><span class="sxs-lookup"><span data-stu-id="4cd6f-110">Update</span></span>](../api/formatprotection_update.md) | [<span data-ttu-id="4cd6f-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="4cd6f-111">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="4cd6f-112">更新 FormatProtection 对象。</span><span class="sxs-lookup"><span data-stu-id="4cd6f-112">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4cd6f-113">属性</span><span class="sxs-lookup"><span data-stu-id="4cd6f-113">Properties</span></span>
| <span data-ttu-id="4cd6f-114">属性</span><span class="sxs-lookup"><span data-stu-id="4cd6f-114">Property</span></span>     | <span data-ttu-id="4cd6f-115">类型</span><span class="sxs-lookup"><span data-stu-id="4cd6f-115">Type</span></span>   |<span data-ttu-id="4cd6f-116">说明</span><span class="sxs-lookup"><span data-stu-id="4cd6f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cd6f-117">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="4cd6f-117">formulaHidden</span></span>|<span data-ttu-id="4cd6f-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="4cd6f-118">boolean</span></span>|<span data-ttu-id="4cd6f-p101">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="4cd6f-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="4cd6f-121">已锁定</span><span class="sxs-lookup"><span data-stu-id="4cd6f-121">locked</span></span>|<span data-ttu-id="4cd6f-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="4cd6f-122">boolean</span></span>|<span data-ttu-id="4cd6f-p102">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="4cd6f-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cd6f-125">关系</span><span class="sxs-lookup"><span data-stu-id="4cd6f-125">Relationships</span></span>
<span data-ttu-id="4cd6f-126">无</span><span class="sxs-lookup"><span data-stu-id="4cd6f-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4cd6f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cd6f-127">JSON representation</span></span>

<span data-ttu-id="4cd6f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cd6f-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->