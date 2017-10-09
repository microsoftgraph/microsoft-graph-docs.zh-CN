# <a name="persontype-resource-type"></a><span data-ttu-id="cafd7-101">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="cafd7-101">personType resource type</span></span>

<span data-ttu-id="cafd7-102">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="cafd7-102">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cafd7-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cafd7-103">JSON representation</span></span>

<span data-ttu-id="cafd7-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cafd7-104">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="cafd7-105">属性</span><span class="sxs-lookup"><span data-stu-id="cafd7-105">Properties</span></span>
| <span data-ttu-id="cafd7-106">属性</span><span class="sxs-lookup"><span data-stu-id="cafd7-106">Property</span></span>     | <span data-ttu-id="cafd7-107">类型</span><span class="sxs-lookup"><span data-stu-id="cafd7-107">Type</span></span>   |<span data-ttu-id="cafd7-108">说明</span><span class="sxs-lookup"><span data-stu-id="cafd7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cafd7-109">class</span><span class="sxs-lookup"><span data-stu-id="cafd7-109">class</span></span>|<span data-ttu-id="cafd7-110">String</span><span class="sxs-lookup"><span data-stu-id="cafd7-110">String</span></span>|<span data-ttu-id="cafd7-111">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="cafd7-111">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="cafd7-112">subclass</span><span class="sxs-lookup"><span data-stu-id="cafd7-112">subclass</span></span>|<span data-ttu-id="cafd7-113">String</span><span class="sxs-lookup"><span data-stu-id="cafd7-113">String</span></span>|<span data-ttu-id="cafd7-114">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="cafd7-114">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persontype resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
