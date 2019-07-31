---
title: deviceConfiguration 资源类型
description: 设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b9bc0bc5c2c589a1eaf1bceb989c981806d553f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001682"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="c9b4f-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9b4f-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="c9b4f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9b4f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b4f-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c9b4f-107">方法</span><span class="sxs-lookup"><span data-stu-id="c9b4f-107">Methods</span></span>
|<span data-ttu-id="c9b4f-108">方法</span><span class="sxs-lookup"><span data-stu-id="c9b4f-108">Method</span></span>|<span data-ttu-id="c9b4f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9b4f-109">Return Type</span></span>|<span data-ttu-id="c9b4f-110">说明</span><span class="sxs-lookup"><span data-stu-id="c9b4f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9b4f-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="c9b4f-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="c9b4f-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="c9b4f-113">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c9b4f-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9b4f-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="c9b4f-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9b4f-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="c9b4f-116">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c9b4f-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="c9b4f-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="c9b4f-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c9b4f-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9b4f-119">Not yet documented</span></span>|
|[<span data-ttu-id="c9b4f-120">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="c9b4f-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="c9b4f-121">无</span><span class="sxs-lookup"><span data-stu-id="c9b4f-121">None</span></span>|<span data-ttu-id="c9b4f-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9b4f-122">Not yet documented</span></span>|
|[<span data-ttu-id="c9b4f-123">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="c9b4f-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="c9b4f-124">无</span><span class="sxs-lookup"><span data-stu-id="c9b4f-124">None</span></span>|<span data-ttu-id="c9b4f-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9b4f-125">Not yet documented</span></span>|
|[<span data-ttu-id="c9b4f-126">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="c9b4f-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="c9b4f-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="c9b4f-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9b4f-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c9b4f-129">属性</span><span class="sxs-lookup"><span data-stu-id="c9b4f-129">Properties</span></span>
|<span data-ttu-id="c9b4f-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9b4f-130">Property</span></span>|<span data-ttu-id="c9b4f-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9b4f-131">Type</span></span>|<span data-ttu-id="c9b4f-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9b4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b4f-133">id</span><span class="sxs-lookup"><span data-stu-id="c9b4f-133">id</span></span>|<span data-ttu-id="c9b4f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c9b4f-134">String</span></span>|<span data-ttu-id="c9b4f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-135">Key of the entity.</span></span>|
|<span data-ttu-id="c9b4f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9b4f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9b4f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9b4f-137">DateTimeOffset</span></span>|<span data-ttu-id="c9b4f-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c9b4f-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9b4f-139">roleScopeTagIds</span></span>|<span data-ttu-id="c9b4f-140">String collection</span><span class="sxs-lookup"><span data-stu-id="c9b4f-140">String collection</span></span>|<span data-ttu-id="c9b4f-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="c9b4f-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9b4f-142">supportsScopeTags</span></span>|<span data-ttu-id="c9b4f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b4f-143">Boolean</span></span>|<span data-ttu-id="c9b4f-144">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9b4f-145">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9b4f-146">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9b4f-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-147">This property is read-only.</span></span>|
|<span data-ttu-id="c9b4f-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9b4f-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c9b4f-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9b4f-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c9b4f-150">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="c9b4f-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9b4f-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c9b4f-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9b4f-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c9b4f-153">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="c9b4f-154">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c9b4f-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c9b4f-155">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c9b4f-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c9b4f-156">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="c9b4f-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9b4f-157">createdDateTime</span></span>|<span data-ttu-id="c9b4f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9b4f-158">DateTimeOffset</span></span>|<span data-ttu-id="c9b4f-159">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="c9b4f-160">说明</span><span class="sxs-lookup"><span data-stu-id="c9b4f-160">description</span></span>|<span data-ttu-id="c9b4f-161">String</span><span class="sxs-lookup"><span data-stu-id="c9b4f-161">String</span></span>|<span data-ttu-id="c9b4f-162">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c9b4f-163">displayName</span><span class="sxs-lookup"><span data-stu-id="c9b4f-163">displayName</span></span>|<span data-ttu-id="c9b4f-164">String</span><span class="sxs-lookup"><span data-stu-id="c9b4f-164">String</span></span>|<span data-ttu-id="c9b4f-165">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c9b4f-166">version</span><span class="sxs-lookup"><span data-stu-id="c9b4f-166">version</span></span>|<span data-ttu-id="c9b4f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b4f-167">Int32</span></span>|<span data-ttu-id="c9b4f-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9b4f-169">关系</span><span class="sxs-lookup"><span data-stu-id="c9b4f-169">Relationships</span></span>
|<span data-ttu-id="c9b4f-170">关系</span><span class="sxs-lookup"><span data-stu-id="c9b4f-170">Relationship</span></span>|<span data-ttu-id="c9b4f-171">类型</span><span class="sxs-lookup"><span data-stu-id="c9b4f-171">Type</span></span>|<span data-ttu-id="c9b4f-172">说明</span><span class="sxs-lookup"><span data-stu-id="c9b4f-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b4f-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c9b4f-173">groupAssignments</span></span>|<span data-ttu-id="c9b4f-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="c9b4f-175">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="c9b4f-176">assignments</span><span class="sxs-lookup"><span data-stu-id="c9b4f-176">assignments</span></span>|<span data-ttu-id="c9b4f-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c9b4f-178">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="c9b4f-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c9b4f-179">deviceStatuses</span></span>|<span data-ttu-id="c9b4f-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c9b4f-181">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="c9b4f-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c9b4f-182">userStatuses</span></span>|<span data-ttu-id="c9b4f-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c9b4f-184">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="c9b4f-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c9b4f-185">deviceStatusOverview</span></span>|[<span data-ttu-id="c9b4f-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c9b4f-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c9b4f-187">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="c9b4f-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="c9b4f-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c9b4f-188">userStatusOverview</span></span>|[<span data-ttu-id="c9b4f-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c9b4f-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c9b4f-190">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="c9b4f-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="c9b4f-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c9b4f-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c9b4f-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9b4f-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c9b4f-193">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="c9b4f-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9b4f-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9b4f-194">JSON Representation</span></span>
<span data-ttu-id="c9b4f-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9b4f-195">Here is a JSON representation of the resource.</span></span>
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





