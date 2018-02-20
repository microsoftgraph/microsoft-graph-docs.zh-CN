# <a name="devicemanagement-resource-type"></a><span data-ttu-id="dfc6e-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfc6e-101">deviceManagement resource type</span></span>

> <span data-ttu-id="dfc6e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfc6e-103">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="dfc6e-104">方法</span><span class="sxs-lookup"><span data-stu-id="dfc6e-104">Methods</span></span>
|<span data-ttu-id="dfc6e-105">方法</span><span class="sxs-lookup"><span data-stu-id="dfc6e-105">Method</span></span>|<span data-ttu-id="dfc6e-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfc6e-106">Return Type</span></span>|<span data-ttu-id="dfc6e-107">说明</span><span class="sxs-lookup"><span data-stu-id="dfc6e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dfc6e-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="dfc6e-108">Get deviceManagement</span></span>](../api/intune_deviceconfig_devicemanagement_get.md)|[<span data-ttu-id="dfc6e-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="dfc6e-109">deviceManagement</span></span>](../resources/intune_deviceconfig_devicemanagement.md)|<span data-ttu-id="dfc6e-110">读取 [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="dfc6e-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="dfc6e-111">Update deviceManagement</span></span>](../api/intune_deviceconfig_devicemanagement_update.md)|[<span data-ttu-id="dfc6e-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="dfc6e-112">deviceManagement</span></span>](../resources/intune_deviceconfig_devicemanagement.md)|<span data-ttu-id="dfc6e-113">更新 [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-113">Update the properties of a [calendar](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfc6e-114">属性</span><span class="sxs-lookup"><span data-stu-id="dfc6e-114">Properties</span></span>
|<span data-ttu-id="dfc6e-115">属性</span><span class="sxs-lookup"><span data-stu-id="dfc6e-115">Property</span></span>|<span data-ttu-id="dfc6e-116">类型</span><span class="sxs-lookup"><span data-stu-id="dfc6e-116">Type</span></span>|<span data-ttu-id="dfc6e-117">说明</span><span class="sxs-lookup"><span data-stu-id="dfc6e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfc6e-118">id</span><span class="sxs-lookup"><span data-stu-id="dfc6e-118">id</span></span>|<span data-ttu-id="dfc6e-119">String</span><span class="sxs-lookup"><span data-stu-id="dfc6e-119">String</span></span>|<span data-ttu-id="dfc6e-120">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="dfc6e-120">Unique Identifier</span></span>|
|<span data-ttu-id="dfc6e-121">settings</span><span class="sxs-lookup"><span data-stu-id="dfc6e-121">settings</span></span>|[<span data-ttu-id="dfc6e-122">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="dfc6e-122">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="dfc6e-123">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-123">Account level settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfc6e-124">关系</span><span class="sxs-lookup"><span data-stu-id="dfc6e-124">Relationships</span></span>
|<span data-ttu-id="dfc6e-125">关系</span><span class="sxs-lookup"><span data-stu-id="dfc6e-125">Relationship</span></span>|<span data-ttu-id="dfc6e-126">类型</span><span class="sxs-lookup"><span data-stu-id="dfc6e-126">Type</span></span>|<span data-ttu-id="dfc6e-127">说明</span><span class="sxs-lookup"><span data-stu-id="dfc6e-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfc6e-128">deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="dfc6e-128">deviceConfigurations</span></span>|<span data-ttu-id="dfc6e-129">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfc6e-129">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) collection</span></span>|<span data-ttu-id="dfc6e-130">设备配置。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-130">The device configurations.</span></span>|
|<span data-ttu-id="dfc6e-131">deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="dfc6e-131">deviceCompliancePolicies</span></span>|<span data-ttu-id="dfc6e-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfc6e-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="dfc6e-133">设备符合性策略。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-133">The device compliance policies.</span></span>|
|<span data-ttu-id="dfc6e-134">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dfc6e-134">softwareUpdateStatusSummary</span></span>|[<span data-ttu-id="dfc6e-135">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dfc6e-135">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="dfc6e-136">软件更新状态摘要。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-136">The software update status summary.</span></span>|
|<span data-ttu-id="dfc6e-137">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="dfc6e-137">deviceCompliancePolicyDeviceStateSummary</span></span>|[<span data-ttu-id="dfc6e-138">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="dfc6e-138">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="dfc6e-139">此帐户的设备符合性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-139">The device compliance state summary for this account.</span></span>|
|<span data-ttu-id="dfc6e-140">deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="dfc6e-140">deviceCompliancePolicySettingStateSummaries</span></span>|<span data-ttu-id="dfc6e-141">[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfc6e-141">[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="dfc6e-142">此帐户的符合性设置的摘要状态。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-142">The summary states of compliance policy settings for this account.</span></span>|
|<span data-ttu-id="dfc6e-143">deviceConfigurationDeviceStateSummaries</span><span class="sxs-lookup"><span data-stu-id="dfc6e-143">deviceConfigurationDeviceStateSummaries</span></span>|[<span data-ttu-id="dfc6e-144">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="dfc6e-144">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="dfc6e-145">此帐户的设备配置设备状态摘要。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-145">The device configuration device state summary for this account.</span></span>|
|<span data-ttu-id="dfc6e-146">iosUpdateStatuses</span><span class="sxs-lookup"><span data-stu-id="dfc6e-146">iosUpdateStatuses</span></span>|<span data-ttu-id="dfc6e-147">[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfc6e-147">[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) collection</span></span>|<span data-ttu-id="dfc6e-148">此帐户的 IOS 软件更新安装状态。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-148">The IOS software update installation statuses for this account.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfc6e-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfc6e-149">JSON Representation</span></span>
<span data-ttu-id="dfc6e-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfc6e-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



