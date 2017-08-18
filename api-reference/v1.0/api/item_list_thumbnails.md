# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="f592b-101">列出 DriveItem 的缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="f592b-102">检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="f592b-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="f592b-p101">DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。</span><span class="sxs-lookup"><span data-stu-id="f592b-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="f592b-p102">可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：</span><span class="sxs-lookup"><span data-stu-id="f592b-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="f592b-108">枚举项目的可用缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="f592b-109">检索项目的单个缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="f592b-110">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="f592b-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="f592b-111">在单个请求中检索多个项目的缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="f592b-112">检索自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="f592b-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="f592b-113">上载项目的自定义缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="f592b-114">确定是否存在自定义的上载缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="prerequisites"></a><span data-ttu-id="f592b-115">先决条件</span><span class="sxs-lookup"><span data-stu-id="f592b-115">Prerequisites</span></span>
<span data-ttu-id="f592b-116">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="f592b-116">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="f592b-117">Files.Read</span><span class="sxs-lookup"><span data-stu-id="f592b-117">Files.Read</span></span>
* <span data-ttu-id="f592b-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f592b-118">Files.ReadWrite</span></span>
* <span data-ttu-id="f592b-119">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="f592b-119">Files.Read.All</span></span>
* <span data-ttu-id="f592b-120">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f592b-120">Files.ReadWrite.All</span></span>
* <span data-ttu-id="f592b-121">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f592b-121">Sites.Read.All</span></span>
* <span data-ttu-id="f592b-122">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f592b-122">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="f592b-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f592b-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f592b-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f592b-124">Optional query parameters</span></span>
<span data-ttu-id="f592b-125">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f592b-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="f592b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f592b-126">Request body</span></span>
<span data-ttu-id="f592b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f592b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f592b-128">响应</span><span class="sxs-lookup"><span data-stu-id="f592b-128">Response</span></span>

<span data-ttu-id="f592b-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f592b-129">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f592b-130">示例</span><span class="sxs-lookup"><span data-stu-id="f592b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f592b-131">请求</span><span class="sxs-lookup"><span data-stu-id="f592b-131">Request</span></span>

<span data-ttu-id="f592b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f592b-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="f592b-133">响应</span><span class="sxs-lookup"><span data-stu-id="f592b-133">Response</span></span>
<span data-ttu-id="f592b-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f592b-134">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="f592b-135">检索单个缩略图</span><span class="sxs-lookup"><span data-stu-id="f592b-135">Retrieve a single thumbnail</span></span>

<span data-ttu-id="f592b-136">通过请求中直接解决来检索单个缩略图和大小的元数据。</span><span class="sxs-lookup"><span data-stu-id="f592b-136">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="f592b-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f592b-137">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="f592b-138">Path 参数</span><span class="sxs-lookup"><span data-stu-id="f592b-138">Path parameters</span></span>

| <span data-ttu-id="f592b-139">名称</span><span class="sxs-lookup"><span data-stu-id="f592b-139">Name</span></span>         | <span data-ttu-id="f592b-140">类型</span><span class="sxs-lookup"><span data-stu-id="f592b-140">Type</span></span>   | <span data-ttu-id="f592b-141">说明</span><span class="sxs-lookup"><span data-stu-id="f592b-141">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="f592b-142">**item-id**</span><span class="sxs-lookup"><span data-stu-id="f592b-142">**item-id**</span></span>  | <span data-ttu-id="f592b-143">string</span><span class="sxs-lookup"><span data-stu-id="f592b-143">string</span></span> | <span data-ttu-id="f592b-144">引用的项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f592b-144">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="f592b-145">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="f592b-145">**thumb-id**</span></span> | <span data-ttu-id="f592b-146">数字</span><span class="sxs-lookup"><span data-stu-id="f592b-146">number</span></span> | <span data-ttu-id="f592b-147">缩略图的索引，通常为 0 到 4。</span><span class="sxs-lookup"><span data-stu-id="f592b-147">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="f592b-148">**size**</span><span class="sxs-lookup"><span data-stu-id="f592b-148">**size**</span></span>     | <span data-ttu-id="f592b-149">string</span><span class="sxs-lookup"><span data-stu-id="f592b-149">string</span></span> | <span data-ttu-id="f592b-p103">请求的缩略图大小。这必须是列出的其中一个标准大小。</span><span class="sxs-lookup"><span data-stu-id="f592b-p103">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="f592b-152">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="f592b-152">Retrieve thumbnail content</span></span>

<span data-ttu-id="f592b-153">可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。</span><span class="sxs-lookup"><span data-stu-id="f592b-153">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="f592b-154">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f592b-154">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="f592b-155">响应</span><span class="sxs-lookup"><span data-stu-id="f592b-155">Response</span></span>

<span data-ttu-id="f592b-156">本服务用到缩略图 URL 的重定向进行响应。</span><span class="sxs-lookup"><span data-stu-id="f592b-156">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="f592b-p104">缩略图的内容 URL 已经过预身份验证，无需下载授权标头。这些 URL 是临时存在的，仅在数小时内有效，不应由应用进行缓存。</span><span class="sxs-lookup"><span data-stu-id="f592b-p104">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="f592b-159">Size 的值</span><span class="sxs-lookup"><span data-stu-id="f592b-159">Size values</span></span>

<span data-ttu-id="f592b-p105">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="f592b-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="f592b-162">名称</span><span class="sxs-lookup"><span data-stu-id="f592b-162">Name</span></span>           | <span data-ttu-id="f592b-163">分辨率</span><span class="sxs-lookup"><span data-stu-id="f592b-163">Resolution</span></span>  | <span data-ttu-id="f592b-164">纵横比​​</span><span class="sxs-lookup"><span data-stu-id="f592b-164">Aspect Ratio</span></span> | <span data-ttu-id="f592b-165">说明</span><span class="sxs-lookup"><span data-stu-id="f592b-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="f592b-166">96 longest</span><span class="sxs-lookup"><span data-stu-id="f592b-166">96 longest</span></span>  | <span data-ttu-id="f592b-167">Original</span><span class="sxs-lookup"><span data-stu-id="f592b-167">Original</span></span>     | <span data-ttu-id="f592b-168">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="f592b-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="f592b-169">176 longest</span><span class="sxs-lookup"><span data-stu-id="f592b-169">176 longest</span></span> | <span data-ttu-id="f592b-170">Original</span><span class="sxs-lookup"><span data-stu-id="f592b-170">Original</span></span>     | <span data-ttu-id="f592b-171">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="f592b-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="f592b-172">800 longest
</span><span class="sxs-lookup"><span data-stu-id="f592b-172">800 longest</span></span> | <span data-ttu-id="f592b-173">Original</span><span class="sxs-lookup"><span data-stu-id="f592b-173">Original</span></span>     | <span data-ttu-id="f592b-174">最长边调整到 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="f592b-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="f592b-175">注解</span><span class="sxs-lookup"><span data-stu-id="f592b-175">Remarks</span></span>

<span data-ttu-id="f592b-176">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="f592b-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="f592b-177">使用这些调用展开缩略图集合不适用于：`GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="f592b-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
