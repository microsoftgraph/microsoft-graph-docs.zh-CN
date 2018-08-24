# <a name="imageinfo-resource-type"></a><span data-ttu-id="f93e5-101">imageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f93e5-101">imageInfo resource type</span></span>

<span data-ttu-id="f93e5-102">代表 [activity](../resources/projectrome_activity.md) 对象 [visualInfo](../resources/projectrome_visualinfo.md) 部分中 **attribution** 属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="f93e5-102">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome_visualinfo.md) part of the [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="f93e5-103">属性</span><span class="sxs-lookup"><span data-stu-id="f93e5-103">Properties</span></span>

|<span data-ttu-id="f93e5-104">名称</span><span class="sxs-lookup"><span data-stu-id="f93e5-104">Name</span></span> | <span data-ttu-id="f93e5-105">类型</span><span class="sxs-lookup"><span data-stu-id="f93e5-105">Type</span></span> | <span data-ttu-id="f93e5-106">说明</span><span class="sxs-lookup"><span data-stu-id="f93e5-106">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f93e5-107">iconUrl</span><span class="sxs-lookup"><span data-stu-id="f93e5-107">iconurl</span></span> | <span data-ttu-id="f93e5-108">字符串</span><span class="sxs-lookup"><span data-stu-id="f93e5-108">String</span></span> | <span data-ttu-id="f93e5-109">可选；指向一个表示用于生成活动的应用程序图标的 URI</span><span class="sxs-lookup"><span data-stu-id="f93e5-109">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="f93e5-110">alternateText</span><span class="sxs-lookup"><span data-stu-id="f93e5-110">alternateText</span></span> | <span data-ttu-id="f93e5-111">字符串</span><span class="sxs-lookup"><span data-stu-id="f93e5-111">String</span></span> | <span data-ttu-id="f93e5-112">可选；图像的替换文字可访问内容</span><span class="sxs-lookup"><span data-stu-id="f93e5-112">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="f93e5-113">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="f93e5-113">addImageQuery</span></span> | <span data-ttu-id="f93e5-114">布尔</span><span class="sxs-lookup"><span data-stu-id="f93e5-114">Boolean</span></span> | <span data-ttu-id="f93e5-115">可选；用来指示服务器能否动态呈现图像以响应参数化的参数。</span><span class="sxs-lookup"><span data-stu-id="f93e5-115">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="f93e5-116">例如，一幅高对比度图像</span><span class="sxs-lookup"><span data-stu-id="f93e5-116">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f93e5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f93e5-117">JSON Representation</span></span>

<span data-ttu-id="f93e5-118">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f93e5-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->