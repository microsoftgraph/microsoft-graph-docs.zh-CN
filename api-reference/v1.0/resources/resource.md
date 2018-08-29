# <a name="onenoteresource-resource-type"></a><span data-ttu-id="95866-101">OneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="95866-101">OneNoteResource resource type</span></span>

<span data-ttu-id="95866-102">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="95866-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="95866-103">可以获取资源的二进制数据，但是不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95866-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="95866-104">可通过向资源的 `content` 终结点发送 GET 请求获取特定资源的二进制数据：</span><span class="sxs-lookup"><span data-stu-id="95866-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="95866-105">使用以下请求获取页面的 HTML 内容后将返回文件的资源 URI：</span><span class="sxs-lookup"><span data-stu-id="95866-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="95866-106">在页面 HTML 中，`img` 标记包含 `data-fullres-src` 属性中的原始图像资源和 `src` 属性中经过优化的图像的终结点。</span><span class="sxs-lookup"><span data-stu-id="95866-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="95866-107">标记（表示 PDF、DOCX 和 PNG 等文件）包含 `data` 属性中的文件资源的终结点：`object`</span><span class="sxs-lookup"><span data-stu-id="95866-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="95866-108">属性</span><span class="sxs-lookup"><span data-stu-id="95866-108">Properties</span></span>

| <span data-ttu-id="95866-109">属性</span><span class="sxs-lookup"><span data-stu-id="95866-109">Property</span></span>             | <span data-ttu-id="95866-110">类型</span><span class="sxs-lookup"><span data-stu-id="95866-110">Type</span></span>            | <span data-ttu-id="95866-111">说明</span><span class="sxs-lookup"><span data-stu-id="95866-111">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="95866-112">内容</span><span class="sxs-lookup"><span data-stu-id="95866-112">content</span></span>              | <span data-ttu-id="95866-113">流</span><span class="sxs-lookup"><span data-stu-id="95866-113">Stream</span></span>          | <span data-ttu-id="95866-114">内容流</span><span class="sxs-lookup"><span data-stu-id="95866-114">The content stream.</span></span>
| <span data-ttu-id="95866-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="95866-115">contentUrl</span></span>           | <span data-ttu-id="95866-116">string (url)</span><span class="sxs-lookup"><span data-stu-id="95866-116">string (url)</span></span>    | <span data-ttu-id="95866-117">用于下载内容的 URL</span><span class="sxs-lookup"><span data-stu-id="95866-117">The URL for the page's HTML content.  Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="95866-118">关系</span><span class="sxs-lookup"><span data-stu-id="95866-118">Relationships</span></span>
<span data-ttu-id="95866-119">无。</span><span class="sxs-lookup"><span data-stu-id="95866-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="95866-120">方法</span><span class="sxs-lookup"><span data-stu-id="95866-120">Methods</span></span>
| <span data-ttu-id="95866-121">方法</span><span class="sxs-lookup"><span data-stu-id="95866-121">Method</span></span>           | <span data-ttu-id="95866-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="95866-122">Return Type</span></span>    |<span data-ttu-id="95866-123">说明</span><span class="sxs-lookup"><span data-stu-id="95866-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95866-124">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="95866-124">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="95866-125">流</span><span class="sxs-lookup"><span data-stu-id="95866-125">Stream</span></span> |<span data-ttu-id="95866-126">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="95866-126">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->