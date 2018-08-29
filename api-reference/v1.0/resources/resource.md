# <a name="onenoteresource-resource-type"></a>OneNoteResource 资源类型

OneNote 页面上的图像或其他文件资源。 

可以获取资源的二进制数据，但是不支持获取资源对象或资源集合的 JSON 表示形式。

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

可通过向资源的 `content` 终结点发送 GET 请求获取特定资源的二进制数据：

```
GET ../onenote/resources/{id}/content
```

使用以下请求获取页面的 HTML 内容后将返回文件的资源 URI：

```
GET ../onenote/pages/{id}/content
```

在页面 HTML 中，`img` 标记包含 `data-fullres-src` 属性中的原始图像资源和 `src` 属性中经过优化的图像的终结点。
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

标记（表示 PDF、DOCX 和 PNG 等文件）包含 `data` 属性中的文件资源的终结点：`object`

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>属性

| 属性             | 类型            | 说明
|:---------------------|:----------------|:---------------------------------
| 内容              | 流          | 内容流
| contentUrl           | string (url)    | 用于下载内容的 URL

## <a name="relationships"></a>关系
无。


## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取资源二进制数据](../api/resource_get.md) | 流 |检索文件或图像资源的二进制数据。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->