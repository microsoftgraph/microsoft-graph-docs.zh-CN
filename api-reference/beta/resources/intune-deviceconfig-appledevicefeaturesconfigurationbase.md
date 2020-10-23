---
title: appleDeviceFeaturesConfigurationBase 资源类型
description: Apple 设备功能配置的配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 337718b5d4163fdc4011252999e415ed3a4477b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703900"
---
# <a name="appledevicefeaturesconfigurationbase-resource-type"></a><span data-ttu-id="89d21-103">appleDeviceFeaturesConfigurationBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="89d21-103">appleDeviceFeaturesConfigurationBase resource type</span></span>

<span data-ttu-id="89d21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89d21-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89d21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89d21-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89d21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d21-107">Apple 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="89d21-107">Apple device features configuration profile.</span></span>


<span data-ttu-id="89d21-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="89d21-109">Methods</span><span class="sxs-lookup"><span data-stu-id="89d21-109">Methods</span></span>
|<span data-ttu-id="89d21-110">方法</span><span class="sxs-lookup"><span data-stu-id="89d21-110">Method</span></span>|<span data-ttu-id="89d21-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="89d21-111">Return Type</span></span>|<span data-ttu-id="89d21-112">说明</span><span class="sxs-lookup"><span data-stu-id="89d21-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89d21-113">List appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="89d21-113">List appleDeviceFeaturesConfigurationBases</span></span>](../api/intune-deviceconfig-appledevicefeaturesconfigurationbase-list.md)|<span data-ttu-id="89d21-114">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-114">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) collection</span></span>|<span data-ttu-id="89d21-115">列出 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89d21-115">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>|
|[<span data-ttu-id="89d21-116">Get appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="89d21-116">Get appleDeviceFeaturesConfigurationBase</span></span>](../api/intune-deviceconfig-appledevicefeaturesconfigurationbase-get.md)|[<span data-ttu-id="89d21-117">appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="89d21-117">appleDeviceFeaturesConfigurationBase</span></span>](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|<span data-ttu-id="89d21-118">读取 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89d21-118">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89d21-119">属性</span><span class="sxs-lookup"><span data-stu-id="89d21-119">Properties</span></span>
|<span data-ttu-id="89d21-120">属性</span><span class="sxs-lookup"><span data-stu-id="89d21-120">Property</span></span>|<span data-ttu-id="89d21-121">类型</span><span class="sxs-lookup"><span data-stu-id="89d21-121">Type</span></span>|<span data-ttu-id="89d21-122">说明</span><span class="sxs-lookup"><span data-stu-id="89d21-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d21-123">id</span><span class="sxs-lookup"><span data-stu-id="89d21-123">id</span></span>|<span data-ttu-id="89d21-124">String</span><span class="sxs-lookup"><span data-stu-id="89d21-124">String</span></span>|<span data-ttu-id="89d21-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="89d21-125">Key of the entity.</span></span> <span data-ttu-id="89d21-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89d21-127">lastModifiedDateTime</span></span>|<span data-ttu-id="89d21-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d21-128">DateTimeOffset</span></span>|<span data-ttu-id="89d21-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="89d21-129">DateTime the object was last modified.</span></span> <span data-ttu-id="89d21-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89d21-131">roleScopeTagIds</span></span>|<span data-ttu-id="89d21-132">String collection</span><span class="sxs-lookup"><span data-stu-id="89d21-132">String collection</span></span>|<span data-ttu-id="89d21-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="89d21-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89d21-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="89d21-135">supportsScopeTags</span></span>|<span data-ttu-id="89d21-136">布尔</span><span class="sxs-lookup"><span data-stu-id="89d21-136">Boolean</span></span>|<span data-ttu-id="89d21-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="89d21-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89d21-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="89d21-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89d21-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="89d21-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89d21-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="89d21-140">This property is read-only.</span></span> <span data-ttu-id="89d21-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89d21-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="89d21-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89d21-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="89d21-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="89d21-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="89d21-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89d21-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="89d21-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89d21-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="89d21-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="89d21-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="89d21-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89d21-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="89d21-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89d21-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="89d21-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="89d21-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="89d21-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89d21-154">createdDateTime</span></span>|<span data-ttu-id="89d21-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d21-155">DateTimeOffset</span></span>|<span data-ttu-id="89d21-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="89d21-156">DateTime the object was created.</span></span> <span data-ttu-id="89d21-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-158">说明</span><span class="sxs-lookup"><span data-stu-id="89d21-158">description</span></span>|<span data-ttu-id="89d21-159">String</span><span class="sxs-lookup"><span data-stu-id="89d21-159">String</span></span>|<span data-ttu-id="89d21-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="89d21-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89d21-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-162">displayName</span><span class="sxs-lookup"><span data-stu-id="89d21-162">displayName</span></span>|<span data-ttu-id="89d21-163">String</span><span class="sxs-lookup"><span data-stu-id="89d21-163">String</span></span>|<span data-ttu-id="89d21-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="89d21-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89d21-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-166">version</span><span class="sxs-lookup"><span data-stu-id="89d21-166">version</span></span>|<span data-ttu-id="89d21-167">Int32</span><span class="sxs-lookup"><span data-stu-id="89d21-167">Int32</span></span>|<span data-ttu-id="89d21-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="89d21-168">Version of the device configuration.</span></span> <span data-ttu-id="89d21-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-170">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="89d21-170">airPrintDestinations</span></span>|<span data-ttu-id="89d21-171">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-171">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="89d21-172">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="89d21-172">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="89d21-173">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="89d21-173">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89d21-174">关系</span><span class="sxs-lookup"><span data-stu-id="89d21-174">Relationships</span></span>
|<span data-ttu-id="89d21-175">关系</span><span class="sxs-lookup"><span data-stu-id="89d21-175">Relationship</span></span>|<span data-ttu-id="89d21-176">类型</span><span class="sxs-lookup"><span data-stu-id="89d21-176">Type</span></span>|<span data-ttu-id="89d21-177">说明</span><span class="sxs-lookup"><span data-stu-id="89d21-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d21-178">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="89d21-178">groupAssignments</span></span>|<span data-ttu-id="89d21-179">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-179">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="89d21-180">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="89d21-180">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="89d21-181">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-182">assignments</span><span class="sxs-lookup"><span data-stu-id="89d21-182">assignments</span></span>|<span data-ttu-id="89d21-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="89d21-184">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="89d21-184">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="89d21-185">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="89d21-186">deviceStatuses</span></span>|<span data-ttu-id="89d21-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="89d21-188">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="89d21-188">Device configuration installation status by device.</span></span> <span data-ttu-id="89d21-189">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-189">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-190">userStatuses</span><span class="sxs-lookup"><span data-stu-id="89d21-190">userStatuses</span></span>|<span data-ttu-id="89d21-191">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-191">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="89d21-192">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="89d21-192">Device configuration installation status by user.</span></span> <span data-ttu-id="89d21-193">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-193">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-194">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="89d21-194">deviceStatusOverview</span></span>|[<span data-ttu-id="89d21-195">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="89d21-195">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="89d21-196">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-196">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-197">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="89d21-197">userStatusOverview</span></span>|[<span data-ttu-id="89d21-198">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="89d21-198">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="89d21-199">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-199">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d21-200">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="89d21-200">deviceSettingStateSummaries</span></span>|<span data-ttu-id="89d21-201">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d21-201">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="89d21-202">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d21-202">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89d21-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89d21-203">JSON Representation</span></span>
<span data-ttu-id="89d21-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d21-204">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleDeviceFeaturesConfigurationBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
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
  "version": 1024,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ]
}
```





