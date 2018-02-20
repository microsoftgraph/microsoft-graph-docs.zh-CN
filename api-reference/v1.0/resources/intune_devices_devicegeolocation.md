# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="78d9a-101">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="78d9a-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="78d9a-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="78d9a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78d9a-103">设备位置</span><span class="sxs-lookup"><span data-stu-id="78d9a-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="78d9a-104">属性</span><span class="sxs-lookup"><span data-stu-id="78d9a-104">Properties</span></span>
|<span data-ttu-id="78d9a-105">属性</span><span class="sxs-lookup"><span data-stu-id="78d9a-105">Property</span></span>|<span data-ttu-id="78d9a-106">类型</span><span class="sxs-lookup"><span data-stu-id="78d9a-106">Type</span></span>|<span data-ttu-id="78d9a-107">说明</span><span class="sxs-lookup"><span data-stu-id="78d9a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78d9a-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="78d9a-108">lastCollectedDateTime</span></span>|<span data-ttu-id="78d9a-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d9a-109">DateTimeOffset</span></span>|<span data-ttu-id="78d9a-110">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="78d9a-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="78d9a-111">longitude</span><span class="sxs-lookup"><span data-stu-id="78d9a-111">longitude</span></span>|<span data-ttu-id="78d9a-112">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-112">Double</span></span>|<span data-ttu-id="78d9a-113">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="78d9a-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="78d9a-114">latitude</span><span class="sxs-lookup"><span data-stu-id="78d9a-114">latitude</span></span>|<span data-ttu-id="78d9a-115">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-115">Double</span></span>|<span data-ttu-id="78d9a-116">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="78d9a-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="78d9a-117">altitude</span><span class="sxs-lookup"><span data-stu-id="78d9a-117">altitude</span></span>|<span data-ttu-id="78d9a-118">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-118">Double</span></span>|<span data-ttu-id="78d9a-119">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="78d9a-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="78d9a-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="78d9a-120">horizontalAccuracy</span></span>|<span data-ttu-id="78d9a-121">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-121">Double</span></span>|<span data-ttu-id="78d9a-122">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="78d9a-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="78d9a-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="78d9a-123">verticalAccuracy</span></span>|<span data-ttu-id="78d9a-124">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-124">Double</span></span>|<span data-ttu-id="78d9a-125">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="78d9a-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="78d9a-126">heading</span><span class="sxs-lookup"><span data-stu-id="78d9a-126">heading</span></span>|<span data-ttu-id="78d9a-127">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-127">Double</span></span>|<span data-ttu-id="78d9a-128">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="78d9a-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="78d9a-129">speed</span><span class="sxs-lookup"><span data-stu-id="78d9a-129">speed</span></span>|<span data-ttu-id="78d9a-130">Double</span><span class="sxs-lookup"><span data-stu-id="78d9a-130">Double</span></span>|<span data-ttu-id="78d9a-131">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="78d9a-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d9a-132">关系</span><span class="sxs-lookup"><span data-stu-id="78d9a-132">Relationships</span></span>
<span data-ttu-id="78d9a-133">无</span><span class="sxs-lookup"><span data-stu-id="78d9a-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78d9a-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78d9a-134">JSON Representation</span></span>
<span data-ttu-id="78d9a-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78d9a-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



