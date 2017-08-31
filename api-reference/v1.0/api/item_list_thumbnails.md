# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="c9657-101">列出 DriveItem 的缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="c9657-102">检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="c9657-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="c9657-p101">DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。</span><span class="sxs-lookup"><span data-stu-id="c9657-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="c9657-p102">可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：</span><span class="sxs-lookup"><span data-stu-id="c9657-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="c9657-108">枚举项目的可用缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="c9657-109">检索项目的单个缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="c9657-110">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="c9657-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="c9657-111">在单个请求中检索多个项目的缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="c9657-112">检索自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="c9657-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="c9657-113">上载项目的自定义缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="c9657-114">确定是否存在自定义的上传缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="c9657-115">权限</span><span class="sxs-lookup"><span data-stu-id="c9657-115">Permissions</span></span>
<span data-ttu-id="c9657-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c9657-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c9657-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9657-118">Permission type</span></span>      | <span data-ttu-id="c9657-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9657-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9657-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9657-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c9657-121">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9657-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9657-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9657-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9657-123">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9657-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9657-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9657-124">Application</span></span> | <span data-ttu-id="c9657-125">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9657-125">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9657-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9657-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9657-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c9657-127">Optional query parameters</span></span>
<span data-ttu-id="c9657-128">此方法支持使用 `$select`[OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c9657-128">This method supports the `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="c9657-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9657-129">Request body</span></span>
<span data-ttu-id="c9657-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9657-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9657-131">响应</span><span class="sxs-lookup"><span data-stu-id="c9657-131">Response</span></span>

<span data-ttu-id="c9657-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c9657-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9657-133">示例</span><span class="sxs-lookup"><span data-stu-id="c9657-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9657-134">请求</span><span class="sxs-lookup"><span data-stu-id="c9657-134">Request</span></span>

<span data-ttu-id="c9657-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9657-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="c9657-136">响应</span><span class="sxs-lookup"><span data-stu-id="c9657-136">Response</span></span>
<span data-ttu-id="c9657-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c9657-137">Here is an example of the response.</span></span>

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

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="c9657-138">检索单个缩略图</span><span class="sxs-lookup"><span data-stu-id="c9657-138">Retrieve a single thumbnail</span></span>

<span data-ttu-id="c9657-139">通过请求中直接解决来检索单个缩略图和大小的元数据。</span><span class="sxs-lookup"><span data-stu-id="c9657-139">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9657-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9657-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="c9657-141">Path 参数</span><span class="sxs-lookup"><span data-stu-id="c9657-141">Path parameters</span></span>

| <span data-ttu-id="c9657-142">名称</span><span class="sxs-lookup"><span data-stu-id="c9657-142">Name</span></span>         | <span data-ttu-id="c9657-143">类型</span><span class="sxs-lookup"><span data-stu-id="c9657-143">Type</span></span>   | <span data-ttu-id="c9657-144">说明</span><span class="sxs-lookup"><span data-stu-id="c9657-144">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="c9657-145">**item-id**</span><span class="sxs-lookup"><span data-stu-id="c9657-145">**item-id**</span></span>  | <span data-ttu-id="c9657-146">string</span><span class="sxs-lookup"><span data-stu-id="c9657-146">string</span></span> | <span data-ttu-id="c9657-147">引用的项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c9657-147">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="c9657-148">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="c9657-148">**thumb-id**</span></span> | <span data-ttu-id="c9657-149">数字</span><span class="sxs-lookup"><span data-stu-id="c9657-149">number</span></span> | <span data-ttu-id="c9657-150">缩略图的索引，通常为 0 到 4。</span><span class="sxs-lookup"><span data-stu-id="c9657-150">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="c9657-151">**size**</span><span class="sxs-lookup"><span data-stu-id="c9657-151">**size**</span></span>     | <span data-ttu-id="c9657-152">string</span><span class="sxs-lookup"><span data-stu-id="c9657-152">string</span></span> | <span data-ttu-id="c9657-p104">请求的缩略图大小。这必须是列出的其中一个标准大小。</span><span class="sxs-lookup"><span data-stu-id="c9657-p104">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |

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

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="c9657-155">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="c9657-155">Retrieve thumbnail content</span></span>

<span data-ttu-id="c9657-156">可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。</span><span class="sxs-lookup"><span data-stu-id="c9657-156">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9657-157">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9657-157">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="c9657-158">响应</span><span class="sxs-lookup"><span data-stu-id="c9657-158">Response</span></span>

<span data-ttu-id="c9657-159">本服务用到缩略图 URL 的重定向进行响应。</span><span class="sxs-lookup"><span data-stu-id="c9657-159">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="c9657-p105">缩略图的内容 URL 已经过预身份验证，无需下载授权标头。这些 URL 是临时存在的，仅在数小时内有效，不应由应用进行缓存。</span><span class="sxs-lookup"><span data-stu-id="c9657-p105">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="c9657-162">Size 的值</span><span class="sxs-lookup"><span data-stu-id="c9657-162">Size values</span></span>

<span data-ttu-id="c9657-p106">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="c9657-p106">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="c9657-165">名称</span><span class="sxs-lookup"><span data-stu-id="c9657-165">Name</span></span>           | <span data-ttu-id="c9657-166">分辨率</span><span class="sxs-lookup"><span data-stu-id="c9657-166">Resolution</span></span>  | <span data-ttu-id="c9657-167">纵横比​​</span><span class="sxs-lookup"><span data-stu-id="c9657-167">Aspect Ratio</span></span> | <span data-ttu-id="c9657-168">说明</span><span class="sxs-lookup"><span data-stu-id="c9657-168">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="c9657-169">96 longest</span><span class="sxs-lookup"><span data-stu-id="c9657-169">96 longest</span></span>  | <span data-ttu-id="c9657-170">Original</span><span class="sxs-lookup"><span data-stu-id="c9657-170">Original</span></span>     | <span data-ttu-id="c9657-171">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="c9657-171">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="c9657-172">176 longest</span><span class="sxs-lookup"><span data-stu-id="c9657-172">176 longest</span></span> | <span data-ttu-id="c9657-173">Original</span><span class="sxs-lookup"><span data-stu-id="c9657-173">Original</span></span>     | <span data-ttu-id="c9657-174">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="c9657-174">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="c9657-175">800 longest
</span><span class="sxs-lookup"><span data-stu-id="c9657-175">800 longest</span></span> | <span data-ttu-id="c9657-176">Original</span><span class="sxs-lookup"><span data-stu-id="c9657-176">Original</span></span>     | <span data-ttu-id="c9657-177">最长边调整到 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="c9657-177">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="c9657-178">注解</span><span class="sxs-lookup"><span data-stu-id="c9657-178">Remarks</span></span>

<span data-ttu-id="c9657-179">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="c9657-179">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="c9657-180">使用这些调用展开缩略图集合不适用于：`GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="c9657-180">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
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
