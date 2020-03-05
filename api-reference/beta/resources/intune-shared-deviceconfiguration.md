---
title: deviceConfiguration 资源类型
description: 设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c38a3b33368d4359ebfca42b83a52e795826643
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523721"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="eed31-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="eed31-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="eed31-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eed31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eed31-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eed31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eed31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eed31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eed31-107">设备配置。</span><span class="sxs-lookup"><span data-stu-id="eed31-107">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="eed31-108">方法</span><span class="sxs-lookup"><span data-stu-id="eed31-108">Methods</span></span>
|<span data-ttu-id="eed31-109">方法</span><span class="sxs-lookup"><span data-stu-id="eed31-109">Method</span></span>|<span data-ttu-id="eed31-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="eed31-110">Return Type</span></span>|<span data-ttu-id="eed31-111">说明</span><span class="sxs-lookup"><span data-stu-id="eed31-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eed31-112">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="eed31-112">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="eed31-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="eed31-114">列出 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eed31-114">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="eed31-115">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="eed31-115">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="eed31-116">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="eed31-116">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="eed31-117">读取 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eed31-117">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="eed31-118">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="eed31-118">**Device configuration**</span></span>|
|[<span data-ttu-id="eed31-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="eed31-119">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="eed31-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="eed31-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eed31-121">Not yet documented</span></span>|
|[<span data-ttu-id="eed31-122">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="eed31-122">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="eed31-123">无</span><span class="sxs-lookup"><span data-stu-id="eed31-123">None</span></span>|<span data-ttu-id="eed31-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eed31-124">Not yet documented</span></span>|
|[<span data-ttu-id="eed31-125">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="eed31-125">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="eed31-126">无</span><span class="sxs-lookup"><span data-stu-id="eed31-126">None</span></span>|<span data-ttu-id="eed31-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eed31-127">Not yet documented</span></span>|
|[<span data-ttu-id="eed31-128">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="eed31-128">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="eed31-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)集合</span><span class="sxs-lookup"><span data-stu-id="eed31-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="eed31-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eed31-130">Not yet documented</span></span>|
|<span data-ttu-id="eed31-131">**策略集**</span><span class="sxs-lookup"><span data-stu-id="eed31-131">**Policy Set**</span></span>|
|[<span data-ttu-id="eed31-132">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="eed31-132">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="eed31-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="eed31-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="eed31-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eed31-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="eed31-135">属性</span><span class="sxs-lookup"><span data-stu-id="eed31-135">Properties</span></span>
|<span data-ttu-id="eed31-136">属性</span><span class="sxs-lookup"><span data-stu-id="eed31-136">Property</span></span>|<span data-ttu-id="eed31-137">类型</span><span class="sxs-lookup"><span data-stu-id="eed31-137">Type</span></span>|<span data-ttu-id="eed31-138">说明</span><span class="sxs-lookup"><span data-stu-id="eed31-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed31-139">id</span><span class="sxs-lookup"><span data-stu-id="eed31-139">id</span></span>|<span data-ttu-id="eed31-140">字符串</span><span class="sxs-lookup"><span data-stu-id="eed31-140">String</span></span>|<span data-ttu-id="eed31-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eed31-141">Key of the entity.</span></span>|
|<span data-ttu-id="eed31-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eed31-142">lastModifiedDateTime</span></span>|<span data-ttu-id="eed31-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eed31-143">DateTimeOffset</span></span>|<span data-ttu-id="eed31-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eed31-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="eed31-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eed31-145">roleScopeTagIds</span></span>|<span data-ttu-id="eed31-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-146">String collection</span></span>|<span data-ttu-id="eed31-147">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="eed31-147">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="eed31-148">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eed31-148">supportsScopeTags</span></span>|<span data-ttu-id="eed31-149">布尔</span><span class="sxs-lookup"><span data-stu-id="eed31-149">Boolean</span></span>|<span data-ttu-id="eed31-150">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="eed31-150">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eed31-151">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="eed31-151">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eed31-152">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="eed31-152">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eed31-153">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="eed31-153">This property is read-only.</span></span>|
|<span data-ttu-id="eed31-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="eed31-154">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="eed31-155">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="eed31-155">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="eed31-156">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="eed31-156">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="eed31-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="eed31-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="eed31-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="eed31-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="eed31-159">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="eed31-159">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="eed31-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="eed31-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="eed31-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="eed31-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="eed31-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="eed31-162">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="eed31-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eed31-163">createdDateTime</span></span>|<span data-ttu-id="eed31-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eed31-164">DateTimeOffset</span></span>|<span data-ttu-id="eed31-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eed31-165">DateTime the object was created.</span></span>|
|<span data-ttu-id="eed31-166">说明</span><span class="sxs-lookup"><span data-stu-id="eed31-166">description</span></span>|<span data-ttu-id="eed31-167">String</span><span class="sxs-lookup"><span data-stu-id="eed31-167">String</span></span>|<span data-ttu-id="eed31-168">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="eed31-168">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="eed31-169">displayName</span><span class="sxs-lookup"><span data-stu-id="eed31-169">displayName</span></span>|<span data-ttu-id="eed31-170">String</span><span class="sxs-lookup"><span data-stu-id="eed31-170">String</span></span>|<span data-ttu-id="eed31-171">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="eed31-171">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="eed31-172">version</span><span class="sxs-lookup"><span data-stu-id="eed31-172">version</span></span>|<span data-ttu-id="eed31-173">Int32</span><span class="sxs-lookup"><span data-stu-id="eed31-173">Int32</span></span>|<span data-ttu-id="eed31-174">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="eed31-174">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eed31-175">关系</span><span class="sxs-lookup"><span data-stu-id="eed31-175">Relationships</span></span>
|<span data-ttu-id="eed31-176">关系</span><span class="sxs-lookup"><span data-stu-id="eed31-176">Relationship</span></span>|<span data-ttu-id="eed31-177">类型</span><span class="sxs-lookup"><span data-stu-id="eed31-177">Type</span></span>|<span data-ttu-id="eed31-178">说明</span><span class="sxs-lookup"><span data-stu-id="eed31-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed31-179">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="eed31-179">**Device configuration**</span></span>|
|<span data-ttu-id="eed31-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="eed31-180">groupAssignments</span></span>|<span data-ttu-id="eed31-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="eed31-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="eed31-182">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="eed31-182">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="eed31-183">assignments</span><span class="sxs-lookup"><span data-stu-id="eed31-183">assignments</span></span>|<span data-ttu-id="eed31-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="eed31-185">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="eed31-185">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="eed31-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="eed31-186">deviceStatuses</span></span>|<span data-ttu-id="eed31-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="eed31-188">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="eed31-188">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="eed31-189">userStatuses</span><span class="sxs-lookup"><span data-stu-id="eed31-189">userStatuses</span></span>|<span data-ttu-id="eed31-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="eed31-191">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="eed31-191">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="eed31-192">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="eed31-192">deviceStatusOverview</span></span>|[<span data-ttu-id="eed31-193">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="eed31-193">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="eed31-194">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="eed31-194">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="eed31-195">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="eed31-195">userStatusOverview</span></span>|[<span data-ttu-id="eed31-196">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="eed31-196">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="eed31-197">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="eed31-197">Device Configuration users status overview</span></span>|
|<span data-ttu-id="eed31-198">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="eed31-198">deviceSettingStateSummaries</span></span>|<span data-ttu-id="eed31-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed31-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="eed31-200">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="eed31-200">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eed31-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eed31-201">JSON Representation</span></span>
<span data-ttu-id="eed31-202">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eed31-202">Here is a JSON representation of the resource.</span></span>
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



