# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="74268-101">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="74268-101">teamFunSettings resource type</span></span>



<span data-ttu-id="74268-102">要配置的设置使用 Giphy、 memes 和[团队](team.md)中的标签。</span><span class="sxs-lookup"><span data-stu-id="74268-102">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="74268-103">属性</span><span class="sxs-lookup"><span data-stu-id="74268-103">Properties</span></span>
| <span data-ttu-id="74268-104">属性</span><span class="sxs-lookup"><span data-stu-id="74268-104">Property</span></span>     | <span data-ttu-id="74268-105">类型</span><span class="sxs-lookup"><span data-stu-id="74268-105">Type</span></span>   |<span data-ttu-id="74268-106">说明</span><span class="sxs-lookup"><span data-stu-id="74268-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74268-107">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="74268-107">allowGiphy</span></span>|<span data-ttu-id="74268-108">布尔</span><span class="sxs-lookup"><span data-stu-id="74268-108">Boolean</span></span>|<span data-ttu-id="74268-109">如果设置为 true，则启用 Giphy 使用。</span><span class="sxs-lookup"><span data-stu-id="74268-109">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="74268-110">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="74268-110">giphyContentRating</span></span>|<span data-ttu-id="74268-111">字符串 (enum)</span><span class="sxs-lookup"><span data-stu-id="74268-111">String (enum)</span></span>|<span data-ttu-id="74268-112">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="74268-112">Giphy content rating.</span></span> <span data-ttu-id="74268-113">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="74268-113">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="74268-114">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="74268-114">allowStickersAndMemes</span></span>|<span data-ttu-id="74268-115">布尔</span><span class="sxs-lookup"><span data-stu-id="74268-115">Boolean</span></span>|<span data-ttu-id="74268-116">如果设置为 true，使用户能够包括标签和 memes。</span><span class="sxs-lookup"><span data-stu-id="74268-116">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="74268-117">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="74268-117">allowCustomMemes</span></span>|<span data-ttu-id="74268-118">布尔</span><span class="sxs-lookup"><span data-stu-id="74268-118">Boolean</span></span>|<span data-ttu-id="74268-119">如果设置为 true，使用户能够包括自定义 memes。</span><span class="sxs-lookup"><span data-stu-id="74268-119">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74268-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74268-120">JSON representation</span></span>

<span data-ttu-id="74268-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74268-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
