# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="0f939-101">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f939-101">deviceConfiguration resource type</span></span>

> <span data-ttu-id="0f939-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0f939-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f939-103">设备配置。</span><span class="sxs-lookup"><span data-stu-id="0f939-103">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="0f939-104">方法</span><span class="sxs-lookup"><span data-stu-id="0f939-104">Methods</span></span>
|<span data-ttu-id="0f939-105">方法</span><span class="sxs-lookup"><span data-stu-id="0f939-105">Method</span></span>|<span data-ttu-id="0f939-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f939-106">Return Type</span></span>|<span data-ttu-id="0f939-107">说明</span><span class="sxs-lookup"><span data-stu-id="0f939-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f939-108">列出deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="0f939-108">List deviceConfigurations</span></span>](../api/intune_deviceconfig_deviceconfiguration_list.md)|<span data-ttu-id="0f939-109">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f939-109">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) collection</span></span>|<span data-ttu-id="0f939-110">列出 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f939-110">List properties and relationships of the [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0f939-111">获取deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f939-111">Get deviceConfiguration</span></span>](../api/intune_deviceconfig_deviceconfiguration_get.md)|[<span data-ttu-id="0f939-112">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f939-112">deviceConfiguration</span></span>](../resources/intune_deviceconfig_deviceconfiguration.md)|<span data-ttu-id="0f939-113">读取 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f939-113">Read properties and relationships of the [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0f939-114">assign 操作</span><span class="sxs-lookup"><span data-stu-id="0f939-114">assign action</span></span>](../api/intune_deviceconfig_deviceconfiguration_assign.md)|<span data-ttu-id="0f939-115">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f939-115">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0f939-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0f939-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0f939-117">属性</span><span class="sxs-lookup"><span data-stu-id="0f939-117">Properties</span></span>
|<span data-ttu-id="0f939-118">属性</span><span class="sxs-lookup"><span data-stu-id="0f939-118">Property</span></span>|<span data-ttu-id="0f939-119">类型</span><span class="sxs-lookup"><span data-stu-id="0f939-119">Type</span></span>|<span data-ttu-id="0f939-120">说明</span><span class="sxs-lookup"><span data-stu-id="0f939-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f939-121">ID</span><span class="sxs-lookup"><span data-stu-id="0f939-121">id</span></span>|<span data-ttu-id="0f939-122">字符串</span><span class="sxs-lookup"><span data-stu-id="0f939-122">String</span></span>|<span data-ttu-id="0f939-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f939-123">Key of the entity.</span></span>|
|<span data-ttu-id="0f939-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f939-124">lastModifiedDateTime</span></span>|<span data-ttu-id="0f939-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f939-125">DateTimeOffset</span></span>|<span data-ttu-id="0f939-126">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f939-126">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0f939-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f939-127">createdDateTime</span></span>|<span data-ttu-id="0f939-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f939-128">DateTimeOffset</span></span>|<span data-ttu-id="0f939-129">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f939-129">DateTime the object was created.</span></span>|
|<span data-ttu-id="0f939-130">说明</span><span class="sxs-lookup"><span data-stu-id="0f939-130">description</span></span>|<span data-ttu-id="0f939-131">字符串</span><span class="sxs-lookup"><span data-stu-id="0f939-131">String</span></span>|<span data-ttu-id="0f939-132">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="0f939-132">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="0f939-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0f939-133">displayName</span></span>|<span data-ttu-id="0f939-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0f939-134">String</span></span>|<span data-ttu-id="0f939-135">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="0f939-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="0f939-136">版本</span><span class="sxs-lookup"><span data-stu-id="0f939-136">version</span></span>|<span data-ttu-id="0f939-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0f939-137">Int32</span></span>|<span data-ttu-id="0f939-138">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0f939-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f939-139">关系</span><span class="sxs-lookup"><span data-stu-id="0f939-139">Relationships</span></span>
|<span data-ttu-id="0f939-140">关系</span><span class="sxs-lookup"><span data-stu-id="0f939-140">Relationship</span></span>|<span data-ttu-id="0f939-141">类型</span><span class="sxs-lookup"><span data-stu-id="0f939-141">Type</span></span>|<span data-ttu-id="0f939-142">说明</span><span class="sxs-lookup"><span data-stu-id="0f939-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f939-143">分配</span><span class="sxs-lookup"><span data-stu-id="0f939-143">assignments</span></span>|<span data-ttu-id="0f939-144">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f939-144">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0f939-145">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0f939-145">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="0f939-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0f939-146">deviceStatuses</span></span>|<span data-ttu-id="0f939-147">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f939-147">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0f939-148">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0f939-148">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="0f939-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0f939-149">userStatuses</span></span>|<span data-ttu-id="0f939-150">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f939-150">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0f939-151">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0f939-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="0f939-152">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0f939-152">deviceStatusOverview</span></span>|[<span data-ttu-id="0f939-153">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0f939-153">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0f939-154">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="0f939-154">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="0f939-155">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0f939-155">userStatusOverview</span></span>|[<span data-ttu-id="0f939-156">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0f939-156">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="0f939-157">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="0f939-157">Device Configuration users status overview</span></span>|
|<span data-ttu-id="0f939-158">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0f939-158">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0f939-159">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f939-159">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0f939-160">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="0f939-160">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f939-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f939-161">JSON Representation</span></span>
<span data-ttu-id="0f939-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f939-162">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```








