# <a name="website-resource-type"></a><span data-ttu-id="ba391-101">website 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba391-101">website resource type</span></span>

<span data-ttu-id="ba391-102">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="ba391-102">Represents a wssnoversshort website.</span></span>


## <a name="properties"></a><span data-ttu-id="ba391-103">属性</span><span class="sxs-lookup"><span data-stu-id="ba391-103">Properties</span></span>
| <span data-ttu-id="ba391-104">属性</span><span class="sxs-lookup"><span data-stu-id="ba391-104">Property</span></span>     | <span data-ttu-id="ba391-105">类型</span><span class="sxs-lookup"><span data-stu-id="ba391-105">Type</span></span>   |<span data-ttu-id="ba391-106">说明</span><span class="sxs-lookup"><span data-stu-id="ba391-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba391-107">类型</span><span class="sxs-lookup"><span data-stu-id="ba391-107">type</span></span>|<span data-ttu-id="ba391-108">String</span><span class="sxs-lookup"><span data-stu-id="ba391-108">String</span></span>| <span data-ttu-id="ba391-109">可能的值是：`other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="ba391-109">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="ba391-110">address</span><span class="sxs-lookup"><span data-stu-id="ba391-110">address</span></span>|<span data-ttu-id="ba391-111">string</span><span class="sxs-lookup"><span data-stu-id="ba391-111">string</span></span>|<span data-ttu-id="ba391-112">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="ba391-112">The URL of the current website.</span></span>|
|<span data-ttu-id="ba391-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ba391-113">displayName</span></span>|<span data-ttu-id="ba391-114">string</span><span class="sxs-lookup"><span data-stu-id="ba391-114">string</span></span>|<span data-ttu-id="ba391-115">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba391-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba391-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba391-116">JSON representation</span></span>

<span data-ttu-id="ba391-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba391-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
