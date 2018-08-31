# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="00a15-101">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="00a15-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="00a15-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00a15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00a15-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="00a15-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="00a15-104">方法</span><span class="sxs-lookup"><span data-stu-id="00a15-104">Methods</span></span>
|<span data-ttu-id="00a15-105">方法</span><span class="sxs-lookup"><span data-stu-id="00a15-105">Method</span></span>|<span data-ttu-id="00a15-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="00a15-106">Return Type</span></span>|<span data-ttu-id="00a15-107">说明</span><span class="sxs-lookup"><span data-stu-id="00a15-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00a15-108">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="00a15-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="00a15-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="00a15-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="00a15-110">读取 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00a15-110">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="00a15-111">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="00a15-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="00a15-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="00a15-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="00a15-113">更新 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00a15-113">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00a15-114">属性</span><span class="sxs-lookup"><span data-stu-id="00a15-114">Properties</span></span>
|<span data-ttu-id="00a15-115">属性</span><span class="sxs-lookup"><span data-stu-id="00a15-115">Property</span></span>|<span data-ttu-id="00a15-116">类型</span><span class="sxs-lookup"><span data-stu-id="00a15-116">Type</span></span>|<span data-ttu-id="00a15-117">说明</span><span class="sxs-lookup"><span data-stu-id="00a15-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a15-118">id</span><span class="sxs-lookup"><span data-stu-id="00a15-118">id</span></span>|<span data-ttu-id="00a15-119">字符串</span><span class="sxs-lookup"><span data-stu-id="00a15-119">String</span></span>|<span data-ttu-id="00a15-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="00a15-120">Key of the entity.</span></span>|
|<span data-ttu-id="00a15-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="00a15-121">pendingCount</span></span>|<span data-ttu-id="00a15-122">Int32</span><span class="sxs-lookup"><span data-stu-id="00a15-122">Int32</span></span>|<span data-ttu-id="00a15-123">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="00a15-123">Number of pending devices</span></span>|
|<span data-ttu-id="00a15-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="00a15-124">notApplicableCount</span></span>|<span data-ttu-id="00a15-125">Int32</span><span class="sxs-lookup"><span data-stu-id="00a15-125">Int32</span></span>|<span data-ttu-id="00a15-126">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="00a15-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="00a15-127">successCount</span><span class="sxs-lookup"><span data-stu-id="00a15-127">successCount</span></span>|<span data-ttu-id="00a15-128">Int32</span><span class="sxs-lookup"><span data-stu-id="00a15-128">Int32</span></span>|<span data-ttu-id="00a15-129">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="00a15-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="00a15-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="00a15-130">errorCount</span></span>|<span data-ttu-id="00a15-131">Int32</span><span class="sxs-lookup"><span data-stu-id="00a15-131">Int32</span></span>|<span data-ttu-id="00a15-132">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="00a15-132">Number of error devices</span></span>|
|<span data-ttu-id="00a15-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="00a15-133">failedCount</span></span>|<span data-ttu-id="00a15-134">Int32</span><span class="sxs-lookup"><span data-stu-id="00a15-134">Int32</span></span>|<span data-ttu-id="00a15-135">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="00a15-135">Number of failed devices</span></span>|
|<span data-ttu-id="00a15-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="00a15-136">lastUpdateDateTime</span></span>|<span data-ttu-id="00a15-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a15-137">DateTimeOffset</span></span>|<span data-ttu-id="00a15-138">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="00a15-138">Last update time</span></span>|
|<span data-ttu-id="00a15-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="00a15-139">configurationVersion</span></span>|<span data-ttu-id="00a15-140">Int32</span><span class="sxs-lookup"><span data-stu-id="00a15-140">Int32</span></span>|<span data-ttu-id="00a15-141">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="00a15-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="00a15-142">关系</span><span class="sxs-lookup"><span data-stu-id="00a15-142">Relationships</span></span>
<span data-ttu-id="00a15-143">无</span><span class="sxs-lookup"><span data-stu-id="00a15-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00a15-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00a15-144">JSON Representation</span></span>
<span data-ttu-id="00a15-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00a15-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}-->
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



