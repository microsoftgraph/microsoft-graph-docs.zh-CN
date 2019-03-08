---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 检索文件或文件夹的缩略图
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e58cdf153ea1fab98eac1a903e402d80228be5d4
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482173"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="0be0d-102">列出 DriveItem 的缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-102">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="0be0d-103">检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="0be0d-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="0be0d-p101">DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。</span><span class="sxs-lookup"><span data-stu-id="0be0d-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="0be0d-p102">可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：</span><span class="sxs-lookup"><span data-stu-id="0be0d-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="0be0d-109">枚举项目的可用缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="0be0d-110">检索项目的单个缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="0be0d-111">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="0be0d-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="0be0d-112">在单个请求中检索多个项目的缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="0be0d-113">检索自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="0be0d-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="0be0d-114">上载项目的自定义缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="0be0d-115">确定是否存在自定义的上传缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-115">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="0be0d-116">权限</span><span class="sxs-lookup"><span data-stu-id="0be0d-116">Permissions</span></span>

<span data-ttu-id="0be0d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0be0d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be0d-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="0be0d-119">Permission type</span></span>      | <span data-ttu-id="0be0d-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0be0d-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0be0d-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0be0d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="0be0d-122">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be0d-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0be0d-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0be0d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0be0d-124">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be0d-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0be0d-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="0be0d-125">Application</span></span> | <span data-ttu-id="0be0d-126">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be0d-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0be0d-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0be0d-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0be0d-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0be0d-128">Optional query parameters</span></span>

<span data-ttu-id="0be0d-129">此方法支持使用 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0be0d-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="0be0d-130">响应</span><span class="sxs-lookup"><span data-stu-id="0be0d-130">Response</span></span>

<span data-ttu-id="0be0d-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0be0d-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be0d-132">示例</span><span class="sxs-lookup"><span data-stu-id="0be0d-132">Example</span></span>

<span data-ttu-id="0be0d-133">下面是检索当前用户的 OneDrive 中某个项的可用缩略图的请求示例。</span><span class="sxs-lookup"><span data-stu-id="0be0d-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="0be0d-134">这将返回项的可用 **thumbnailSet** 的数组。</span><span class="sxs-lookup"><span data-stu-id="0be0d-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="0be0d-135">驱动器中的任何项都可以有零个或多个缩略图。</span><span class="sxs-lookup"><span data-stu-id="0be0d-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="0be0d-p105">**注意：** 可以使用 _select_ 查询字符串参数，控制在 **ThumbnailSet** 中返回的缩略图尺寸。 例如，`/thumbnails?select=medium` 仅检索中等大小的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0be0d-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="0be0d-138">响应</span><span class="sxs-lookup"><span data-stu-id="0be0d-138">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="0be0d-139">获取单个缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-139">Get a single thumbnail</span></span>

<span data-ttu-id="0be0d-140">通过直接在请求中对其进行寻址来检索单个缩略图和大小的元数据。</span><span class="sxs-lookup"><span data-stu-id="0be0d-140">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="0be0d-141">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0be0d-141">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="0be0d-142">Path 参数</span><span class="sxs-lookup"><span data-stu-id="0be0d-142">Path parameters</span></span>

| <span data-ttu-id="0be0d-143">名称</span><span class="sxs-lookup"><span data-stu-id="0be0d-143">Name</span></span>         | <span data-ttu-id="0be0d-144">类型</span><span class="sxs-lookup"><span data-stu-id="0be0d-144">Type</span></span>   | <span data-ttu-id="0be0d-145">说明</span><span class="sxs-lookup"><span data-stu-id="0be0d-145">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="0be0d-146">**item-id**</span><span class="sxs-lookup"><span data-stu-id="0be0d-146">**item-id**</span></span>  | <span data-ttu-id="0be0d-147">string</span><span class="sxs-lookup"><span data-stu-id="0be0d-147">string</span></span> | <span data-ttu-id="0be0d-148">引用的项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0be0d-148">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="0be0d-149">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="0be0d-149">**thumb-id**</span></span> | <span data-ttu-id="0be0d-150">数字</span><span class="sxs-lookup"><span data-stu-id="0be0d-150">number</span></span> | <span data-ttu-id="0be0d-p106">缩略图的索引，通常介于 0 到 4 之间。 如果没有自定义缩略图，索引为 0。</span><span class="sxs-lookup"><span data-stu-id="0be0d-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="0be0d-153">**size**</span><span class="sxs-lookup"><span data-stu-id="0be0d-153">**size**</span></span>     | <span data-ttu-id="0be0d-154">string</span><span class="sxs-lookup"><span data-stu-id="0be0d-154">string</span></span> | <span data-ttu-id="0be0d-155">请求获取的缩略图的大小。</span><span class="sxs-lookup"><span data-stu-id="0be0d-155">The size of the thumbnail requested.</span></span> <span data-ttu-id="0be0d-156">可取值为下面列出的标准大小之一或自定义大小。</span><span class="sxs-lookup"><span data-stu-id="0be0d-156">This can be one of the standard sizes listed below or a custom size.</span></span> |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="0be0d-157">检索缩略图的二进制内容</span><span class="sxs-lookup"><span data-stu-id="0be0d-157">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="0be0d-158">可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。</span><span class="sxs-lookup"><span data-stu-id="0be0d-158">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="0be0d-159">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0be0d-159">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="0be0d-160">响应</span><span class="sxs-lookup"><span data-stu-id="0be0d-160">Response</span></span>

<span data-ttu-id="0be0d-161">本服务用到缩略图 URL 的重定向进行响应。</span><span class="sxs-lookup"><span data-stu-id="0be0d-161">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="0be0d-162">缩略图 URL 具有缓存安全性。</span><span class="sxs-lookup"><span data-stu-id="0be0d-162">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="0be0d-163">如果在项发生更改后需要生成新的缩略图，URL 将会更改。</span><span class="sxs-lookup"><span data-stu-id="0be0d-163">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="0be0d-164">列出 DriveItem 时获取缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-164">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="0be0d-165">如果检索要显示的 DriveItem 资源的列表，可以使用_ $expand_ 查询字符串参数，以便同时包含这些资源的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0be0d-165">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="0be0d-166">这使你的应用可以通过一个请求同时检索缩略图和项，而不是发出多个请求。</span><span class="sxs-lookup"><span data-stu-id="0be0d-166">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="0be0d-167">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0be0d-167">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="0be0d-168">响应</span><span class="sxs-lookup"><span data-stu-id="0be0d-168">Response</span></span>

<span data-ttu-id="0be0d-169">本服务通过 DriveItem 及其缩略图的列表进行响应。</span><span class="sxs-lookup"><span data-stu-id="0be0d-169">The service responses with the list of DriveItems and their thumbnails.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-options"></a><span data-ttu-id="0be0d-170">大小选项</span><span class="sxs-lookup"><span data-stu-id="0be0d-170">Size options</span></span>

<span data-ttu-id="0be0d-p110">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="0be0d-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="0be0d-173">名称</span><span class="sxs-lookup"><span data-stu-id="0be0d-173">Name</span></span>           | <span data-ttu-id="0be0d-174">解决方案</span><span class="sxs-lookup"><span data-stu-id="0be0d-174">Resolution</span></span>  | <span data-ttu-id="0be0d-175">纵横比</span><span class="sxs-lookup"><span data-stu-id="0be0d-175">Aspect Ratio</span></span> | <span data-ttu-id="0be0d-176">说明</span><span class="sxs-lookup"><span data-stu-id="0be0d-176">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="0be0d-177">96 longest</span><span class="sxs-lookup"><span data-stu-id="0be0d-177">96 longest</span></span>  | <span data-ttu-id="0be0d-178">原始大小</span><span class="sxs-lookup"><span data-stu-id="0be0d-178">Original</span></span>     | <span data-ttu-id="0be0d-179">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="0be0d-179">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="0be0d-180">176 longest</span><span class="sxs-lookup"><span data-stu-id="0be0d-180">176 longest</span></span> | <span data-ttu-id="0be0d-181">原始大小</span><span class="sxs-lookup"><span data-stu-id="0be0d-181">Original</span></span>     | <span data-ttu-id="0be0d-182">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="0be0d-182">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="0be0d-183">800 longest</span><span class="sxs-lookup"><span data-stu-id="0be0d-183">800 longest</span></span> | <span data-ttu-id="0be0d-184">Original</span><span class="sxs-lookup"><span data-stu-id="0be0d-184">Original</span></span>     | <span data-ttu-id="0be0d-185">最长边重设为 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0be0d-185">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="0be0d-186">96x96</span><span class="sxs-lookup"><span data-stu-id="0be0d-186">96x96</span></span>       | <span data-ttu-id="0be0d-187">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="0be0d-187">Square Crop</span></span>  | <span data-ttu-id="0be0d-188">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-188">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="0be0d-189">176x176</span><span class="sxs-lookup"><span data-stu-id="0be0d-189">176x176</span></span>     | <span data-ttu-id="0be0d-190">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="0be0d-190">Square Crop</span></span>  | <span data-ttu-id="0be0d-191">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-191">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="0be0d-192">800x800</span><span class="sxs-lookup"><span data-stu-id="0be0d-192">800x800</span></span>     | <span data-ttu-id="0be0d-193">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="0be0d-193">Square Crop</span></span>  | <span data-ttu-id="0be0d-194">大方形缩略图</span><span class="sxs-lookup"><span data-stu-id="0be0d-194">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="0be0d-195">请求自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="0be0d-195">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="0be0d-196">除了定义大小外，应用还可以指定前缀为 `c` 的缩略图大小，从而请求获取自定义缩略图大小。</span><span class="sxs-lookup"><span data-stu-id="0be0d-196">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="0be0d-197">例如，如果你的应用需要 300x400 的缩略图，可以按如下所示请求获取此大小：</span><span class="sxs-lookup"><span data-stu-id="0be0d-197">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="0be0d-198">响应只包含选定的自定义缩略图大小：</span><span class="sxs-lookup"><span data-stu-id="0be0d-198">Which responds with just the custom thumbnail size selected:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

<span data-ttu-id="0be0d-199">可以在请求获取的缩略图尺寸后指定以下选项：</span><span class="sxs-lookup"><span data-stu-id="0be0d-199">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="0be0d-200">自定义标识符示例</span><span class="sxs-lookup"><span data-stu-id="0be0d-200">Examples of custom identifiers</span></span>

| <span data-ttu-id="0be0d-201">缩略图标识符</span><span class="sxs-lookup"><span data-stu-id="0be0d-201">Thumbnail identifier</span></span> | <span data-ttu-id="0be0d-202">分辨率</span><span class="sxs-lookup"><span data-stu-id="0be0d-202">Resolution</span></span>             | <span data-ttu-id="0be0d-203">纵横比</span><span class="sxs-lookup"><span data-stu-id="0be0d-203">Aspect ratio</span></span> | <span data-ttu-id="0be0d-204">说明</span><span class="sxs-lookup"><span data-stu-id="0be0d-204">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0be0d-205">c300x400</span><span class="sxs-lookup"><span data-stu-id="0be0d-205">c300x400</span></span>             | <span data-ttu-id="0be0d-206">300x400 像素框</span><span class="sxs-lookup"><span data-stu-id="0be0d-206">Bounded by 300x400 box</span></span> | <span data-ttu-id="0be0d-207">原始大小</span><span class="sxs-lookup"><span data-stu-id="0be0d-207">Original</span></span>     | <span data-ttu-id="0be0d-208">生成适应在 300x400 像素框中显示的缩略图，纵横比不变</span><span class="sxs-lookup"><span data-stu-id="0be0d-208">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="0be0d-209">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="0be0d-209">c300x400_Crop</span></span>        | <span data-ttu-id="0be0d-210">300x400</span><span class="sxs-lookup"><span data-stu-id="0be0d-210">300x400</span></span>                | <span data-ttu-id="0be0d-211">已裁剪</span><span class="sxs-lookup"><span data-stu-id="0be0d-211">Cropped</span></span>      | <span data-ttu-id="0be0d-p112">生成 300x400 像素缩略图。 具体方式为，重设图像大小以填充 300x400 框，并裁剪超出框外的内容。</span><span class="sxs-lookup"><span data-stu-id="0be0d-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="0be0d-214">**注意：** 返回的缩略图可能与请求的像素尺寸不完全匹配，但与纵横比匹配。</span><span class="sxs-lookup"><span data-stu-id="0be0d-214">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="0be0d-215">在某些情况下，如果缩略图已经存在并且可以轻松缩放来匹配请求的分辨率，则可能会返回比请求的大小更大的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0be0d-215">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="0be0d-216">注解</span><span class="sxs-lookup"><span data-stu-id="0be0d-216">Remarks</span></span>

<span data-ttu-id="0be0d-217">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="0be0d-217">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="0be0d-218">使用这些调用展开缩略图集合不适用于：</span><span class="sxs-lookup"><span data-stu-id="0be0d-218">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="0be0d-219">SharePoint Server 2016 不支持缩略图。</span><span class="sxs-lookup"><span data-stu-id="0be0d-219">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="0be0d-220">错误响应</span><span class="sxs-lookup"><span data-stu-id="0be0d-220">Error responses</span></span>

<span data-ttu-id="0be0d-221">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="0be0d-221">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem-list-thumbnails.md:
      Unable to map some markdown elements into schema.
         Unmapped methods:
      enum-item-thumbnails, get-one-thumbnail, get-thumbnail-content, get-thumbnail-while-listing, get-thumbnail-custom-size
         Unmapped tables:
      Permissions - AuthScopes, Path parameters - PathParameters, Size options - Unknown, Examples of custom identifiers - Unknown",
    "Warning: Couldn't serialize request for path /me/drive/items/{var}/thumbnails/{var}/{var}/content into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property '{var}' on 'thumbnailSet'. Possible issues:
         1) Doc bug where '{var}' isn't defined on the resource.         2) Doc bug where '{var}' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'thumbnailSet' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 1145
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 821"
  ],
  "tocPath": "Items/Thumbnails"
} -->
