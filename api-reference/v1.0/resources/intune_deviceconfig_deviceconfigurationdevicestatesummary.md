# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="c80f5-101">deviceConfigurationDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c80f5-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="c80f5-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c80f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c80f5-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c80f5-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="c80f5-104">方法</span><span class="sxs-lookup"><span data-stu-id="c80f5-104">Methods</span></span>
|<span data-ttu-id="c80f5-105">方法</span><span class="sxs-lookup"><span data-stu-id="c80f5-105">Method</span></span>|<span data-ttu-id="c80f5-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="c80f5-106">Return Type</span></span>|<span data-ttu-id="c80f5-107">说明</span><span class="sxs-lookup"><span data-stu-id="c80f5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c80f5-108">获取 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c80f5-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="c80f5-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c80f5-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="c80f5-110">读取 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c80f5-110">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="c80f5-111">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c80f5-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="c80f5-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c80f5-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="c80f5-113">更新 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c80f5-113">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c80f5-114">属性</span><span class="sxs-lookup"><span data-stu-id="c80f5-114">Properties</span></span>
|<span data-ttu-id="c80f5-115">属性</span><span class="sxs-lookup"><span data-stu-id="c80f5-115">Property</span></span>|<span data-ttu-id="c80f5-116">类型</span><span class="sxs-lookup"><span data-stu-id="c80f5-116">Type</span></span>|<span data-ttu-id="c80f5-117">说明</span><span class="sxs-lookup"><span data-stu-id="c80f5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c80f5-118">id</span><span class="sxs-lookup"><span data-stu-id="c80f5-118">id</span></span>|<span data-ttu-id="c80f5-119">String</span><span class="sxs-lookup"><span data-stu-id="c80f5-119">String</span></span>|<span data-ttu-id="c80f5-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c80f5-120">Key of the entity.</span></span>|
|<span data-ttu-id="c80f5-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-121">unknownDeviceCount</span></span>|<span data-ttu-id="c80f5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-122">Int32</span></span>|<span data-ttu-id="c80f5-123">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-123">Number of unknown devices</span></span>|
|<span data-ttu-id="c80f5-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="c80f5-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-125">Int32</span></span>|<span data-ttu-id="c80f5-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="c80f5-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-127">compliantDeviceCount</span></span>|<span data-ttu-id="c80f5-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-128">Int32</span></span>|<span data-ttu-id="c80f5-129">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-129">Number of compliant devices</span></span>|
|<span data-ttu-id="c80f5-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-130">remediatedDeviceCount</span></span>|<span data-ttu-id="c80f5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-131">Int32</span></span>|<span data-ttu-id="c80f5-132">已修正设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-132">Number of remediated devices</span></span>|
|<span data-ttu-id="c80f5-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c80f5-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-134">Int32</span></span>|<span data-ttu-id="c80f5-135">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c80f5-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-136">errorDeviceCount</span></span>|<span data-ttu-id="c80f5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-137">Int32</span></span>|<span data-ttu-id="c80f5-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-138">Number of error devices</span></span>|
|<span data-ttu-id="c80f5-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c80f5-139">conflictDeviceCount</span></span>|<span data-ttu-id="c80f5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c80f5-140">Int32</span></span>|<span data-ttu-id="c80f5-141">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="c80f5-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c80f5-142">关系</span><span class="sxs-lookup"><span data-stu-id="c80f5-142">Relationships</span></span>
<span data-ttu-id="c80f5-143">无</span><span class="sxs-lookup"><span data-stu-id="c80f5-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c80f5-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c80f5-144">JSON Representation</span></span>
<span data-ttu-id="c80f5-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c80f5-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



