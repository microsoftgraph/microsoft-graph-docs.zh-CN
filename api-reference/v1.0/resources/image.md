# <a name="image-resource-type"></a><span data-ttu-id="30670-101">图像资源类型</span><span class="sxs-lookup"><span data-stu-id="30670-101">Image resource type</span></span>

<span data-ttu-id="30670-p101">**图像**资源将与图像相关的属性分组到一个单一结构。如果 [**DriveItem**](driveitem.md)具有一个非 null **图像**方面，则该项表示一个位图图像。</span><span class="sxs-lookup"><span data-stu-id="30670-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="30670-104">**注意：**如果该服务无法确定图像的宽度和高度，**图像**资源可能为空。</span><span class="sxs-lookup"><span data-stu-id="30670-104">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30670-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30670-105">JSON representation</span></span>

<span data-ttu-id="30670-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30670-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.image"
}-->

```json
{
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a><span data-ttu-id="30670-107">属性</span><span class="sxs-lookup"><span data-stu-id="30670-107">Properties</span></span>

| <span data-ttu-id="30670-108">属性</span><span class="sxs-lookup"><span data-stu-id="30670-108">Property</span></span>   | <span data-ttu-id="30670-109">类型</span><span class="sxs-lookup"><span data-stu-id="30670-109">Type</span></span>  | <span data-ttu-id="30670-110">说明</span><span class="sxs-lookup"><span data-stu-id="30670-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="30670-111">**高度**</span><span class="sxs-lookup"><span data-stu-id="30670-111">**height**</span></span> | <span data-ttu-id="30670-112">Int32</span><span class="sxs-lookup"><span data-stu-id="30670-112">Int32</span></span> | <span data-ttu-id="30670-p102">可选。图像的高度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="30670-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="30670-116">**宽度**</span><span class="sxs-lookup"><span data-stu-id="30670-116">**width**</span></span>  | <span data-ttu-id="30670-117">Int32</span><span class="sxs-lookup"><span data-stu-id="30670-117">Int32</span></span> | <span data-ttu-id="30670-p103">可选。图像的宽度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="30670-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="30670-121">注解</span><span class="sxs-lookup"><span data-stu-id="30670-121">Remarks</span></span>

<span data-ttu-id="30670-p104">在 OneDrive for Business 中，基于文件扩展名在应为图像的项目中返回此类资源。此类资源在 OneDrive for Business 中不返回任何属性。</span><span class="sxs-lookup"><span data-stu-id="30670-p104">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension. This resource returns no properties in OneDrive for Business.</span></span>

<span data-ttu-id="30670-124">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="30670-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
