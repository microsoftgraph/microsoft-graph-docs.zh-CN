# <a name="list-thumbnails-for-a-driveitem"></a>列出 DriveItem 的缩略图

检索 [DriveItem](../resources/driveitem.md) 资源的 [ThumbnailSet](../resources/thumbnailset.md) 资源集合。

DriveItem 可以由零个或多个 [ThumbnailSet](../resources/thumbnailset.md) 资源表示。每个 **thumbnailSet** 都可以有一个或多个 [**thumbnail**](../resources/thumbnail.md) 对象，此类对象是表示项目的图像。例如，**thumbnailSet** 可包括 **thumbnail** 对象，例如包括 `small`、`medium` 或 `large` 等常见对象。

可以通过多种方式在 OneDrive 上对缩略图进行操作。以下是一些最常见的操作：

* 枚举项目的可用缩略图
* 检索项目的单个缩略图
* 检索缩略图的内容
* 在单个请求中检索多个项目的缩略图
* 检索自定义缩略图的大小
* 上载项目的自定义缩略图
* 确定是否存在自定义的上载缩略图


## <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**之一：

* Files.Read
* Files.ReadWrite
* Files.Read.All
* Files.ReadWrite.All
* Sites.Read.All
* Sites.ReadWrite.All


## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ThumbnailSet](../resources/thumbnailset.md) 对象集合。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a>响应
下面是一个响应示例。

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

## <a name="retrieve-a-single-thumbnail"></a>检索单个缩略图

通过请求中直接解决来检索单个缩略图和大小的元数据。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a>Path 参数

| 名称         | 类型   | 说明                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| **item-id**  | string | 引用的项目的唯一标识符。                                      |
| **thumb-id** | 数字 | 缩略图的索引，通常为 0 到 4。                                            |
| **size**     | string | 请求的缩略图大小。这必须是列出的其中一个标准大小。 |


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

## <a name="retrieve-thumbnail-content"></a>检索缩略图的内容

可以通过请求缩略图的 **content** 属性直接检索缩略图的内容。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a>响应

本服务用到缩略图 URL 的重定向进行响应。

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

缩略图的内容 URL 已经过预身份验证，无需下载授权标头。这些 URL 是临时存在的，仅在数小时内有效，不应由应用进行缓存。


## <a name="size-values"></a>Size 的值

下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：

| 名称           | 分辨率  | 纵横比​​ | 说明                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 longest  | Original     | 小型的高压缩缩略图，裁剪为正方形纵横比。 |
| `medium`       | 176 longest | Original     | 裁剪为 OneDrive Web 视图的标准项目大小。         |
| `large`        | 800 longest
 | Original     | 最长边调整到 800 像素的缩略图。               |

## <a name="remarks"></a>注解

**注意** 在 OneDrive for Business 和 SharePoint 中：

* 使用这些调用展开缩略图集合不适用于：`GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
