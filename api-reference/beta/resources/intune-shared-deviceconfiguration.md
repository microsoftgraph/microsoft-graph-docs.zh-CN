---
title: deviceConfiguration 资源类型
description: 设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5a82af9a6d5de359891498b32489a899e3b8f82
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306889"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="90cee-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="90cee-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="90cee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90cee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90cee-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90cee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90cee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90cee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90cee-107">设备配置。</span><span class="sxs-lookup"><span data-stu-id="90cee-107">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="90cee-108">Methods</span><span class="sxs-lookup"><span data-stu-id="90cee-108">Methods</span></span>
|<span data-ttu-id="90cee-109">方法</span><span class="sxs-lookup"><span data-stu-id="90cee-109">Method</span></span>|<span data-ttu-id="90cee-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="90cee-110">Return Type</span></span>|<span data-ttu-id="90cee-111">Description</span><span class="sxs-lookup"><span data-stu-id="90cee-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90cee-112">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="90cee-112">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="90cee-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="90cee-114">列出 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90cee-114">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="90cee-115">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="90cee-115">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="90cee-116">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="90cee-116">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="90cee-117">读取 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90cee-117">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="90cee-118">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="90cee-118">**Device configuration**</span></span>|
|[<span data-ttu-id="90cee-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="90cee-119">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="90cee-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="90cee-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="90cee-121">Not yet documented</span></span>|
|[<span data-ttu-id="90cee-122">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="90cee-122">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="90cee-123">无</span><span class="sxs-lookup"><span data-stu-id="90cee-123">None</span></span>|<span data-ttu-id="90cee-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="90cee-124">Not yet documented</span></span>|
|[<span data-ttu-id="90cee-125">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="90cee-125">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="90cee-126">无</span><span class="sxs-lookup"><span data-stu-id="90cee-126">None</span></span>|<span data-ttu-id="90cee-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="90cee-127">Not yet documented</span></span>|
|[<span data-ttu-id="90cee-128">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="90cee-128">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="90cee-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="90cee-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="90cee-130">Not yet documented</span></span>|
|<span data-ttu-id="90cee-131">**策略集**</span><span class="sxs-lookup"><span data-stu-id="90cee-131">**Policy Set**</span></span>|
|[<span data-ttu-id="90cee-132">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="90cee-132">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="90cee-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="90cee-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="90cee-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="90cee-135">属性</span><span class="sxs-lookup"><span data-stu-id="90cee-135">Properties</span></span>
|<span data-ttu-id="90cee-136">属性</span><span class="sxs-lookup"><span data-stu-id="90cee-136">Property</span></span>|<span data-ttu-id="90cee-137">类型</span><span class="sxs-lookup"><span data-stu-id="90cee-137">Type</span></span>|<span data-ttu-id="90cee-138">说明</span><span class="sxs-lookup"><span data-stu-id="90cee-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90cee-139">id</span><span class="sxs-lookup"><span data-stu-id="90cee-139">id</span></span>|<span data-ttu-id="90cee-140">字符串</span><span class="sxs-lookup"><span data-stu-id="90cee-140">String</span></span>|<span data-ttu-id="90cee-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="90cee-141">Key of the entity.</span></span>|
|<span data-ttu-id="90cee-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90cee-142">lastModifiedDateTime</span></span>|<span data-ttu-id="90cee-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90cee-143">DateTimeOffset</span></span>|<span data-ttu-id="90cee-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90cee-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="90cee-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90cee-145">roleScopeTagIds</span></span>|<span data-ttu-id="90cee-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-146">String collection</span></span>|<span data-ttu-id="90cee-147">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="90cee-147">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="90cee-148">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="90cee-148">supportsScopeTags</span></span>|<span data-ttu-id="90cee-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cee-149">Boolean</span></span>|<span data-ttu-id="90cee-150">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="90cee-150">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="90cee-151">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="90cee-151">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="90cee-152">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="90cee-152">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="90cee-153">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="90cee-153">This property is read-only.</span></span>|
|<span data-ttu-id="90cee-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90cee-154">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="90cee-155">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90cee-155">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="90cee-156">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="90cee-156">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="90cee-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90cee-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="90cee-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90cee-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="90cee-159">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="90cee-159">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="90cee-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90cee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="90cee-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90cee-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="90cee-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="90cee-162">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="90cee-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90cee-163">createdDateTime</span></span>|<span data-ttu-id="90cee-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90cee-164">DateTimeOffset</span></span>|<span data-ttu-id="90cee-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90cee-165">DateTime the object was created.</span></span>|
|<span data-ttu-id="90cee-166">description</span><span class="sxs-lookup"><span data-stu-id="90cee-166">description</span></span>|<span data-ttu-id="90cee-167">字符串</span><span class="sxs-lookup"><span data-stu-id="90cee-167">String</span></span>|<span data-ttu-id="90cee-168">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="90cee-168">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="90cee-169">displayName</span><span class="sxs-lookup"><span data-stu-id="90cee-169">displayName</span></span>|<span data-ttu-id="90cee-170">字符串</span><span class="sxs-lookup"><span data-stu-id="90cee-170">String</span></span>|<span data-ttu-id="90cee-171">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="90cee-171">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="90cee-172">version</span><span class="sxs-lookup"><span data-stu-id="90cee-172">version</span></span>|<span data-ttu-id="90cee-173">Int32</span><span class="sxs-lookup"><span data-stu-id="90cee-173">Int32</span></span>|<span data-ttu-id="90cee-174">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="90cee-174">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90cee-175">关系</span><span class="sxs-lookup"><span data-stu-id="90cee-175">Relationships</span></span>
|<span data-ttu-id="90cee-176">关系</span><span class="sxs-lookup"><span data-stu-id="90cee-176">Relationship</span></span>|<span data-ttu-id="90cee-177">类型</span><span class="sxs-lookup"><span data-stu-id="90cee-177">Type</span></span>|<span data-ttu-id="90cee-178">Description</span><span class="sxs-lookup"><span data-stu-id="90cee-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90cee-179">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="90cee-179">**Device configuration**</span></span>|
|<span data-ttu-id="90cee-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="90cee-180">groupAssignments</span></span>|<span data-ttu-id="90cee-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="90cee-182">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="90cee-182">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="90cee-183">assignments</span><span class="sxs-lookup"><span data-stu-id="90cee-183">assignments</span></span>|<span data-ttu-id="90cee-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="90cee-185">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="90cee-185">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="90cee-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="90cee-186">deviceStatuses</span></span>|<span data-ttu-id="90cee-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="90cee-188">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="90cee-188">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="90cee-189">userStatuses</span><span class="sxs-lookup"><span data-stu-id="90cee-189">userStatuses</span></span>|<span data-ttu-id="90cee-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="90cee-191">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="90cee-191">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="90cee-192">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="90cee-192">deviceStatusOverview</span></span>|[<span data-ttu-id="90cee-193">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="90cee-193">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="90cee-194">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="90cee-194">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="90cee-195">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="90cee-195">userStatusOverview</span></span>|[<span data-ttu-id="90cee-196">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="90cee-196">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="90cee-197">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="90cee-197">Device Configuration users status overview</span></span>|
|<span data-ttu-id="90cee-198">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="90cee-198">deviceSettingStateSummaries</span></span>|<span data-ttu-id="90cee-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90cee-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="90cee-200">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="90cee-200">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90cee-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90cee-201">JSON Representation</span></span>
<span data-ttu-id="90cee-202">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90cee-202">Here is a JSON representation of the resource.</span></span>
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




