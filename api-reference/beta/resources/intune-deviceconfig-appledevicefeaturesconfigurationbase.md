---
title: appleDeviceFeaturesConfigurationBase 资源类型
description: Apple 设备功能配置的配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf16c3fd21d64d2d479a14eb62bead849ca04e62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026815"
---
# <a name="appledevicefeaturesconfigurationbase-resource-type"></a><span data-ttu-id="83d07-103">appleDeviceFeaturesConfigurationBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="83d07-103">appleDeviceFeaturesConfigurationBase resource type</span></span>

<span data-ttu-id="83d07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83d07-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83d07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83d07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83d07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83d07-107">Apple 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="83d07-107">Apple device features configuration profile.</span></span>


<span data-ttu-id="83d07-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="83d07-109">方法</span><span class="sxs-lookup"><span data-stu-id="83d07-109">Methods</span></span>
|<span data-ttu-id="83d07-110">方法</span><span class="sxs-lookup"><span data-stu-id="83d07-110">Method</span></span>|<span data-ttu-id="83d07-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="83d07-111">Return Type</span></span>|<span data-ttu-id="83d07-112">说明</span><span class="sxs-lookup"><span data-stu-id="83d07-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83d07-113">List appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="83d07-113">List appleDeviceFeaturesConfigurationBases</span></span>](../api/intune-deviceconfig-appledevicefeaturesconfigurationbase-list.md)|<span data-ttu-id="83d07-114">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-114">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) collection</span></span>|<span data-ttu-id="83d07-115">列出 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83d07-115">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>|
|[<span data-ttu-id="83d07-116">Get appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="83d07-116">Get appleDeviceFeaturesConfigurationBase</span></span>](../api/intune-deviceconfig-appledevicefeaturesconfigurationbase-get.md)|[<span data-ttu-id="83d07-117">appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="83d07-117">appleDeviceFeaturesConfigurationBase</span></span>](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|<span data-ttu-id="83d07-118">读取 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83d07-118">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83d07-119">属性</span><span class="sxs-lookup"><span data-stu-id="83d07-119">Properties</span></span>
|<span data-ttu-id="83d07-120">属性</span><span class="sxs-lookup"><span data-stu-id="83d07-120">Property</span></span>|<span data-ttu-id="83d07-121">类型</span><span class="sxs-lookup"><span data-stu-id="83d07-121">Type</span></span>|<span data-ttu-id="83d07-122">说明</span><span class="sxs-lookup"><span data-stu-id="83d07-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83d07-123">id</span><span class="sxs-lookup"><span data-stu-id="83d07-123">id</span></span>|<span data-ttu-id="83d07-124">String</span><span class="sxs-lookup"><span data-stu-id="83d07-124">String</span></span>|<span data-ttu-id="83d07-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83d07-125">Key of the entity.</span></span> <span data-ttu-id="83d07-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83d07-127">lastModifiedDateTime</span></span>|<span data-ttu-id="83d07-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d07-128">DateTimeOffset</span></span>|<span data-ttu-id="83d07-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83d07-129">DateTime the object was last modified.</span></span> <span data-ttu-id="83d07-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83d07-131">roleScopeTagIds</span></span>|<span data-ttu-id="83d07-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-132">String collection</span></span>|<span data-ttu-id="83d07-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="83d07-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83d07-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83d07-135">supportsScopeTags</span></span>|<span data-ttu-id="83d07-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="83d07-136">Boolean</span></span>|<span data-ttu-id="83d07-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="83d07-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83d07-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="83d07-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83d07-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="83d07-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83d07-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="83d07-140">This property is read-only.</span></span> <span data-ttu-id="83d07-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83d07-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83d07-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83d07-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83d07-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="83d07-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83d07-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83d07-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83d07-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83d07-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83d07-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="83d07-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83d07-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83d07-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83d07-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83d07-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83d07-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="83d07-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83d07-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83d07-154">createdDateTime</span></span>|<span data-ttu-id="83d07-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d07-155">DateTimeOffset</span></span>|<span data-ttu-id="83d07-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83d07-156">DateTime the object was created.</span></span> <span data-ttu-id="83d07-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-158">description</span><span class="sxs-lookup"><span data-stu-id="83d07-158">description</span></span>|<span data-ttu-id="83d07-159">String</span><span class="sxs-lookup"><span data-stu-id="83d07-159">String</span></span>|<span data-ttu-id="83d07-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="83d07-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83d07-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-162">displayName</span><span class="sxs-lookup"><span data-stu-id="83d07-162">displayName</span></span>|<span data-ttu-id="83d07-163">String</span><span class="sxs-lookup"><span data-stu-id="83d07-163">String</span></span>|<span data-ttu-id="83d07-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="83d07-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83d07-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-166">version</span><span class="sxs-lookup"><span data-stu-id="83d07-166">version</span></span>|<span data-ttu-id="83d07-167">Int32</span><span class="sxs-lookup"><span data-stu-id="83d07-167">Int32</span></span>|<span data-ttu-id="83d07-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="83d07-168">Version of the device configuration.</span></span> <span data-ttu-id="83d07-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-170">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="83d07-170">airPrintDestinations</span></span>|<span data-ttu-id="83d07-171">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-171">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="83d07-172">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="83d07-172">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="83d07-173">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="83d07-173">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83d07-174">关系</span><span class="sxs-lookup"><span data-stu-id="83d07-174">Relationships</span></span>
|<span data-ttu-id="83d07-175">关系</span><span class="sxs-lookup"><span data-stu-id="83d07-175">Relationship</span></span>|<span data-ttu-id="83d07-176">类型</span><span class="sxs-lookup"><span data-stu-id="83d07-176">Type</span></span>|<span data-ttu-id="83d07-177">说明</span><span class="sxs-lookup"><span data-stu-id="83d07-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83d07-178">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="83d07-178">groupAssignments</span></span>|<span data-ttu-id="83d07-179">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-179">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="83d07-180">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="83d07-180">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="83d07-181">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-182">assignments</span><span class="sxs-lookup"><span data-stu-id="83d07-182">assignments</span></span>|<span data-ttu-id="83d07-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="83d07-184">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="83d07-184">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="83d07-185">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="83d07-186">deviceStatuses</span></span>|<span data-ttu-id="83d07-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="83d07-188">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="83d07-188">Device configuration installation status by device.</span></span> <span data-ttu-id="83d07-189">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-189">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-190">userStatuses</span><span class="sxs-lookup"><span data-stu-id="83d07-190">userStatuses</span></span>|<span data-ttu-id="83d07-191">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-191">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="83d07-192">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="83d07-192">Device configuration installation status by user.</span></span> <span data-ttu-id="83d07-193">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-193">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-194">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="83d07-194">deviceStatusOverview</span></span>|[<span data-ttu-id="83d07-195">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83d07-195">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="83d07-196">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-196">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-197">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="83d07-197">userStatusOverview</span></span>|[<span data-ttu-id="83d07-198">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="83d07-198">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="83d07-199">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-199">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d07-200">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="83d07-200">deviceSettingStateSummaries</span></span>|<span data-ttu-id="83d07-201">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83d07-201">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="83d07-202">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83d07-202">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83d07-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83d07-203">JSON Representation</span></span>
<span data-ttu-id="83d07-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83d07-204">Here is a JSON representation of the resource.</span></span>
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






