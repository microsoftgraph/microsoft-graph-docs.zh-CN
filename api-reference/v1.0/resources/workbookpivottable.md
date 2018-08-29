# <a name="pivottable-resource-type"></a><span data-ttu-id="7d4a9-101">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d4a9-101">pivotTable resource type</span></span>

<span data-ttu-id="7d4a9-102">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-102">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="7d4a9-103">方法</span><span class="sxs-lookup"><span data-stu-id="7d4a9-103">Methods</span></span>

| <span data-ttu-id="7d4a9-104">方法</span><span class="sxs-lookup"><span data-stu-id="7d4a9-104">Method</span></span>           | <span data-ttu-id="7d4a9-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d4a9-105">Return Type</span></span>    |<span data-ttu-id="7d4a9-106">说明</span><span class="sxs-lookup"><span data-stu-id="7d4a9-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d4a9-107">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="7d4a9-107">Get workbookPivotTable</span></span>](../api/workbookpivottable_get.md) | [<span data-ttu-id="7d4a9-108">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="7d4a9-108">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="7d4a9-109">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-109">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="7d4a9-110">Refresh</span><span class="sxs-lookup"><span data-stu-id="7d4a9-110">Refresh</span></span>](../api/workbookpivottable_refresh.md)|<span data-ttu-id="7d4a9-111">无</span><span class="sxs-lookup"><span data-stu-id="7d4a9-111">None</span></span>|<span data-ttu-id="7d4a9-112">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-112">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="7d4a9-113">Refreshall</span><span class="sxs-lookup"><span data-stu-id="7d4a9-113">Refreshall</span></span>](../api/workbookpivottable_refreshall.md)|<span data-ttu-id="7d4a9-114">无</span><span class="sxs-lookup"><span data-stu-id="7d4a9-114">None</span></span>|<span data-ttu-id="7d4a9-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d4a9-117">属性</span><span class="sxs-lookup"><span data-stu-id="7d4a9-117">Properties</span></span>
| <span data-ttu-id="7d4a9-118">属性</span><span class="sxs-lookup"><span data-stu-id="7d4a9-118">Property</span></span>     | <span data-ttu-id="7d4a9-119">类型</span><span class="sxs-lookup"><span data-stu-id="7d4a9-119">Type</span></span>   |<span data-ttu-id="7d4a9-120">说明</span><span class="sxs-lookup"><span data-stu-id="7d4a9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d4a9-121">id</span><span class="sxs-lookup"><span data-stu-id="7d4a9-121">id</span></span>|<span data-ttu-id="7d4a9-122">字符串</span><span class="sxs-lookup"><span data-stu-id="7d4a9-122">String</span></span>| <span data-ttu-id="7d4a9-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="7d4a9-125">name</span><span class="sxs-lookup"><span data-stu-id="7d4a9-125">name</span></span>|<span data-ttu-id="7d4a9-126">字符串</span><span class="sxs-lookup"><span data-stu-id="7d4a9-126">String</span></span>|<span data-ttu-id="7d4a9-127">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-127">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="7d4a9-128">关系</span><span class="sxs-lookup"><span data-stu-id="7d4a9-128">Relationships</span></span>
| <span data-ttu-id="7d4a9-129">关系</span><span class="sxs-lookup"><span data-stu-id="7d4a9-129">Relationship</span></span> | <span data-ttu-id="7d4a9-130">类型</span><span class="sxs-lookup"><span data-stu-id="7d4a9-130">Type</span></span>   |<span data-ttu-id="7d4a9-131">说明</span><span class="sxs-lookup"><span data-stu-id="7d4a9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d4a9-132">worksheet</span><span class="sxs-lookup"><span data-stu-id="7d4a9-132">worksheet</span></span>|[<span data-ttu-id="7d4a9-133">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="7d4a9-133">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="7d4a9-p103">包含当前 PivotTable 对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="7d4a9-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d4a9-136">JSON representation</span></span>
<span data-ttu-id="7d4a9-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d4a9-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
