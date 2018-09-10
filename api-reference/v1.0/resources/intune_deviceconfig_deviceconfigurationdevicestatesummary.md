# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="94442-101">deviceConfigurationDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="94442-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="94442-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="94442-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94442-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94442-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="94442-104">方法</span><span class="sxs-lookup"><span data-stu-id="94442-104">Methods</span></span>
|<span data-ttu-id="94442-105">方法</span><span class="sxs-lookup"><span data-stu-id="94442-105">Method</span></span>|<span data-ttu-id="94442-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="94442-106">Return Type</span></span>|<span data-ttu-id="94442-107">说明</span><span class="sxs-lookup"><span data-stu-id="94442-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94442-108">获取 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="94442-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="94442-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="94442-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="94442-110">读取 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94442-110">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="94442-111">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="94442-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="94442-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="94442-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="94442-113">更新 [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94442-113">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94442-114">属性</span><span class="sxs-lookup"><span data-stu-id="94442-114">Properties</span></span>
|<span data-ttu-id="94442-115">属性</span><span class="sxs-lookup"><span data-stu-id="94442-115">Property</span></span>|<span data-ttu-id="94442-116">类型</span><span class="sxs-lookup"><span data-stu-id="94442-116">Type</span></span>|<span data-ttu-id="94442-117">说明</span><span class="sxs-lookup"><span data-stu-id="94442-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94442-118">ID</span><span class="sxs-lookup"><span data-stu-id="94442-118">id</span></span>|<span data-ttu-id="94442-119">字符串</span><span class="sxs-lookup"><span data-stu-id="94442-119">String</span></span>|<span data-ttu-id="94442-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94442-120">Key of the entity.</span></span>|
|<span data-ttu-id="94442-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-121">unknownDeviceCount</span></span>|<span data-ttu-id="94442-122">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-122">Int32</span></span>|<span data-ttu-id="94442-123">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-123">Number of unknown devices</span></span>|
|<span data-ttu-id="94442-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="94442-125">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-125">Int32</span></span>|<span data-ttu-id="94442-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="94442-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-127">compliantDeviceCount</span></span>|<span data-ttu-id="94442-128">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-128">Int32</span></span>|<span data-ttu-id="94442-129">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-129">Number of compliant devices</span></span>|
|<span data-ttu-id="94442-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-130">remediatedDeviceCount</span></span>|<span data-ttu-id="94442-131">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-131">Int32</span></span>|<span data-ttu-id="94442-132">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-132">Number of remediated devices</span></span>|
|<span data-ttu-id="94442-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="94442-134">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-134">Int32</span></span>|<span data-ttu-id="94442-135">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="94442-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-136">errorDeviceCount</span></span>|<span data-ttu-id="94442-137">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-137">Int32</span></span>|<span data-ttu-id="94442-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-138">Number of error devices</span></span>|
|<span data-ttu-id="94442-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94442-139">conflictDeviceCount</span></span>|<span data-ttu-id="94442-140">Int32</span><span class="sxs-lookup"><span data-stu-id="94442-140">Int32</span></span>|<span data-ttu-id="94442-141">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="94442-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="94442-142">关系</span><span class="sxs-lookup"><span data-stu-id="94442-142">Relationships</span></span>
<span data-ttu-id="94442-143">无</span><span class="sxs-lookup"><span data-stu-id="94442-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94442-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94442-144">JSON Representation</span></span>
<span data-ttu-id="94442-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94442-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}-->
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








