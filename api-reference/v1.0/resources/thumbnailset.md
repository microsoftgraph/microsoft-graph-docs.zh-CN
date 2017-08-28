# <a name="thumbnailset-resource-type"></a><span data-ttu-id="0c860-101">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c860-101">ThumbnailSet resource type</span></span>

<span data-ttu-id="0c860-p101">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="0c860-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c860-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c860-104">JSON representation</span></span>

<span data-ttu-id="0c860-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c860-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": {"@odata.type": "microsoft.graph.thumbnail"},
  "medium": {"@odata.type": "microsoft.graph.thumbnail"},
  "small": {"@odata.type": "microsoft.graph.thumbnail"},
  "source": {"@odata.type": "microsoft.graph.thumbnail"}
}
```

## <a name="properties"></a><span data-ttu-id="0c860-106">属性</span><span class="sxs-lookup"><span data-stu-id="0c860-106">Properties</span></span>

| <span data-ttu-id="0c860-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c860-107">Property</span></span> | <span data-ttu-id="0c860-108">类型</span><span class="sxs-lookup"><span data-stu-id="0c860-108">Type</span></span>                      | <span data-ttu-id="0c860-109">说明</span><span class="sxs-lookup"><span data-stu-id="0c860-109">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="0c860-110">id</span><span class="sxs-lookup"><span data-stu-id="0c860-110">id</span></span>       | <span data-ttu-id="0c860-111">String</span><span class="sxs-lookup"><span data-stu-id="0c860-111">String</span></span>                    | <span data-ttu-id="0c860-p102">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="0c860-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="0c860-114">大</span><span class="sxs-lookup"><span data-stu-id="0c860-114">large</span></span>    | [<span data-ttu-id="0c860-115">缩略图</span><span class="sxs-lookup"><span data-stu-id="0c860-115">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="0c860-116">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0c860-116">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="0c860-117">中等</span><span class="sxs-lookup"><span data-stu-id="0c860-117">medium</span></span>   | [<span data-ttu-id="0c860-118">缩略图</span><span class="sxs-lookup"><span data-stu-id="0c860-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="0c860-119">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0c860-119">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="0c860-120">小</span><span class="sxs-lookup"><span data-stu-id="0c860-120">small</span></span>    | [<span data-ttu-id="0c860-121">缩略图</span><span class="sxs-lookup"><span data-stu-id="0c860-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="0c860-122">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="0c860-122">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="0c860-123">源</span><span class="sxs-lookup"><span data-stu-id="0c860-123">source</span></span>   | [<span data-ttu-id="0c860-124">缩略图</span><span class="sxs-lookup"><span data-stu-id="0c860-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="0c860-125">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="0c860-125">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnailSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
