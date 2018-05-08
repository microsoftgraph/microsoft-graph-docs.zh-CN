# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="32341-101">outlookGeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="32341-101">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="32341-102">地理坐标、海拔，以及它们物理位置的精确度。</span><span class="sxs-lookup"><span data-stu-id="32341-102">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32341-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32341-103">JSON representation</span></span>

<span data-ttu-id="32341-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32341-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="32341-105">属性</span><span class="sxs-lookup"><span data-stu-id="32341-105">Properties</span></span>
| <span data-ttu-id="32341-106">属性</span><span class="sxs-lookup"><span data-stu-id="32341-106">Property</span></span>     | <span data-ttu-id="32341-107">类型</span><span class="sxs-lookup"><span data-stu-id="32341-107">Type</span></span>   |<span data-ttu-id="32341-108">说明</span><span class="sxs-lookup"><span data-stu-id="32341-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32341-109">accuracy</span><span class="sxs-lookup"><span data-stu-id="32341-109">accuracy</span></span>|<span data-ttu-id="32341-110">double</span><span class="sxs-lookup"><span data-stu-id="32341-110">double</span></span>|<span data-ttu-id="32341-111">纬度和经度的精确度。</span><span class="sxs-lookup"><span data-stu-id="32341-111">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="32341-112">举个例子，精确度可以以米为单位度量，如纬度和经度可以精确到 50 米内。</span><span class="sxs-lookup"><span data-stu-id="32341-112">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="32341-113">altitude</span><span class="sxs-lookup"><span data-stu-id="32341-113">altitude</span></span>|<span data-ttu-id="32341-114">double</span><span class="sxs-lookup"><span data-stu-id="32341-114">double</span></span>|<span data-ttu-id="32341-115">位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="32341-115">The altitude of the location.</span></span>|
|<span data-ttu-id="32341-116">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="32341-116">altitudeAccuracy</span></span>|<span data-ttu-id="32341-117">double</span><span class="sxs-lookup"><span data-stu-id="32341-117">double</span></span>|<span data-ttu-id="32341-118">海拔高度的精确度。</span><span class="sxs-lookup"><span data-stu-id="32341-118">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="32341-119">latitude</span><span class="sxs-lookup"><span data-stu-id="32341-119">latitude</span></span>|<span data-ttu-id="32341-120">double</span><span class="sxs-lookup"><span data-stu-id="32341-120">double</span></span>|<span data-ttu-id="32341-121">位置的纬度。</span><span class="sxs-lookup"><span data-stu-id="32341-121">The latitude of the location.</span></span>|
|<span data-ttu-id="32341-122">longitude</span><span class="sxs-lookup"><span data-stu-id="32341-122">longitude</span></span>|<span data-ttu-id="32341-123">double</span><span class="sxs-lookup"><span data-stu-id="32341-123">double</span></span>|<span data-ttu-id="32341-124">位置的经度。</span><span class="sxs-lookup"><span data-stu-id="32341-124">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->