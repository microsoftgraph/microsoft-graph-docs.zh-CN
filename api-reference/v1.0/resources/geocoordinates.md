# <a name="geocoordinates-resource-type"></a><span data-ttu-id="e77ad-101">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="e77ad-101">GeoCoordinates resource type</span></span>

<span data-ttu-id="e77ad-p101">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="e77ad-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e77ad-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e77ad-104">JSON representation</span></span>

<span data-ttu-id="e77ad-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e77ad-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="e77ad-106">属性</span><span class="sxs-lookup"><span data-stu-id="e77ad-106">Properties</span></span>

| <span data-ttu-id="e77ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="e77ad-107">Property</span></span>  | <span data-ttu-id="e77ad-108">类型</span><span class="sxs-lookup"><span data-stu-id="e77ad-108">Type</span></span>   | <span data-ttu-id="e77ad-109">说明</span><span class="sxs-lookup"><span data-stu-id="e77ad-109">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="e77ad-110">海拔</span><span class="sxs-lookup"><span data-stu-id="e77ad-110">altitude</span></span>  | <span data-ttu-id="e77ad-111">双精度数</span><span class="sxs-lookup"><span data-stu-id="e77ad-111">Double</span></span> | <span data-ttu-id="e77ad-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="e77ad-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span> |
| <span data-ttu-id="e77ad-115">纬度</span><span class="sxs-lookup"><span data-stu-id="e77ad-115">latitude</span></span>  | <span data-ttu-id="e77ad-116">双精度数</span><span class="sxs-lookup"><span data-stu-id="e77ad-116">Double</span></span> | <span data-ttu-id="e77ad-p103">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="e77ad-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>   |
| <span data-ttu-id="e77ad-120">经度</span><span class="sxs-lookup"><span data-stu-id="e77ad-120">longitude</span></span> | <span data-ttu-id="e77ad-121">双精度数</span><span class="sxs-lookup"><span data-stu-id="e77ad-121">Double</span></span> | <span data-ttu-id="e77ad-p104">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="e77ad-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="e77ad-125">注解</span><span class="sxs-lookup"><span data-stu-id="e77ad-125">Remarks</span></span>

<span data-ttu-id="e77ad-126">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e77ad-126">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
