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
# <a name="list-thumbnails-for-a-driveitem"></a>列出 DriveItem 的缩略图

命名空间：microsoft.graph

检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。

DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。

可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：

* 枚举项目的可用缩略图
* 检索项目的单个缩略图
* 检索缩略图的内容
* 在单个请求中检索多个项目的缩略图
* 检索自定义缩略图的大小
* 上载项目的自定义缩略图
* 确定是否存在自定义的上传缩略图

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$select`[OData 查询参数](/graph/query-parameters)自定义响应。

此外，此方法还支持通过追加查询参数来检索包含原始方向 EXIF 值且没有应用旋转的 `originalOrientation=true` 缩略图。
目前仅 OneDrive 个人版支持此操作。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。

## <a name="example"></a>示例

下面是检索当前用户的 OneDrive 中某个项的可用缩略图的请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


这将返回项的可用 **thumbnailSet** 的数组。 驱动器中的任何项都可以有零个或多个缩略图。

**注意：** 可以使用 _select_ 查询字符串参数，控制在 **ThumbnailSet** 中返回的缩略图尺寸。 例如，`/thumbnails?select=medium` 仅检索中等大小的缩略图。


### <a name="response"></a>响应

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

## <a name="get-a-single-thumbnail"></a>获取单个缩略图

通过在请求中直接解决来检索单个缩略图和大小的元数据。

### <a name="http-request"></a>HTTP 请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a>路径参数

| 名称         | 类型   | 说明                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| **item-id**  | string | 引用的项目的唯一标识符。                                           |
| **thumb-id** | number | 缩略图的索引，通常介于 0 到 4 之间。 如果没有自定义缩略图，索引为 0。 |
| **size**     | string | 请求获取的缩略图的尺寸。 可取值为下面列出的标准大小之一或自定义大小。 |

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

## <a name="retrieve-thumbnail-binary-content"></a>检索缩略图的二进制内容

可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。

### <a name="http-request"></a>HTTP 请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

本服务通过到缩略图 URL 的重定向进行响应。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

缩略图 URL 具有缓存安全性。 如果在项发生更改后需要生成新的缩略图，URL 将会更改。


## <a name="getting-thumbnails-while-listing-driveitems"></a>获取缩略图的同时列出 DriveItem

如果检索要显示的 DriveItem 资源的列表，可以使用 _$expand_ 查询字符串参数，以便同时包含这些资源的缩略图。
这使你的应用可以通过一个请求同时检索缩略图和项，而不是发出多个请求。

### <a name="http-request"></a>HTTP 请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

本服务通过 DriveItem 及其缩略图的列表进行响应。

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

## <a name="size-options"></a>大小选项

下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：

| 名称           | 分辨率  | 纵横比​​ | 说明                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 longest  | Original     | 小型的高压缩缩略图，裁剪为正方形纵横比。 |
| `medium`       | 176 longest | Original     | 裁剪为 OneDrive Web 视图的标准项目大小。         |
| `large`        | 800 longest
 | Original     | 最长边重设为 800 像素的缩略图。               |
| `smallSquare`  | 96x96       | 方形裁剪  | 小方形缩略图                                               |
| `mediumSquare` | 176x176     | 方形裁剪  | 小方形缩略图                                               |
| `largeSquare`  | 800x800     | 方形裁剪  | 大方形缩略图                                               |

## <a name="requesting-custom-thumbnail-sizes"></a>请求自定义缩略图的大小

除了定义尺寸外，应用还可以指定前缀为 `c` 的缩略图尺寸，从而请求获取自定义缩略图尺寸。
例如，如果你的应用需要 300x400 的缩略图，可以按如下所示请求获取此大小：


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_crop
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


响应只包含选定的自定义缩略图尺寸：

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

可以在请求获取的缩略图尺寸后指定以下选项：

### <a name="examples-of-custom-identifiers"></a>自定义标识符示例

| 缩略图标识符 | 分辨率             | 纵横比 | 说明                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| c300x400             | 300x400 像素框 | 原始大小     | 生成适应在 300x400 像素框中显示的缩略图，纵横比不变                                                                 |
| c300x400_crop        | 300x400                | 已裁剪      | 生成 300x400 像素缩略图。 具体方式为，重设图像大小以填充 300x400 框，并裁剪超出框外的内容。 |

**注意：** 返回的缩略图可能与请求的像素尺寸不完全匹配，但与纵横比匹配。
在某些情况下，如果缩略图已经存在并且可以轻松缩放来匹配请求的分辨率，则可能会返回比请求的大小更大的缩略图。

## <a name="remarks"></a>备注

**注意** 在 OneDrive for Business 和 SharePoint 中：

使用这些调用展开缩略图集合不适用于：

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

SharePoint Server 2016 不支持缩略图。

### <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

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

