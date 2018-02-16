# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="1d25a-101">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d25a-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="1d25a-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1d25a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d25a-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1d25a-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1d25a-104">方法</span><span class="sxs-lookup"><span data-stu-id="1d25a-104">Methods</span></span>
|<span data-ttu-id="1d25a-105">方法</span><span class="sxs-lookup"><span data-stu-id="1d25a-105">Method</span></span>|<span data-ttu-id="1d25a-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d25a-106">Return Type</span></span>|<span data-ttu-id="1d25a-107">说明</span><span class="sxs-lookup"><span data-stu-id="1d25a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d25a-108">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1d25a-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="1d25a-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1d25a-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1d25a-110">读取 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d25a-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="1d25a-111">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1d25a-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="1d25a-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1d25a-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1d25a-113">更新 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1d25a-113">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d25a-114">属性</span><span class="sxs-lookup"><span data-stu-id="1d25a-114">Properties</span></span>
|<span data-ttu-id="1d25a-115">属性</span><span class="sxs-lookup"><span data-stu-id="1d25a-115">Property</span></span>|<span data-ttu-id="1d25a-116">类型</span><span class="sxs-lookup"><span data-stu-id="1d25a-116">Type</span></span>|<span data-ttu-id="1d25a-117">说明</span><span class="sxs-lookup"><span data-stu-id="1d25a-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d25a-118">id</span><span class="sxs-lookup"><span data-stu-id="1d25a-118">id</span></span>|<span data-ttu-id="1d25a-119">String</span><span class="sxs-lookup"><span data-stu-id="1d25a-119">String</span></span>|<span data-ttu-id="1d25a-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d25a-120">Key of the setting.</span></span>|
|<span data-ttu-id="1d25a-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1d25a-121">pendingCount</span></span>|<span data-ttu-id="1d25a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1d25a-122">Int32</span></span>|<span data-ttu-id="1d25a-123">待定设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d25a-123">Number of pending devices</span></span>|
|<span data-ttu-id="1d25a-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1d25a-124">notApplicableCount</span></span>|<span data-ttu-id="1d25a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1d25a-125">Int32</span></span>|<span data-ttu-id="1d25a-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d25a-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="1d25a-127">successCount</span><span class="sxs-lookup"><span data-stu-id="1d25a-127">successCount</span></span>|<span data-ttu-id="1d25a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1d25a-128">Int32</span></span>|<span data-ttu-id="1d25a-129">成功的设备数量</span><span class="sxs-lookup"><span data-stu-id="1d25a-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="1d25a-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="1d25a-130">errorCount</span></span>|<span data-ttu-id="1d25a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1d25a-131">Int32</span></span>|<span data-ttu-id="1d25a-132">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="1d25a-132">Number of error devices</span></span>|
|<span data-ttu-id="1d25a-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="1d25a-133">failedCount</span></span>|<span data-ttu-id="1d25a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="1d25a-134">Int32</span></span>|<span data-ttu-id="1d25a-135">失败的设备数量</span><span class="sxs-lookup"><span data-stu-id="1d25a-135">Number of failed devices</span></span>|
|<span data-ttu-id="1d25a-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1d25a-136">lastUpdateDateTime</span></span>|<span data-ttu-id="1d25a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d25a-137">DateTimeOffset</span></span>|<span data-ttu-id="1d25a-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="1d25a-138">Last update time</span></span>|
|<span data-ttu-id="1d25a-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1d25a-139">configurationVersion</span></span>|<span data-ttu-id="1d25a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1d25a-140">Int32</span></span>|<span data-ttu-id="1d25a-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="1d25a-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d25a-142">关系</span><span class="sxs-lookup"><span data-stu-id="1d25a-142">Relationships</span></span>
<span data-ttu-id="1d25a-143">无</span><span class="sxs-lookup"><span data-stu-id="1d25a-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d25a-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d25a-144">JSON Representation</span></span>
<span data-ttu-id="1d25a-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d25a-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



