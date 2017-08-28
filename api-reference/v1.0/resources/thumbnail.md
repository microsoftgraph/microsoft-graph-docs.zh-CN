# <a name="thumbnail-resource-type"></a><span data-ttu-id="1faf3-101">缩略图资源类型</span><span class="sxs-lookup"><span data-stu-id="1faf3-101">Thumbnail resource type</span></span>

<span data-ttu-id="1faf3-102">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="1faf3-102">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1faf3-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1faf3-103">JSON representation</span></span>

<span data-ttu-id="1faf3-104">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1faf3-104">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="1faf3-105">属性</span><span class="sxs-lookup"><span data-stu-id="1faf3-105">Properties</span></span>

| <span data-ttu-id="1faf3-106">属性</span><span class="sxs-lookup"><span data-stu-id="1faf3-106">Property</span></span>     | <span data-ttu-id="1faf3-107">类型</span><span class="sxs-lookup"><span data-stu-id="1faf3-107">Type</span></span>   | <span data-ttu-id="1faf3-108">说明</span><span class="sxs-lookup"><span data-stu-id="1faf3-108">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1faf3-109">height</span><span class="sxs-lookup"><span data-stu-id="1faf3-109">height</span></span>       | <span data-ttu-id="1faf3-110">Int32</span><span class="sxs-lookup"><span data-stu-id="1faf3-110">Int32</span></span>  | <span data-ttu-id="1faf3-111">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="1faf3-111">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="1faf3-112">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="1faf3-112">sourceItemId</span></span> | <span data-ttu-id="1faf3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1faf3-113">String</span></span> | <span data-ttu-id="1faf3-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="1faf3-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="1faf3-116">url</span><span class="sxs-lookup"><span data-stu-id="1faf3-116">url</span></span>          | <span data-ttu-id="1faf3-117">String</span><span class="sxs-lookup"><span data-stu-id="1faf3-117">String</span></span> | <span data-ttu-id="1faf3-118">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="1faf3-118">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="1faf3-119">width</span><span class="sxs-lookup"><span data-stu-id="1faf3-119">width</span></span>        | <span data-ttu-id="1faf3-120">Int32</span><span class="sxs-lookup"><span data-stu-id="1faf3-120">Int32</span></span>  | <span data-ttu-id="1faf3-121">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="1faf3-121">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="1faf3-122">关系</span><span class="sxs-lookup"><span data-stu-id="1faf3-122">Relationships</span></span>

| <span data-ttu-id="1faf3-123">名称</span><span class="sxs-lookup"><span data-stu-id="1faf3-123">Name</span></span>    | <span data-ttu-id="1faf3-124">类型</span><span class="sxs-lookup"><span data-stu-id="1faf3-124">Type</span></span>   | <span data-ttu-id="1faf3-125">说明</span><span class="sxs-lookup"><span data-stu-id="1faf3-125">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="1faf3-126">内容</span><span class="sxs-lookup"><span data-stu-id="1faf3-126">content</span></span> | <span data-ttu-id="1faf3-127">流</span><span class="sxs-lookup"><span data-stu-id="1faf3-127">Stream</span></span> | <span data-ttu-id="1faf3-128">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="1faf3-128">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
