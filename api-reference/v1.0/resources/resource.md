# <a name="resource-resource-type"></a><span data-ttu-id="b0a38-101">资源资源类型</span><span class="sxs-lookup"><span data-stu-id="b0a38-101">resource resource type</span></span>

<span data-ttu-id="b0a38-102">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="b0a38-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="b0a38-103">可以获取资源的二进制数据，但是不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0a38-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="b0a38-104">可通过向资源的 `content` 终结点发送 GET 请求获取特定资源的二进制数据：</span><span class="sxs-lookup"><span data-stu-id="b0a38-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="b0a38-105">使用以下请求获取页面的 HTML 内容后将返回文件的资源 URI：</span><span class="sxs-lookup"><span data-stu-id="b0a38-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="b0a38-106">在页面 HTML 中，`img` 标记包含 `data-fullres-src` 属性中的原始图像资源和 `src` 属性中经过优化的图像的终结点。</span><span class="sxs-lookup"><span data-stu-id="b0a38-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="b0a38-107">`object` 标记（表示 PDF、DOCX 和 PNG 等文件）包含 `data` 属性中的文件资源的终结点：</span><span class="sxs-lookup"><span data-stu-id="b0a38-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="b0a38-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0a38-108">Properties</span></span>
<span data-ttu-id="b0a38-109">无。</span><span class="sxs-lookup"><span data-stu-id="b0a38-109">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="b0a38-110">关系</span><span class="sxs-lookup"><span data-stu-id="b0a38-110">Relationships</span></span>
<span data-ttu-id="b0a38-111">无。</span><span class="sxs-lookup"><span data-stu-id="b0a38-111">None.</span></span>


## <a name="methods"></a><span data-ttu-id="b0a38-112">方法</span><span class="sxs-lookup"><span data-stu-id="b0a38-112">Methods</span></span>
| <span data-ttu-id="b0a38-113">方法</span><span class="sxs-lookup"><span data-stu-id="b0a38-113">Method</span></span>           | <span data-ttu-id="b0a38-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0a38-114">Return Type</span></span>    |<span data-ttu-id="b0a38-115">说明</span><span class="sxs-lookup"><span data-stu-id="b0a38-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0a38-116">Get resource binary data</span><span class="sxs-lookup"><span data-stu-id="b0a38-116">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="b0a38-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b0a38-117">Stream</span></span> |<span data-ttu-id="b0a38-118">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="b0a38-118">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->