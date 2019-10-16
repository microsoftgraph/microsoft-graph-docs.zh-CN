---
title: deviceConfiguration 资源类型
description: 设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68204c747aa983ed44cf2c30fb056baaa7de7225
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539146"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="f6185-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6185-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="f6185-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6185-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6185-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6185-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6185-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="f6185-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="f6185-107">方法</span><span class="sxs-lookup"><span data-stu-id="f6185-107">Methods</span></span>
|<span data-ttu-id="f6185-108">方法</span><span class="sxs-lookup"><span data-stu-id="f6185-108">Method</span></span>|<span data-ttu-id="f6185-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6185-109">Return Type</span></span>|<span data-ttu-id="f6185-110">说明</span><span class="sxs-lookup"><span data-stu-id="f6185-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6185-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="f6185-111">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="f6185-112">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-112">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="f6185-113">列出 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f6185-113">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f6185-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f6185-114">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="f6185-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f6185-115">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="f6185-116">读取 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f6185-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="f6185-117">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="f6185-117">**Device configuration**</span></span>|
|[<span data-ttu-id="f6185-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="f6185-118">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="f6185-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f6185-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6185-120">Not yet documented</span></span>|
|[<span data-ttu-id="f6185-121">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="f6185-121">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="f6185-122">无</span><span class="sxs-lookup"><span data-stu-id="f6185-122">None</span></span>|<span data-ttu-id="f6185-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6185-123">Not yet documented</span></span>|
|[<span data-ttu-id="f6185-124">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="f6185-124">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="f6185-125">无</span><span class="sxs-lookup"><span data-stu-id="f6185-125">None</span></span>|<span data-ttu-id="f6185-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6185-126">Not yet documented</span></span>|
|[<span data-ttu-id="f6185-127">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="f6185-127">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="f6185-128">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6185-128">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="f6185-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6185-129">Not yet documented</span></span>|
|<span data-ttu-id="f6185-130">**策略集**</span><span class="sxs-lookup"><span data-stu-id="f6185-130">**Policy Set**</span></span>|
|[<span data-ttu-id="f6185-131">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="f6185-131">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="f6185-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6185-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="f6185-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6185-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f6185-134">属性</span><span class="sxs-lookup"><span data-stu-id="f6185-134">Properties</span></span>
|<span data-ttu-id="f6185-135">属性</span><span class="sxs-lookup"><span data-stu-id="f6185-135">Property</span></span>|<span data-ttu-id="f6185-136">类型</span><span class="sxs-lookup"><span data-stu-id="f6185-136">Type</span></span>|<span data-ttu-id="f6185-137">说明</span><span class="sxs-lookup"><span data-stu-id="f6185-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6185-138">id</span><span class="sxs-lookup"><span data-stu-id="f6185-138">id</span></span>|<span data-ttu-id="f6185-139">字符串</span><span class="sxs-lookup"><span data-stu-id="f6185-139">String</span></span>|<span data-ttu-id="f6185-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f6185-140">Key of the entity.</span></span>|
|<span data-ttu-id="f6185-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6185-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f6185-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6185-142">DateTimeOffset</span></span>|<span data-ttu-id="f6185-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6185-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f6185-144">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6185-144">roleScopeTagIds</span></span>|<span data-ttu-id="f6185-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-145">String collection</span></span>|<span data-ttu-id="f6185-146">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f6185-146">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="f6185-147">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f6185-147">supportsScopeTags</span></span>|<span data-ttu-id="f6185-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6185-148">Boolean</span></span>|<span data-ttu-id="f6185-149">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f6185-149">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f6185-150">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f6185-150">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f6185-151">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f6185-151">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f6185-152">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f6185-152">This property is read-only.</span></span>|
|<span data-ttu-id="f6185-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6185-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f6185-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6185-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f6185-155">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f6185-155">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="f6185-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6185-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f6185-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6185-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f6185-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f6185-158">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="f6185-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f6185-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f6185-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f6185-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f6185-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f6185-161">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="f6185-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6185-162">createdDateTime</span></span>|<span data-ttu-id="f6185-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6185-163">DateTimeOffset</span></span>|<span data-ttu-id="f6185-164">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6185-164">DateTime the object was created.</span></span>|
|<span data-ttu-id="f6185-165">说明</span><span class="sxs-lookup"><span data-stu-id="f6185-165">description</span></span>|<span data-ttu-id="f6185-166">String</span><span class="sxs-lookup"><span data-stu-id="f6185-166">String</span></span>|<span data-ttu-id="f6185-167">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="f6185-167">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="f6185-168">displayName</span><span class="sxs-lookup"><span data-stu-id="f6185-168">displayName</span></span>|<span data-ttu-id="f6185-169">String</span><span class="sxs-lookup"><span data-stu-id="f6185-169">String</span></span>|<span data-ttu-id="f6185-170">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="f6185-170">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="f6185-171">version</span><span class="sxs-lookup"><span data-stu-id="f6185-171">version</span></span>|<span data-ttu-id="f6185-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f6185-172">Int32</span></span>|<span data-ttu-id="f6185-173">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f6185-173">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6185-174">关系</span><span class="sxs-lookup"><span data-stu-id="f6185-174">Relationships</span></span>
|<span data-ttu-id="f6185-175">关系</span><span class="sxs-lookup"><span data-stu-id="f6185-175">Relationship</span></span>|<span data-ttu-id="f6185-176">类型</span><span class="sxs-lookup"><span data-stu-id="f6185-176">Type</span></span>|<span data-ttu-id="f6185-177">说明</span><span class="sxs-lookup"><span data-stu-id="f6185-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6185-178">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="f6185-178">**Device configuration**</span></span>|
|<span data-ttu-id="f6185-179">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="f6185-179">groupAssignments</span></span>|<span data-ttu-id="f6185-180">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6185-180">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="f6185-181">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="f6185-181">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="f6185-182">assignments</span><span class="sxs-lookup"><span data-stu-id="f6185-182">assignments</span></span>|<span data-ttu-id="f6185-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f6185-184">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="f6185-184">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="f6185-185">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f6185-185">deviceStatuses</span></span>|<span data-ttu-id="f6185-186">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-186">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="f6185-187">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="f6185-187">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="f6185-188">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f6185-188">userStatuses</span></span>|<span data-ttu-id="f6185-189">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-189">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="f6185-190">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="f6185-190">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="f6185-191">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f6185-191">deviceStatusOverview</span></span>|[<span data-ttu-id="f6185-192">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f6185-192">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="f6185-193">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="f6185-193">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="f6185-194">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f6185-194">userStatusOverview</span></span>|[<span data-ttu-id="f6185-195">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f6185-195">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="f6185-196">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="f6185-196">Device Configuration users status overview</span></span>|
|<span data-ttu-id="f6185-197">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f6185-197">deviceSettingStateSummaries</span></span>|<span data-ttu-id="f6185-198">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6185-198">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="f6185-199">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="f6185-199">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6185-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6185-200">JSON Representation</span></span>
<span data-ttu-id="f6185-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6185-201">Here is a JSON representation of the resource.</span></span>
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



