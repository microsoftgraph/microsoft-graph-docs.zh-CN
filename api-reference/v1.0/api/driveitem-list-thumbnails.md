---
author: JeremyKelley
ms.date: 09/10/2017
title: 检索文件或文件夹的缩略图
localization_priority: Normal
ms.prod: sharepoint
description: 检索 DriveItem 资源的 ThumbnailSet 资源集合。
doc_type: apiPageType
ms.openlocfilehash: 63ee68ade1a314a34cbb5ee778e5eccaec413a62
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059367"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="2c1ac-103">列出 DriveItem 的缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="2c1ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c1ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c1ac-105">检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="2c1ac-p101">DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="2c1ac-p102">可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="2c1ac-111">枚举项目的可用缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="2c1ac-112">检索项目的单个缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="2c1ac-113">检索缩略图的内容</span><span class="sxs-lookup"><span data-stu-id="2c1ac-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="2c1ac-114">在单个请求中检索多个项目的缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="2c1ac-115">检索自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="2c1ac-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="2c1ac-116">上载项目的自定义缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="2c1ac-117">确定是否存在自定义的上传缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-117">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="2c1ac-118">权限</span><span class="sxs-lookup"><span data-stu-id="2c1ac-118">Permissions</span></span>

<span data-ttu-id="2c1ac-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c1ac-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c1ac-121">Permission type</span></span>      | <span data-ttu-id="2c1ac-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c1ac-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c1ac-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c1ac-123">Delegated (work or school account)</span></span> | <span data-ttu-id="2c1ac-124">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c1ac-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c1ac-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c1ac-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c1ac-126">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c1ac-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c1ac-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c1ac-127">Application</span></span> | <span data-ttu-id="2c1ac-128">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c1ac-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c1ac-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c1ac-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c1ac-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c1ac-130">Optional query parameters</span></span>

<span data-ttu-id="2c1ac-131">此方法支持使用 `$select`[OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="2c1ac-132">此外，此方法还支持通过追加查询参数来检索包含原始方向 EXIF 值且没有应用旋转的 `originalOrientation=true` 缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-132">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="2c1ac-133">目前仅 OneDrive 个人版支持此操作。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-133">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="2c1ac-134">响应</span><span class="sxs-lookup"><span data-stu-id="2c1ac-134">Response</span></span>

<span data-ttu-id="2c1ac-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-135">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c1ac-136">示例</span><span class="sxs-lookup"><span data-stu-id="2c1ac-136">Example</span></span>

<span data-ttu-id="2c1ac-137">下面是检索当前用户的 OneDrive 中某个项的可用缩略图的请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-137">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c1ac-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1ac-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[<span data-ttu-id="2c1ac-139">C#</span><span class="sxs-lookup"><span data-stu-id="2c1ac-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c1ac-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c1ac-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c1ac-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c1ac-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c1ac-142">Java</span><span class="sxs-lookup"><span data-stu-id="2c1ac-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2c1ac-143">这将返回项的可用 **thumbnailSet** 的数组。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-143">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="2c1ac-144">驱动器中的任何项都可以有零个或多个缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-144">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="2c1ac-p106">**注意：** 可以使用 _select_ 查询字符串参数，控制在 **ThumbnailSet** 中返回的缩略图尺寸。 例如，`/thumbnails?select=medium` 仅检索中等大小的缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="2c1ac-147">响应</span><span class="sxs-lookup"><span data-stu-id="2c1ac-147">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="2c1ac-148">获取单个缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-148">Get a single thumbnail</span></span>

<span data-ttu-id="2c1ac-149">通过在请求中直接解决来检索单个缩略图和大小的元数据。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-149">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c1ac-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c1ac-150">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2c1ac-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1ac-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[<span data-ttu-id="2c1ac-152">C#</span><span class="sxs-lookup"><span data-stu-id="2c1ac-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c1ac-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c1ac-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c1ac-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c1ac-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c1ac-155">Java</span><span class="sxs-lookup"><span data-stu-id="2c1ac-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="2c1ac-156">路径参数</span><span class="sxs-lookup"><span data-stu-id="2c1ac-156">Path parameters</span></span>

| <span data-ttu-id="2c1ac-157">名称</span><span class="sxs-lookup"><span data-stu-id="2c1ac-157">Name</span></span>         | <span data-ttu-id="2c1ac-158">类型</span><span class="sxs-lookup"><span data-stu-id="2c1ac-158">Type</span></span>   | <span data-ttu-id="2c1ac-159">说明</span><span class="sxs-lookup"><span data-stu-id="2c1ac-159">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="2c1ac-160">**item-id**</span><span class="sxs-lookup"><span data-stu-id="2c1ac-160">**item-id**</span></span>  | <span data-ttu-id="2c1ac-161">string</span><span class="sxs-lookup"><span data-stu-id="2c1ac-161">string</span></span> | <span data-ttu-id="2c1ac-162">引用的项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-162">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="2c1ac-163">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="2c1ac-163">**thumb-id**</span></span> | <span data-ttu-id="2c1ac-164">number</span><span class="sxs-lookup"><span data-stu-id="2c1ac-164">number</span></span> | <span data-ttu-id="2c1ac-p107">缩略图的索引，通常介于 0 到 4 之间。 如果没有自定义缩略图，索引为 0。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="2c1ac-167">**size**</span><span class="sxs-lookup"><span data-stu-id="2c1ac-167">**size**</span></span>     | <span data-ttu-id="2c1ac-168">string</span><span class="sxs-lookup"><span data-stu-id="2c1ac-168">string</span></span> | <span data-ttu-id="2c1ac-169">请求获取的缩略图的尺寸。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-169">The size of the thumbnail requested.</span></span> <span data-ttu-id="2c1ac-170">可取值为下面列出的标准大小之一或自定义大小。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-170">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="2c1ac-171">检索缩略图的二进制内容</span><span class="sxs-lookup"><span data-stu-id="2c1ac-171">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="2c1ac-172">可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-172">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c1ac-173">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c1ac-173">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2c1ac-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1ac-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[<span data-ttu-id="2c1ac-175">C#</span><span class="sxs-lookup"><span data-stu-id="2c1ac-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c1ac-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c1ac-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c1ac-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c1ac-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c1ac-178">Java</span><span class="sxs-lookup"><span data-stu-id="2c1ac-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c1ac-179">响应</span><span class="sxs-lookup"><span data-stu-id="2c1ac-179">Response</span></span>

<span data-ttu-id="2c1ac-180">本服务通过到缩略图 URL 的重定向进行响应。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-180">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="2c1ac-p109">缩略图 URL 具有缓存安全性。 如果在项发生更改后需要生成新的缩略图，URL 将会更改。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p109">Thumbnail URLs are cache-safe. The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="2c1ac-183">获取缩略图的同时列出 DriveItem</span><span class="sxs-lookup"><span data-stu-id="2c1ac-183">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="2c1ac-184">如果检索要显示的 DriveItem 资源的列表，可以使用 _$expand_ 查询字符串参数，以便同时包含这些资源的缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-184">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="2c1ac-185">这使你的应用可以通过一个请求同时检索缩略图和项，而不是发出多个请求。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-185">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c1ac-186">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c1ac-186">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2c1ac-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1ac-187">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[<span data-ttu-id="2c1ac-188">C#</span><span class="sxs-lookup"><span data-stu-id="2c1ac-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c1ac-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c1ac-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c1ac-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c1ac-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c1ac-191">Java</span><span class="sxs-lookup"><span data-stu-id="2c1ac-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c1ac-192">响应</span><span class="sxs-lookup"><span data-stu-id="2c1ac-192">Response</span></span>

<span data-ttu-id="2c1ac-193">本服务通过 DriveItem 及其缩略图的列表进行响应。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-193">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-options"></a><span data-ttu-id="2c1ac-194">大小选项</span><span class="sxs-lookup"><span data-stu-id="2c1ac-194">Size options</span></span>

<span data-ttu-id="2c1ac-p111">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="2c1ac-197">名称</span><span class="sxs-lookup"><span data-stu-id="2c1ac-197">Name</span></span>           | <span data-ttu-id="2c1ac-198">分辨率</span><span class="sxs-lookup"><span data-stu-id="2c1ac-198">Resolution</span></span>  | <span data-ttu-id="2c1ac-199">纵横比​​</span><span class="sxs-lookup"><span data-stu-id="2c1ac-199">Aspect Ratio</span></span> | <span data-ttu-id="2c1ac-200">说明</span><span class="sxs-lookup"><span data-stu-id="2c1ac-200">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="2c1ac-201">96 longest</span><span class="sxs-lookup"><span data-stu-id="2c1ac-201">96 longest</span></span>  | <span data-ttu-id="2c1ac-202">Original</span><span class="sxs-lookup"><span data-stu-id="2c1ac-202">Original</span></span>     | <span data-ttu-id="2c1ac-203">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-203">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="2c1ac-204">176 longest</span><span class="sxs-lookup"><span data-stu-id="2c1ac-204">176 longest</span></span> | <span data-ttu-id="2c1ac-205">Original</span><span class="sxs-lookup"><span data-stu-id="2c1ac-205">Original</span></span>     | <span data-ttu-id="2c1ac-206">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-206">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="2c1ac-207">800 longest
</span><span class="sxs-lookup"><span data-stu-id="2c1ac-207">800 longest</span></span> | <span data-ttu-id="2c1ac-208">Original</span><span class="sxs-lookup"><span data-stu-id="2c1ac-208">Original</span></span>     | <span data-ttu-id="2c1ac-209">最长边重设为 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-209">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="2c1ac-210">96x96</span><span class="sxs-lookup"><span data-stu-id="2c1ac-210">96x96</span></span>       | <span data-ttu-id="2c1ac-211">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="2c1ac-211">Square Crop</span></span>  | <span data-ttu-id="2c1ac-212">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-212">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="2c1ac-213">176x176</span><span class="sxs-lookup"><span data-stu-id="2c1ac-213">176x176</span></span>     | <span data-ttu-id="2c1ac-214">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="2c1ac-214">Square Crop</span></span>  | <span data-ttu-id="2c1ac-215">小方形缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-215">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="2c1ac-216">800x800</span><span class="sxs-lookup"><span data-stu-id="2c1ac-216">800x800</span></span>     | <span data-ttu-id="2c1ac-217">方形裁剪</span><span class="sxs-lookup"><span data-stu-id="2c1ac-217">Square Crop</span></span>  | <span data-ttu-id="2c1ac-218">大方形缩略图</span><span class="sxs-lookup"><span data-stu-id="2c1ac-218">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="2c1ac-219">请求自定义缩略图的大小</span><span class="sxs-lookup"><span data-stu-id="2c1ac-219">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="2c1ac-220">除了定义尺寸外，应用还可以指定前缀为 `c` 的缩略图尺寸，从而请求获取自定义缩略图尺寸。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-220">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="2c1ac-221">例如，如果你的应用需要 300x400 的缩略图，可以按如下所示请求获取此大小：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-221">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="http"></a>[<span data-ttu-id="2c1ac-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1ac-222">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_crop
```
# <a name="c"></a>[<span data-ttu-id="2c1ac-223">C#</span><span class="sxs-lookup"><span data-stu-id="2c1ac-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c1ac-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c1ac-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c1ac-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c1ac-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c1ac-226">Java</span><span class="sxs-lookup"><span data-stu-id="2c1ac-226">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2c1ac-227">响应只包含选定的自定义缩略图尺寸：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-227">Which responds with just the custom thumbnail size selected:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

<span data-ttu-id="2c1ac-228">可以在请求获取的缩略图尺寸后指定以下选项：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-228">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="2c1ac-229">自定义标识符示例</span><span class="sxs-lookup"><span data-stu-id="2c1ac-229">Examples of custom identifiers</span></span>

| <span data-ttu-id="2c1ac-230">缩略图标识符</span><span class="sxs-lookup"><span data-stu-id="2c1ac-230">Thumbnail identifier</span></span> | <span data-ttu-id="2c1ac-231">分辨率</span><span class="sxs-lookup"><span data-stu-id="2c1ac-231">Resolution</span></span>             | <span data-ttu-id="2c1ac-232">纵横比</span><span class="sxs-lookup"><span data-stu-id="2c1ac-232">Aspect ratio</span></span> | <span data-ttu-id="2c1ac-233">说明</span><span class="sxs-lookup"><span data-stu-id="2c1ac-233">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2c1ac-234">c300x400</span><span class="sxs-lookup"><span data-stu-id="2c1ac-234">c300x400</span></span>             | <span data-ttu-id="2c1ac-235">300x400 像素框</span><span class="sxs-lookup"><span data-stu-id="2c1ac-235">Bounded by 300x400 box</span></span> | <span data-ttu-id="2c1ac-236">原始大小</span><span class="sxs-lookup"><span data-stu-id="2c1ac-236">Original</span></span>     | <span data-ttu-id="2c1ac-237">生成适应在 300x400 像素框中显示的缩略图，纵横比不变</span><span class="sxs-lookup"><span data-stu-id="2c1ac-237">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="2c1ac-238">c300x400_crop</span><span class="sxs-lookup"><span data-stu-id="2c1ac-238">c300x400_crop</span></span>        | <span data-ttu-id="2c1ac-239">300x400</span><span class="sxs-lookup"><span data-stu-id="2c1ac-239">300x400</span></span>                | <span data-ttu-id="2c1ac-240">已裁剪</span><span class="sxs-lookup"><span data-stu-id="2c1ac-240">Cropped</span></span>      | <span data-ttu-id="2c1ac-p113">生成 300x400 像素缩略图。 具体方式为，重设图像大小以填充 300x400 框，并裁剪超出框外的内容。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="2c1ac-243">**注意：** 返回的缩略图可能与请求的像素尺寸不完全匹配，但与纵横比匹配。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-243">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="2c1ac-244">在某些情况下，如果缩略图已经存在并且可以轻松缩放来匹配请求的分辨率，则可能会返回比请求的大小更大的缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-244">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="2c1ac-245">备注</span><span class="sxs-lookup"><span data-stu-id="2c1ac-245">Remarks</span></span>

<span data-ttu-id="2c1ac-246">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-246">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="2c1ac-247">使用这些调用展开缩略图集合不适用于：</span><span class="sxs-lookup"><span data-stu-id="2c1ac-247">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="2c1ac-248">SharePoint Server 2016 不支持缩略图。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-248">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="2c1ac-249">错误响应</span><span class="sxs-lookup"><span data-stu-id="2c1ac-249">Error responses</span></span>

<span data-ttu-id="2c1ac-250">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="2c1ac-250">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath&quot;: &quot;Items/Thumbnails"
} -->

