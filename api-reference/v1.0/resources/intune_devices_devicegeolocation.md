# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="3f394-101">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f394-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="3f394-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3f394-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f394-103">设备位置</span><span class="sxs-lookup"><span data-stu-id="3f394-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="3f394-104">属性</span><span class="sxs-lookup"><span data-stu-id="3f394-104">Properties</span></span>
|<span data-ttu-id="3f394-105">属性</span><span class="sxs-lookup"><span data-stu-id="3f394-105">Property</span></span>|<span data-ttu-id="3f394-106">类型</span><span class="sxs-lookup"><span data-stu-id="3f394-106">Type</span></span>|<span data-ttu-id="3f394-107">说明</span><span class="sxs-lookup"><span data-stu-id="3f394-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f394-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f394-108">lastCollectedDateTime</span></span>|<span data-ttu-id="3f394-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f394-109">DateTimeOffset</span></span>|<span data-ttu-id="3f394-110">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="3f394-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3f394-111">longitude</span><span class="sxs-lookup"><span data-stu-id="3f394-111">longitude</span></span>|<span data-ttu-id="3f394-112">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-112">Double</span></span>|<span data-ttu-id="3f394-113">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="3f394-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3f394-114">latitude</span><span class="sxs-lookup"><span data-stu-id="3f394-114">latitude</span></span>|<span data-ttu-id="3f394-115">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-115">Double</span></span>|<span data-ttu-id="3f394-116">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="3f394-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3f394-117">altitude</span><span class="sxs-lookup"><span data-stu-id="3f394-117">altitude</span></span>|<span data-ttu-id="3f394-118">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-118">Double</span></span>|<span data-ttu-id="3f394-119">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="3f394-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="3f394-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3f394-120">horizontalAccuracy</span></span>|<span data-ttu-id="3f394-121">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-121">Double</span></span>|<span data-ttu-id="3f394-122">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="3f394-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="3f394-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3f394-123">verticalAccuracy</span></span>|<span data-ttu-id="3f394-124">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-124">Double</span></span>|<span data-ttu-id="3f394-125">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="3f394-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="3f394-126">heading</span><span class="sxs-lookup"><span data-stu-id="3f394-126">heading</span></span>|<span data-ttu-id="3f394-127">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-127">Double</span></span>|<span data-ttu-id="3f394-128">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="3f394-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="3f394-129">speed</span><span class="sxs-lookup"><span data-stu-id="3f394-129">speed</span></span>|<span data-ttu-id="3f394-130">Double</span><span class="sxs-lookup"><span data-stu-id="3f394-130">Double</span></span>|<span data-ttu-id="3f394-131">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="3f394-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f394-132">关系</span><span class="sxs-lookup"><span data-stu-id="3f394-132">Relationships</span></span>
<span data-ttu-id="3f394-133">无</span><span class="sxs-lookup"><span data-stu-id="3f394-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3f394-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f394-134">JSON Representation</span></span>
<span data-ttu-id="3f394-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f394-135">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616,
  "horizontalAccuracy": 2.9,
  "verticalAccuracy": 1.25,
  "heading": 36.3,
  "speed": 705.9

}
```



