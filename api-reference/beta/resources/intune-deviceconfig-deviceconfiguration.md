---
title: deviceConfiguration 资源类型
description: 设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 980ec0e08ff43cd5b364801b3eca732bcb810188
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995964"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="45044-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="45044-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="45044-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="45044-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45044-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45044-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45044-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="45044-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="45044-107">方法</span><span class="sxs-lookup"><span data-stu-id="45044-107">Methods</span></span>
|<span data-ttu-id="45044-108">方法</span><span class="sxs-lookup"><span data-stu-id="45044-108">Method</span></span>|<span data-ttu-id="45044-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="45044-109">Return Type</span></span>|<span data-ttu-id="45044-110">说明</span><span class="sxs-lookup"><span data-stu-id="45044-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45044-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="45044-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="45044-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45044-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="45044-113">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="45044-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="45044-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="45044-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="45044-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="45044-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="45044-116">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="45044-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="45044-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="45044-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="45044-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45044-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="45044-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45044-119">Not yet documented</span></span>|
|[<span data-ttu-id="45044-120">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="45044-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="45044-121">无</span><span class="sxs-lookup"><span data-stu-id="45044-121">None</span></span>|<span data-ttu-id="45044-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45044-122">Not yet documented</span></span>|
|[<span data-ttu-id="45044-123">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="45044-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="45044-124">无</span><span class="sxs-lookup"><span data-stu-id="45044-124">None</span></span>|<span data-ttu-id="45044-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45044-125">Not yet documented</span></span>|
|[<span data-ttu-id="45044-126">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="45044-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="45044-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)集合</span><span class="sxs-lookup"><span data-stu-id="45044-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="45044-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45044-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="45044-129">属性</span><span class="sxs-lookup"><span data-stu-id="45044-129">Properties</span></span>
|<span data-ttu-id="45044-130">属性</span><span class="sxs-lookup"><span data-stu-id="45044-130">Property</span></span>|<span data-ttu-id="45044-131">类型</span><span class="sxs-lookup"><span data-stu-id="45044-131">Type</span></span>|<span data-ttu-id="45044-132">说明</span><span class="sxs-lookup"><span data-stu-id="45044-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45044-133">id</span><span class="sxs-lookup"><span data-stu-id="45044-133">id</span></span>|<span data-ttu-id="45044-134">字符串</span><span class="sxs-lookup"><span data-stu-id="45044-134">String</span></span>|<span data-ttu-id="45044-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="45044-135">Key of the entity.</span></span>|
|<span data-ttu-id="45044-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45044-136">lastModifiedDateTime</span></span>|<span data-ttu-id="45044-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45044-137">DateTimeOffset</span></span>|<span data-ttu-id="45044-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="45044-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="45044-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45044-139">roleScopeTagIds</span></span>|<span data-ttu-id="45044-140">String collection</span><span class="sxs-lookup"><span data-stu-id="45044-140">String collection</span></span>|<span data-ttu-id="45044-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="45044-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="45044-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45044-142">supportsScopeTags</span></span>|<span data-ttu-id="45044-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="45044-143">Boolean</span></span>|<span data-ttu-id="45044-144">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="45044-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45044-145">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="45044-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45044-146">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="45044-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45044-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="45044-147">This property is read-only.</span></span>|
|<span data-ttu-id="45044-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45044-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="45044-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45044-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="45044-150">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="45044-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="45044-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45044-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="45044-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45044-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="45044-153">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="45044-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="45044-154">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45044-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="45044-155">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45044-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="45044-156">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="45044-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="45044-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45044-157">createdDateTime</span></span>|<span data-ttu-id="45044-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45044-158">DateTimeOffset</span></span>|<span data-ttu-id="45044-159">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="45044-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="45044-160">说明</span><span class="sxs-lookup"><span data-stu-id="45044-160">description</span></span>|<span data-ttu-id="45044-161">String</span><span class="sxs-lookup"><span data-stu-id="45044-161">String</span></span>|<span data-ttu-id="45044-162">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="45044-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="45044-163">displayName</span><span class="sxs-lookup"><span data-stu-id="45044-163">displayName</span></span>|<span data-ttu-id="45044-164">String</span><span class="sxs-lookup"><span data-stu-id="45044-164">String</span></span>|<span data-ttu-id="45044-165">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="45044-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="45044-166">version</span><span class="sxs-lookup"><span data-stu-id="45044-166">version</span></span>|<span data-ttu-id="45044-167">Int32</span><span class="sxs-lookup"><span data-stu-id="45044-167">Int32</span></span>|<span data-ttu-id="45044-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="45044-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45044-169">关系</span><span class="sxs-lookup"><span data-stu-id="45044-169">Relationships</span></span>
|<span data-ttu-id="45044-170">关系</span><span class="sxs-lookup"><span data-stu-id="45044-170">Relationship</span></span>|<span data-ttu-id="45044-171">类型</span><span class="sxs-lookup"><span data-stu-id="45044-171">Type</span></span>|<span data-ttu-id="45044-172">说明</span><span class="sxs-lookup"><span data-stu-id="45044-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45044-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="45044-173">groupAssignments</span></span>|<span data-ttu-id="45044-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="45044-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="45044-175">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="45044-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="45044-176">assignments</span><span class="sxs-lookup"><span data-stu-id="45044-176">assignments</span></span>|<span data-ttu-id="45044-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45044-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="45044-178">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="45044-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="45044-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="45044-179">deviceStatuses</span></span>|<span data-ttu-id="45044-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45044-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="45044-181">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="45044-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="45044-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="45044-182">userStatuses</span></span>|<span data-ttu-id="45044-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45044-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="45044-184">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="45044-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="45044-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="45044-185">deviceStatusOverview</span></span>|[<span data-ttu-id="45044-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="45044-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="45044-187">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="45044-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="45044-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="45044-188">userStatusOverview</span></span>|[<span data-ttu-id="45044-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="45044-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="45044-190">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="45044-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="45044-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="45044-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="45044-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45044-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="45044-193">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="45044-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45044-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45044-194">JSON Representation</span></span>
<span data-ttu-id="45044-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45044-195">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```





