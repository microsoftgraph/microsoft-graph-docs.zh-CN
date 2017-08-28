# <a name="photo-resource-type"></a><span data-ttu-id="baad8-101">照片资源类型</span><span class="sxs-lookup"><span data-stu-id="baad8-101">Photo resource type</span></span>

<span data-ttu-id="baad8-102">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="baad8-102">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="baad8-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baad8-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="baad8-104">属性</span><span class="sxs-lookup"><span data-stu-id="baad8-104">Properties</span></span>
| <span data-ttu-id="baad8-105">属性</span><span class="sxs-lookup"><span data-stu-id="baad8-105">Property</span></span>                | <span data-ttu-id="baad8-106">类型</span><span class="sxs-lookup"><span data-stu-id="baad8-106">Type</span></span>                      | <span data-ttu-id="baad8-107">说明</span><span class="sxs-lookup"><span data-stu-id="baad8-107">Description</span></span>                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| <span data-ttu-id="baad8-108">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="baad8-108">**takenDateTime**</span></span>       | <span data-ttu-id="baad8-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baad8-109">DateTimeOffset</span></span>            | <span data-ttu-id="baad8-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p101">Represents the date and time the photo was taken. Read-only.</span></span>               |
| <span data-ttu-id="baad8-112">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="baad8-112">**cameraMake**</span></span>          | <span data-ttu-id="baad8-113">String</span><span class="sxs-lookup"><span data-stu-id="baad8-113">String</span></span>                    | <span data-ttu-id="baad8-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p102">Camera manufacturer. Read-only.</span></span>                                            |
| <span data-ttu-id="baad8-116">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="baad8-116">**cameraModel**</span></span>         | <span data-ttu-id="baad8-117">String</span><span class="sxs-lookup"><span data-stu-id="baad8-117">String</span></span>                    | <span data-ttu-id="baad8-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p103">Camera model. Read-only.</span></span>                                                   |
| <span data-ttu-id="baad8-120">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="baad8-120">**fNumber**</span></span>             | <span data-ttu-id="baad8-121">Double</span><span class="sxs-lookup"><span data-stu-id="baad8-121">Double</span></span>                    | <span data-ttu-id="baad8-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p104">The F-stop value from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="baad8-124">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="baad8-124">**exposureDenominator**</span></span> | <span data-ttu-id="baad8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="baad8-125">Int32</span></span>                     | <span data-ttu-id="baad8-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
| <span data-ttu-id="baad8-128">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="baad8-128">**exposureNumerator**</span></span>   | <span data-ttu-id="baad8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="baad8-129">Int32</span></span>                     | <span data-ttu-id="baad8-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
| <span data-ttu-id="baad8-132">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="baad8-132">**focalLength**</span></span>         | <span data-ttu-id="baad8-133">Double</span><span class="sxs-lookup"><span data-stu-id="baad8-133">Double</span></span>                    | <span data-ttu-id="baad8-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p107">The focal length from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="baad8-136">**iso**</span><span class="sxs-lookup"><span data-stu-id="baad8-136">**iso**</span></span>                 | <span data-ttu-id="baad8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="baad8-137">Int32</span></span>                     | <span data-ttu-id="baad8-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="baad8-p108">The ISO value from the camera. Read-only.</span></span>                                  |

## <a name="remarks"></a><span data-ttu-id="baad8-140">注解</span><span class="sxs-lookup"><span data-stu-id="baad8-140">Remarks</span></span>
<span data-ttu-id="baad8-141">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="baad8-141">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="baad8-142">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="baad8-142">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
