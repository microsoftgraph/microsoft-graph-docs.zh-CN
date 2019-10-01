---
author: JeremyKelley
description: 检索 DriveItem 资源的 ThumbnailSet 资源集合。
ms.date: 09/10/2017
title: 检索文件或文件夹的缩略图
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2bed97e65a57c4a7d46336e9dcd845780e9e8d30
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333225"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="68782-103">列出 DriveItem 的缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-103">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68782-104">检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="68782-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="68782-p101">DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。</span><span class="sxs-lookup"><span data-stu-id="68782-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="68782-p102">可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：</span><span class="sxs-lookup"><span data-stu-id="68782-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="68782-110">枚举项目的可用缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="68782-111">检索项目的单个缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="68782-112">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="68782-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="68782-113">在单个请求中检索多个项目的缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="68782-114">检索自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="68782-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="68782-115">上载项目的自定义缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="68782-116">确定是否存在自定义的上传缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-116">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="68782-117">权限</span><span class="sxs-lookup"><span data-stu-id="68782-117">Permissions</span></span>

<span data-ttu-id="68782-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68782-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68782-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="68782-120">Permission type</span></span>      | <span data-ttu-id="68782-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68782-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68782-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68782-122">Delegated (work or school account)</span></span> | <span data-ttu-id="68782-123">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68782-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="68782-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68782-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68782-125">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68782-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="68782-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="68782-126">Application</span></span> | <span data-ttu-id="68782-127">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68782-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68782-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68782-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68782-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="68782-129">Optional query parameters</span></span>

<span data-ttu-id="68782-130">此方法支持使用 `$select`[OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="68782-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="68782-131">此外，此方法支持检索具有原始方向 EXIF 值的缩略图，并且不通过追加`originalOrientation=true`查询参数来使用应用旋转。</span><span class="sxs-lookup"><span data-stu-id="68782-131">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="68782-132">此项当前仅在 OneDrive 个人版上受支持。</span><span class="sxs-lookup"><span data-stu-id="68782-132">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="68782-133">响应</span><span class="sxs-lookup"><span data-stu-id="68782-133">Response</span></span>

<span data-ttu-id="68782-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="68782-134">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68782-135">示例</span><span class="sxs-lookup"><span data-stu-id="68782-135">Example</span></span>

<span data-ttu-id="68782-136">下面是检索当前用户的 OneDrive 中某个项的可用缩略图的请求示例。</span><span class="sxs-lookup"><span data-stu-id="68782-136">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68782-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="68782-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68782-138">C#</span><span class="sxs-lookup"><span data-stu-id="68782-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68782-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68782-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68782-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68782-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="68782-141">这将返回项的可用 **thumbnailSet** 的数组。</span><span class="sxs-lookup"><span data-stu-id="68782-141">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="68782-142">驱动器中的任何项都可以有零个或多个缩略图。</span><span class="sxs-lookup"><span data-stu-id="68782-142">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="68782-p106">**注意：** 可以使用 _select_ 查询字符串参数，控制在 **ThumbnailSet** 中返回的缩略图尺寸。 例如，`/thumbnails?select=medium` 仅检索中等大小的缩略图。</span><span class="sxs-lookup"><span data-stu-id="68782-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="68782-145">响应</span><span class="sxs-lookup"><span data-stu-id="68782-145">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="68782-146">获取单个缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-146">Get a single thumbnail</span></span>

<span data-ttu-id="68782-147">通过直接在请求中对其进行寻址来检索单个缩略图和大小的元数据。</span><span class="sxs-lookup"><span data-stu-id="68782-147">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="68782-148">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68782-148">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68782-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="68782-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68782-150">C#</span><span class="sxs-lookup"><span data-stu-id="68782-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68782-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68782-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68782-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68782-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="68782-153">Path 参数</span><span class="sxs-lookup"><span data-stu-id="68782-153">Path parameters</span></span>

| <span data-ttu-id="68782-154">名称</span><span class="sxs-lookup"><span data-stu-id="68782-154">Name</span></span>         | <span data-ttu-id="68782-155">类型</span><span class="sxs-lookup"><span data-stu-id="68782-155">Type</span></span>   | <span data-ttu-id="68782-156">说明</span><span class="sxs-lookup"><span data-stu-id="68782-156">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="68782-157">**item-id**</span><span class="sxs-lookup"><span data-stu-id="68782-157">**item-id**</span></span>  | <span data-ttu-id="68782-158">string</span><span class="sxs-lookup"><span data-stu-id="68782-158">string</span></span> | <span data-ttu-id="68782-159">引用的项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="68782-159">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="68782-160">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="68782-160">**thumb-id**</span></span> | <span data-ttu-id="68782-161">数字</span><span class="sxs-lookup"><span data-stu-id="68782-161">number</span></span> | <span data-ttu-id="68782-p107">缩略图的索引，通常介于 0 到 4 之间。 如果没有自定义缩略图，索引为 0。</span><span class="sxs-lookup"><span data-stu-id="68782-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="68782-164">**size**</span><span class="sxs-lookup"><span data-stu-id="68782-164">**size**</span></span>     | <span data-ttu-id="68782-165">string</span><span class="sxs-lookup"><span data-stu-id="68782-165">string</span></span> | <span data-ttu-id="68782-166">请求获取的缩略图的大小。</span><span class="sxs-lookup"><span data-stu-id="68782-166">The size of the thumbnail requested.</span></span> <span data-ttu-id="68782-167">可取值为下面列出的标准大小之一或自定义大小。</span><span class="sxs-lookup"><span data-stu-id="68782-167">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="68782-168">检索缩略图的二进制内容</span><span class="sxs-lookup"><span data-stu-id="68782-168">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="68782-169">可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。</span><span class="sxs-lookup"><span data-stu-id="68782-169">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="68782-170">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68782-170">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68782-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="68782-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68782-172">C#</span><span class="sxs-lookup"><span data-stu-id="68782-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68782-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68782-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68782-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68782-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68782-175">响应</span><span class="sxs-lookup"><span data-stu-id="68782-175">Response</span></span>

<span data-ttu-id="68782-176">本服务用到缩略图 URL 的重定向进行响应。</span><span class="sxs-lookup"><span data-stu-id="68782-176">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="68782-177">缩略图 URL 具有缓存安全性。</span><span class="sxs-lookup"><span data-stu-id="68782-177">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="68782-178">如果在项发生更改后需要生成新的缩略图，URL 将会更改。</span><span class="sxs-lookup"><span data-stu-id="68782-178">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="68782-179">列出 DriveItem 时获取缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-179">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="68782-180">如果检索要显示的 DriveItem 资源的列表，可以使用_ $expand_ 查询字符串参数，以便同时包含这些资源的缩略图。</span><span class="sxs-lookup"><span data-stu-id="68782-180">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="68782-181">这使你的应用可以通过一个请求同时检索缩略图和项，而不是发出多个请求。</span><span class="sxs-lookup"><span data-stu-id="68782-181">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="68782-182">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68782-182">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68782-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="68782-183">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68782-184">C#</span><span class="sxs-lookup"><span data-stu-id="68782-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68782-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68782-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68782-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68782-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68782-187">响应</span><span class="sxs-lookup"><span data-stu-id="68782-187">Response</span></span>

<span data-ttu-id="68782-188">本服务通过 DriveItem 及其缩略图的列表进行响应。</span><span class="sxs-lookup"><span data-stu-id="68782-188">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="68782-189">Size 的值</span><span class="sxs-lookup"><span data-stu-id="68782-189">Size values</span></span>

<span data-ttu-id="68782-p111">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="68782-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="68782-192">名称</span><span class="sxs-lookup"><span data-stu-id="68782-192">Name</span></span>           | <span data-ttu-id="68782-193">分辨率</span><span class="sxs-lookup"><span data-stu-id="68782-193">Resolution</span></span>  | <span data-ttu-id="68782-194">纵横比</span><span class="sxs-lookup"><span data-stu-id="68782-194">Aspect Ratio</span></span> | <span data-ttu-id="68782-195">说明</span><span class="sxs-lookup"><span data-stu-id="68782-195">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="68782-196">96 longest</span><span class="sxs-lookup"><span data-stu-id="68782-196">96 longest</span></span>  | <span data-ttu-id="68782-197">原始大小</span><span class="sxs-lookup"><span data-stu-id="68782-197">Original</span></span>     | <span data-ttu-id="68782-198">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="68782-198">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="68782-199">176 longest</span><span class="sxs-lookup"><span data-stu-id="68782-199">176 longest</span></span> | <span data-ttu-id="68782-200">原始大小</span><span class="sxs-lookup"><span data-stu-id="68782-200">Original</span></span>     | <span data-ttu-id="68782-201">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="68782-201">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="68782-202">800 longest</span><span class="sxs-lookup"><span data-stu-id="68782-202">800 longest</span></span> | <span data-ttu-id="68782-203">Original</span><span class="sxs-lookup"><span data-stu-id="68782-203">Original</span></span>     | <span data-ttu-id="68782-204">最长边重设为 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="68782-204">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="68782-205">96x96</span><span class="sxs-lookup"><span data-stu-id="68782-205">96x96</span></span>       | <span data-ttu-id="68782-206">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="68782-206">Square Crop</span></span>  | <span data-ttu-id="68782-207">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-207">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="68782-208">176x176</span><span class="sxs-lookup"><span data-stu-id="68782-208">176x176</span></span>     | <span data-ttu-id="68782-209">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="68782-209">Square Crop</span></span>  | <span data-ttu-id="68782-210">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-210">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="68782-211">800x800</span><span class="sxs-lookup"><span data-stu-id="68782-211">800x800</span></span>     | <span data-ttu-id="68782-212">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="68782-212">Square Crop</span></span>  | <span data-ttu-id="68782-213">大方形缩略图</span><span class="sxs-lookup"><span data-stu-id="68782-213">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="68782-214">请求自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="68782-214">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="68782-215">除了定义大小外，应用还可以指定前缀为 `c` 的缩略图大小，从而请求获取自定义缩略图大小。</span><span class="sxs-lookup"><span data-stu-id="68782-215">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="68782-216">例如，如果你的应用需要 300x400 的缩略图，可以按如下所示请求获取此大小：</span><span class="sxs-lookup"><span data-stu-id="68782-216">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68782-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="68782-217">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68782-218">C#</span><span class="sxs-lookup"><span data-stu-id="68782-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68782-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68782-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68782-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68782-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="68782-221">响应只包含选定的自定义缩略图尺寸：</span><span class="sxs-lookup"><span data-stu-id="68782-221">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="68782-222">可以在请求获取的缩略图尺寸后指定以下选项：</span><span class="sxs-lookup"><span data-stu-id="68782-222">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="68782-223">自定义标识符示例</span><span class="sxs-lookup"><span data-stu-id="68782-223">Examples of custom identifiers</span></span>

| <span data-ttu-id="68782-224">缩略图标识符</span><span class="sxs-lookup"><span data-stu-id="68782-224">Thumbnail identifier</span></span> | <span data-ttu-id="68782-225">分辨率</span><span class="sxs-lookup"><span data-stu-id="68782-225">Resolution</span></span>             | <span data-ttu-id="68782-226">纵横比</span><span class="sxs-lookup"><span data-stu-id="68782-226">Aspect ratio</span></span> | <span data-ttu-id="68782-227">说明</span><span class="sxs-lookup"><span data-stu-id="68782-227">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68782-228">c300x400</span><span class="sxs-lookup"><span data-stu-id="68782-228">c300x400</span></span>             | <span data-ttu-id="68782-229">300x400 像素框</span><span class="sxs-lookup"><span data-stu-id="68782-229">Bounded by 300x400 box</span></span> | <span data-ttu-id="68782-230">原始大小</span><span class="sxs-lookup"><span data-stu-id="68782-230">Original</span></span>     | <span data-ttu-id="68782-231">生成适应在 300x400 像素框中显示的缩略图，纵横比不变</span><span class="sxs-lookup"><span data-stu-id="68782-231">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="68782-232">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="68782-232">c300x400_Crop</span></span>        | <span data-ttu-id="68782-233">300x400</span><span class="sxs-lookup"><span data-stu-id="68782-233">300x400</span></span>                | <span data-ttu-id="68782-234">已裁剪</span><span class="sxs-lookup"><span data-stu-id="68782-234">Cropped</span></span>      | <span data-ttu-id="68782-p113">生成 300x400 像素缩略图。 具体方式为，重设图像大小以填充 300x400 框，并裁剪超出框外的内容。</span><span class="sxs-lookup"><span data-stu-id="68782-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="68782-237">**注意：** 返回的缩略图可能与请求的像素尺寸不完全匹配，但与纵横比匹配。</span><span class="sxs-lookup"><span data-stu-id="68782-237">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="68782-238">在某些情况下，如果缩略图已经存在并且可以轻松缩放来匹配请求的分辨率，则可能会返回比请求的大小更大的缩略图。</span><span class="sxs-lookup"><span data-stu-id="68782-238">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="68782-239">注解</span><span class="sxs-lookup"><span data-stu-id="68782-239">Remarks</span></span>

<span data-ttu-id="68782-240">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="68782-240">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="68782-241">使用这些调用展开缩略图集合不适用于：</span><span class="sxs-lookup"><span data-stu-id="68782-241">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="68782-242">SharePoint Server 2016 不支持缩略图。</span><span class="sxs-lookup"><span data-stu-id="68782-242">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="68782-243">错误响应</span><span class="sxs-lookup"><span data-stu-id="68782-243">Error responses</span></span>

<span data-ttu-id="68782-244">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="68782-244">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
