---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 检索文件或文件夹的缩略图
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 53ff273f489c283ff3a196096904c42fd39d2883
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436359"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="62349-102">列出 DriveItem 的缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-102">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62349-103">检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="62349-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="62349-p101">DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。</span><span class="sxs-lookup"><span data-stu-id="62349-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="62349-p102">可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：</span><span class="sxs-lookup"><span data-stu-id="62349-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="62349-109">枚举项目的可用缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="62349-110">检索项目的单个缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="62349-111">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="62349-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="62349-112">在单个请求中检索多个项目的缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="62349-113">检索自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="62349-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="62349-114">上载项目的自定义缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="62349-115">确定是否存在自定义的上传缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-115">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="62349-116">权限</span><span class="sxs-lookup"><span data-stu-id="62349-116">Permissions</span></span>

<span data-ttu-id="62349-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62349-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62349-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="62349-119">Permission type</span></span>      | <span data-ttu-id="62349-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62349-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62349-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62349-121">Delegated (work or school account)</span></span> | <span data-ttu-id="62349-122">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62349-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="62349-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62349-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62349-124">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62349-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="62349-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="62349-125">Application</span></span> | <span data-ttu-id="62349-126">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62349-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62349-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62349-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62349-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="62349-128">Optional query parameters</span></span>

<span data-ttu-id="62349-129">此方法支持使用 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="62349-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="62349-130">响应</span><span class="sxs-lookup"><span data-stu-id="62349-130">Response</span></span>

<span data-ttu-id="62349-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="62349-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62349-132">示例</span><span class="sxs-lookup"><span data-stu-id="62349-132">Example</span></span>

<span data-ttu-id="62349-133">下面是检索当前用户的 OneDrive 中某个项的可用缩略图的请求示例。</span><span class="sxs-lookup"><span data-stu-id="62349-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62349-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="62349-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62349-135">C#</span><span class="sxs-lookup"><span data-stu-id="62349-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62349-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="62349-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62349-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="62349-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="62349-138">这将返回项的可用 **thumbnailSet** 的数组。</span><span class="sxs-lookup"><span data-stu-id="62349-138">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="62349-139">驱动器中的任何项都可以有零个或多个缩略图。</span><span class="sxs-lookup"><span data-stu-id="62349-139">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="62349-p105">**注意：** 可以使用 _select_ 查询字符串参数，控制在 **ThumbnailSet** 中返回的缩略图尺寸。 例如，`/thumbnails?select=medium` 仅检索中等大小的缩略图。</span><span class="sxs-lookup"><span data-stu-id="62349-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="62349-142">响应</span><span class="sxs-lookup"><span data-stu-id="62349-142">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="62349-143">获取单个缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-143">Get a single thumbnail</span></span>

<span data-ttu-id="62349-144">通过直接在请求中对其进行寻址来检索单个缩略图和大小的元数据。</span><span class="sxs-lookup"><span data-stu-id="62349-144">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="62349-145">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62349-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62349-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="62349-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62349-147">C#</span><span class="sxs-lookup"><span data-stu-id="62349-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62349-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="62349-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62349-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="62349-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="62349-150">Path 参数</span><span class="sxs-lookup"><span data-stu-id="62349-150">Path parameters</span></span>

| <span data-ttu-id="62349-151">名称</span><span class="sxs-lookup"><span data-stu-id="62349-151">Name</span></span>         | <span data-ttu-id="62349-152">类型</span><span class="sxs-lookup"><span data-stu-id="62349-152">Type</span></span>   | <span data-ttu-id="62349-153">说明</span><span class="sxs-lookup"><span data-stu-id="62349-153">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="62349-154">**item-id**</span><span class="sxs-lookup"><span data-stu-id="62349-154">**item-id**</span></span>  | <span data-ttu-id="62349-155">string</span><span class="sxs-lookup"><span data-stu-id="62349-155">string</span></span> | <span data-ttu-id="62349-156">引用的项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="62349-156">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="62349-157">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="62349-157">**thumb-id**</span></span> | <span data-ttu-id="62349-158">数字</span><span class="sxs-lookup"><span data-stu-id="62349-158">number</span></span> | <span data-ttu-id="62349-p106">缩略图的索引，通常介于 0 到 4 之间。 如果没有自定义缩略图，索引为 0。</span><span class="sxs-lookup"><span data-stu-id="62349-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="62349-161">**size**</span><span class="sxs-lookup"><span data-stu-id="62349-161">**size**</span></span>     | <span data-ttu-id="62349-162">string</span><span class="sxs-lookup"><span data-stu-id="62349-162">string</span></span> | <span data-ttu-id="62349-163">请求获取的缩略图的大小。</span><span class="sxs-lookup"><span data-stu-id="62349-163">The size of the thumbnail requested.</span></span> <span data-ttu-id="62349-164">可取值为下面列出的标准大小之一或自定义大小。</span><span class="sxs-lookup"><span data-stu-id="62349-164">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="62349-165">检索缩略图的二进制内容</span><span class="sxs-lookup"><span data-stu-id="62349-165">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="62349-166">可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。</span><span class="sxs-lookup"><span data-stu-id="62349-166">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="62349-167">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62349-167">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62349-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="62349-168">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62349-169">C#</span><span class="sxs-lookup"><span data-stu-id="62349-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62349-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="62349-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62349-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="62349-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62349-172">响应</span><span class="sxs-lookup"><span data-stu-id="62349-172">Response</span></span>

<span data-ttu-id="62349-173">本服务用到缩略图 URL 的重定向进行响应。</span><span class="sxs-lookup"><span data-stu-id="62349-173">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="62349-174">缩略图 URL 具有缓存安全性。</span><span class="sxs-lookup"><span data-stu-id="62349-174">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="62349-175">如果在项发生更改后需要生成新的缩略图，URL 将会更改。</span><span class="sxs-lookup"><span data-stu-id="62349-175">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="62349-176">列出 DriveItem 时获取缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-176">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="62349-177">如果检索要显示的 DriveItem 资源的列表，可以使用_ $expand_ 查询字符串参数，以便同时包含这些资源的缩略图。</span><span class="sxs-lookup"><span data-stu-id="62349-177">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="62349-178">这使你的应用可以通过一个请求同时检索缩略图和项，而不是发出多个请求。</span><span class="sxs-lookup"><span data-stu-id="62349-178">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="62349-179">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62349-179">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62349-180">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="62349-180">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62349-181">C#</span><span class="sxs-lookup"><span data-stu-id="62349-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62349-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="62349-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62349-183">目标-C</span><span class="sxs-lookup"><span data-stu-id="62349-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62349-184">响应</span><span class="sxs-lookup"><span data-stu-id="62349-184">Response</span></span>

<span data-ttu-id="62349-185">本服务通过 DriveItem 及其缩略图的列表进行响应。</span><span class="sxs-lookup"><span data-stu-id="62349-185">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="62349-186">Size 的值</span><span class="sxs-lookup"><span data-stu-id="62349-186">Size values</span></span>

<span data-ttu-id="62349-p110">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="62349-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="62349-189">名称</span><span class="sxs-lookup"><span data-stu-id="62349-189">Name</span></span>           | <span data-ttu-id="62349-190">分辨率</span><span class="sxs-lookup"><span data-stu-id="62349-190">Resolution</span></span>  | <span data-ttu-id="62349-191">纵横比</span><span class="sxs-lookup"><span data-stu-id="62349-191">Aspect Ratio</span></span> | <span data-ttu-id="62349-192">说明</span><span class="sxs-lookup"><span data-stu-id="62349-192">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="62349-193">96 longest</span><span class="sxs-lookup"><span data-stu-id="62349-193">96 longest</span></span>  | <span data-ttu-id="62349-194">原始大小</span><span class="sxs-lookup"><span data-stu-id="62349-194">Original</span></span>     | <span data-ttu-id="62349-195">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="62349-195">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="62349-196">176 longest</span><span class="sxs-lookup"><span data-stu-id="62349-196">176 longest</span></span> | <span data-ttu-id="62349-197">原始大小</span><span class="sxs-lookup"><span data-stu-id="62349-197">Original</span></span>     | <span data-ttu-id="62349-198">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="62349-198">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="62349-199">800 longest</span><span class="sxs-lookup"><span data-stu-id="62349-199">800 longest</span></span> | <span data-ttu-id="62349-200">Original</span><span class="sxs-lookup"><span data-stu-id="62349-200">Original</span></span>     | <span data-ttu-id="62349-201">最长边重设为 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="62349-201">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="62349-202">96x96</span><span class="sxs-lookup"><span data-stu-id="62349-202">96x96</span></span>       | <span data-ttu-id="62349-203">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="62349-203">Square Crop</span></span>  | <span data-ttu-id="62349-204">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-204">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="62349-205">176x176</span><span class="sxs-lookup"><span data-stu-id="62349-205">176x176</span></span>     | <span data-ttu-id="62349-206">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="62349-206">Square Crop</span></span>  | <span data-ttu-id="62349-207">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-207">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="62349-208">800x800</span><span class="sxs-lookup"><span data-stu-id="62349-208">800x800</span></span>     | <span data-ttu-id="62349-209">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="62349-209">Square Crop</span></span>  | <span data-ttu-id="62349-210">大方形缩略图</span><span class="sxs-lookup"><span data-stu-id="62349-210">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="62349-211">请求自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="62349-211">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="62349-212">除了定义大小外，应用还可以指定前缀为 `c` 的缩略图大小，从而请求获取自定义缩略图大小。</span><span class="sxs-lookup"><span data-stu-id="62349-212">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="62349-213">例如，如果你的应用需要 300x400 的缩略图，可以按如下所示请求获取此大小：</span><span class="sxs-lookup"><span data-stu-id="62349-213">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62349-214">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="62349-214">HTTP</span></span>](#tab/http)
<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62349-215">C#</span><span class="sxs-lookup"><span data-stu-id="62349-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62349-216">Javascript</span><span class="sxs-lookup"><span data-stu-id="62349-216">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62349-217">目标-C</span><span class="sxs-lookup"><span data-stu-id="62349-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="62349-218">响应只包含选定的自定义缩略图尺寸：</span><span class="sxs-lookup"><span data-stu-id="62349-218">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="62349-219">可以在请求获取的缩略图尺寸后指定以下选项：</span><span class="sxs-lookup"><span data-stu-id="62349-219">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="62349-220">自定义标识符示例</span><span class="sxs-lookup"><span data-stu-id="62349-220">Examples of custom identifiers</span></span>

| <span data-ttu-id="62349-221">缩略图标识符</span><span class="sxs-lookup"><span data-stu-id="62349-221">Thumbnail identifier</span></span> | <span data-ttu-id="62349-222">分辨率</span><span class="sxs-lookup"><span data-stu-id="62349-222">Resolution</span></span>             | <span data-ttu-id="62349-223">纵横比</span><span class="sxs-lookup"><span data-stu-id="62349-223">Aspect ratio</span></span> | <span data-ttu-id="62349-224">说明</span><span class="sxs-lookup"><span data-stu-id="62349-224">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="62349-225">c300x400</span><span class="sxs-lookup"><span data-stu-id="62349-225">c300x400</span></span>             | <span data-ttu-id="62349-226">300x400 像素框</span><span class="sxs-lookup"><span data-stu-id="62349-226">Bounded by 300x400 box</span></span> | <span data-ttu-id="62349-227">原始大小</span><span class="sxs-lookup"><span data-stu-id="62349-227">Original</span></span>     | <span data-ttu-id="62349-228">生成适应在 300x400 像素框中显示的缩略图，纵横比不变</span><span class="sxs-lookup"><span data-stu-id="62349-228">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="62349-229">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="62349-229">c300x400_Crop</span></span>        | <span data-ttu-id="62349-230">300x400</span><span class="sxs-lookup"><span data-stu-id="62349-230">300x400</span></span>                | <span data-ttu-id="62349-231">已裁剪</span><span class="sxs-lookup"><span data-stu-id="62349-231">Cropped</span></span>      | <span data-ttu-id="62349-p112">生成 300x400 像素缩略图。 具体方式为，重设图像大小以填充 300x400 框，并裁剪超出框外的内容。</span><span class="sxs-lookup"><span data-stu-id="62349-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="62349-234">**注意：** 返回的缩略图可能与请求的像素尺寸不完全匹配，但与纵横比匹配。</span><span class="sxs-lookup"><span data-stu-id="62349-234">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="62349-235">在某些情况下，如果缩略图已经存在并且可以轻松缩放来匹配请求的分辨率，则可能会返回比请求的大小更大的缩略图。</span><span class="sxs-lookup"><span data-stu-id="62349-235">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="62349-236">注解</span><span class="sxs-lookup"><span data-stu-id="62349-236">Remarks</span></span>

<span data-ttu-id="62349-237">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="62349-237">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="62349-238">使用这些调用展开缩略图集合不适用于：</span><span class="sxs-lookup"><span data-stu-id="62349-238">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="62349-239">SharePoint Server 2016 不支持缩略图。</span><span class="sxs-lookup"><span data-stu-id="62349-239">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="62349-240">错误响应</span><span class="sxs-lookup"><span data-stu-id="62349-240">Error responses</span></span>

<span data-ttu-id="62349-241">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="62349-241">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
  ]
}
-->
