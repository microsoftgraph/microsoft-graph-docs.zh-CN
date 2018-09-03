# <a name="rangesort-resource-type"></a><span data-ttu-id="3f2ce-101">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f2ce-101">RangeSort resource type</span></span>

<span data-ttu-id="3f2ce-102">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="3f2ce-102">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="3f2ce-103">方法</span><span class="sxs-lookup"><span data-stu-id="3f2ce-103">Methods</span></span>

| <span data-ttu-id="3f2ce-104">方法</span><span class="sxs-lookup"><span data-stu-id="3f2ce-104">Method</span></span>           | <span data-ttu-id="3f2ce-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f2ce-105">Return Type</span></span>    |<span data-ttu-id="3f2ce-106">说明</span><span class="sxs-lookup"><span data-stu-id="3f2ce-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f2ce-107">Apply</span><span class="sxs-lookup"><span data-stu-id="3f2ce-107">Apply</span></span>](../api/rangesort_apply.md)|<span data-ttu-id="3f2ce-108">无</span><span class="sxs-lookup"><span data-stu-id="3f2ce-108">None</span></span>|<span data-ttu-id="3f2ce-109">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="3f2ce-109">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f2ce-110">属性</span><span class="sxs-lookup"><span data-stu-id="3f2ce-110">Properties</span></span>
<span data-ttu-id="3f2ce-111">无</span><span class="sxs-lookup"><span data-stu-id="3f2ce-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3f2ce-112">关系</span><span class="sxs-lookup"><span data-stu-id="3f2ce-112">Relationships</span></span>
<span data-ttu-id="3f2ce-113">无</span><span class="sxs-lookup"><span data-stu-id="3f2ce-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f2ce-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f2ce-114">JSON representation</span></span>

<span data-ttu-id="3f2ce-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f2ce-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="3f2ce-116">请求</span><span class="sxs-lookup"><span data-stu-id="3f2ce-116">Request</span></span>
<span data-ttu-id="3f2ce-117">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f2ce-117">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="3f2ce-118">响应</span><span class="sxs-lookup"><span data-stu-id="3f2ce-118">Response</span></span>
<span data-ttu-id="3f2ce-119">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3f2ce-119">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->