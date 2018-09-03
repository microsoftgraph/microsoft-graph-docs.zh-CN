# <a name="website-resource-type"></a><span data-ttu-id="8e5f0-101">website 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e5f0-101">website resource type</span></span>

<span data-ttu-id="8e5f0-102">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="8e5f0-102">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="8e5f0-103">属性</span><span class="sxs-lookup"><span data-stu-id="8e5f0-103">Properties</span></span>
| <span data-ttu-id="8e5f0-104">属性</span><span class="sxs-lookup"><span data-stu-id="8e5f0-104">Property</span></span>     | <span data-ttu-id="8e5f0-105">类型</span><span class="sxs-lookup"><span data-stu-id="8e5f0-105">Type</span></span>   |<span data-ttu-id="8e5f0-106">说明</span><span class="sxs-lookup"><span data-stu-id="8e5f0-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e5f0-107">type</span><span class="sxs-lookup"><span data-stu-id="8e5f0-107">type</span></span>|<span data-ttu-id="8e5f0-108">websiteType</span><span class="sxs-lookup"><span data-stu-id="8e5f0-108">WebsiteType</span></span>| <span data-ttu-id="8e5f0-109">可取值为：`other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="8e5f0-109">The possible values are `other`, `home`, `work`, `blog`, `profile`, , , , , , , or .</span></span>|
|<span data-ttu-id="8e5f0-110">address</span><span class="sxs-lookup"><span data-stu-id="8e5f0-110">address</span></span>|<span data-ttu-id="8e5f0-111">string</span><span class="sxs-lookup"><span data-stu-id="8e5f0-111">string</span></span>|<span data-ttu-id="8e5f0-112">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="8e5f0-112">The URL of the website.</span></span>|
|<span data-ttu-id="8e5f0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="8e5f0-113">displayName</span></span>|<span data-ttu-id="8e5f0-114">string</span><span class="sxs-lookup"><span data-stu-id="8e5f0-114">string</span></span>|<span data-ttu-id="8e5f0-115">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8e5f0-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e5f0-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e5f0-116">JSON representation</span></span>

<span data-ttu-id="8e5f0-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e5f0-117">The following is a JSON representation of the resource.</span></span>

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
