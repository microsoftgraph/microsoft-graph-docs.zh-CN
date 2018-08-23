# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="c7be9-101">onenoteEntityBaseModel 资源</span><span class="sxs-lookup"><span data-stu-id="c7be9-101">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="c7be9-102">这是 OneNote 实体的基础类型。</span><span class="sxs-lookup"><span data-stu-id="c7be9-102">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7be9-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7be9-103">JSON representation</span></span>

<span data-ttu-id="c7be9-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7be9-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c7be9-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7be9-105">Properties</span></span>
| <span data-ttu-id="c7be9-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7be9-106">Property</span></span>     | <span data-ttu-id="c7be9-107">类型</span><span class="sxs-lookup"><span data-stu-id="c7be9-107">Type</span></span>   |<span data-ttu-id="c7be9-108">说明</span><span class="sxs-lookup"><span data-stu-id="c7be9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7be9-109">self</span><span class="sxs-lookup"><span data-stu-id="c7be9-109">self</span></span>|<span data-ttu-id="c7be9-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c7be9-110">String</span></span>|<span data-ttu-id="c7be9-p101">可以在其中获取关于页面的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="c7be9-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->