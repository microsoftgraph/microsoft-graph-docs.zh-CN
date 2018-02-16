# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="89de9-101">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="89de9-101">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="89de9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89de9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89de9-103">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="89de9-103">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="89de9-104">方法</span><span class="sxs-lookup"><span data-stu-id="89de9-104">Methods</span></span>
|<span data-ttu-id="89de9-105">方法</span><span class="sxs-lookup"><span data-stu-id="89de9-105">Method</span></span>|<span data-ttu-id="89de9-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="89de9-106">Return Type</span></span>|<span data-ttu-id="89de9-107">说明</span><span class="sxs-lookup"><span data-stu-id="89de9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89de9-108">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="89de9-108">Get managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_get.md)|[<span data-ttu-id="89de9-109">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="89de9-109">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="89de9-110">读取 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89de9-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="89de9-111">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="89de9-111">Update managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_update.md)|[<span data-ttu-id="89de9-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="89de9-112">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="89de9-113">更新 [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89de9-113">Update the properties of a [calendar](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89de9-114">属性</span><span class="sxs-lookup"><span data-stu-id="89de9-114">Properties</span></span>
|<span data-ttu-id="89de9-115">属性</span><span class="sxs-lookup"><span data-stu-id="89de9-115">Property</span></span>|<span data-ttu-id="89de9-116">类型</span><span class="sxs-lookup"><span data-stu-id="89de9-116">Type</span></span>|<span data-ttu-id="89de9-117">说明</span><span class="sxs-lookup"><span data-stu-id="89de9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89de9-118">id</span><span class="sxs-lookup"><span data-stu-id="89de9-118">id</span></span>|<span data-ttu-id="89de9-119">String</span><span class="sxs-lookup"><span data-stu-id="89de9-119">String</span></span>|<span data-ttu-id="89de9-120">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="89de9-120">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="89de9-121">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89de9-121">enrolledDeviceCount</span></span>|<span data-ttu-id="89de9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="89de9-122">Int32</span></span>|<span data-ttu-id="89de9-123">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="89de9-123">Total enrolled device count.</span></span> <span data-ttu-id="89de9-124">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="89de9-124">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="89de9-125">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="89de9-125">mdmEnrolledCount</span></span>|<span data-ttu-id="89de9-126">Int32</span><span class="sxs-lookup"><span data-stu-id="89de9-126">Int32</span></span>|<span data-ttu-id="89de9-127">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="89de9-127">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="89de9-128">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89de9-128">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="89de9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="89de9-129">Int32</span></span>|<span data-ttu-id="89de9-130">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="89de9-130">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="89de9-131">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="89de9-131">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="89de9-132">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="89de9-132">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="89de9-133">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="89de9-133">Device operating system summary.</span></span>|
|<span data-ttu-id="89de9-134">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="89de9-134">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="89de9-135">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="89de9-135">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="89de9-136">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="89de9-136">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="89de9-137">关系</span><span class="sxs-lookup"><span data-stu-id="89de9-137">Relationships</span></span>
<span data-ttu-id="89de9-138">无</span><span class="sxs-lookup"><span data-stu-id="89de9-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89de9-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89de9-139">JSON Representation</span></span>
<span data-ttu-id="89de9-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89de9-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



