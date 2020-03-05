---
title: appleDeviceFeaturesConfigurationBase 资源类型
description: Apple 设备功能配置的配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ea9eb2451dd9312475784097ae47048295ab4f12
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527131"
---
# <a name="appledevicefeaturesconfigurationbase-resource-type"></a><span data-ttu-id="fd2cc-103">appleDeviceFeaturesConfigurationBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd2cc-103">appleDeviceFeaturesConfigurationBase resource type</span></span>

<span data-ttu-id="fd2cc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fd2cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd2cc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd2cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd2cc-107">Apple 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-107">Apple device features configuration profile.</span></span>


<span data-ttu-id="fd2cc-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="fd2cc-109">方法</span><span class="sxs-lookup"><span data-stu-id="fd2cc-109">Methods</span></span>
|<span data-ttu-id="fd2cc-110">方法</span><span class="sxs-lookup"><span data-stu-id="fd2cc-110">Method</span></span>|<span data-ttu-id="fd2cc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd2cc-111">Return Type</span></span>|<span data-ttu-id="fd2cc-112">说明</span><span class="sxs-lookup"><span data-stu-id="fd2cc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd2cc-113">List appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="fd2cc-113">List appleDeviceFeaturesConfigurationBases</span></span>](../api/intune-deviceconfig-appledevicefeaturesconfigurationbase-list.md)|<span data-ttu-id="fd2cc-114">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-114">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) collection</span></span>|<span data-ttu-id="fd2cc-115">列出 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-115">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>|
|[<span data-ttu-id="fd2cc-116">Get appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="fd2cc-116">Get appleDeviceFeaturesConfigurationBase</span></span>](../api/intune-deviceconfig-appledevicefeaturesconfigurationbase-get.md)|[<span data-ttu-id="fd2cc-117">appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="fd2cc-117">appleDeviceFeaturesConfigurationBase</span></span>](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|<span data-ttu-id="fd2cc-118">读取 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-118">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd2cc-119">属性</span><span class="sxs-lookup"><span data-stu-id="fd2cc-119">Properties</span></span>
|<span data-ttu-id="fd2cc-120">属性</span><span class="sxs-lookup"><span data-stu-id="fd2cc-120">Property</span></span>|<span data-ttu-id="fd2cc-121">类型</span><span class="sxs-lookup"><span data-stu-id="fd2cc-121">Type</span></span>|<span data-ttu-id="fd2cc-122">说明</span><span class="sxs-lookup"><span data-stu-id="fd2cc-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd2cc-123">id</span><span class="sxs-lookup"><span data-stu-id="fd2cc-123">id</span></span>|<span data-ttu-id="fd2cc-124">字符串</span><span class="sxs-lookup"><span data-stu-id="fd2cc-124">String</span></span>|<span data-ttu-id="fd2cc-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-125">Key of the entity.</span></span> <span data-ttu-id="fd2cc-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2cc-127">lastModifiedDateTime</span></span>|<span data-ttu-id="fd2cc-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd2cc-128">DateTimeOffset</span></span>|<span data-ttu-id="fd2cc-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-129">DateTime the object was last modified.</span></span> <span data-ttu-id="fd2cc-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd2cc-131">roleScopeTagIds</span></span>|<span data-ttu-id="fd2cc-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-132">String collection</span></span>|<span data-ttu-id="fd2cc-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fd2cc-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fd2cc-135">supportsScopeTags</span></span>|<span data-ttu-id="fd2cc-136">布尔</span><span class="sxs-lookup"><span data-stu-id="fd2cc-136">Boolean</span></span>|<span data-ttu-id="fd2cc-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fd2cc-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fd2cc-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fd2cc-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-140">This property is read-only.</span></span> <span data-ttu-id="fd2cc-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fd2cc-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fd2cc-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fd2cc-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fd2cc-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fd2cc-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fd2cc-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fd2cc-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fd2cc-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fd2cc-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fd2cc-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fd2cc-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fd2cc-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fd2cc-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fd2cc-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fd2cc-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2cc-154">createdDateTime</span></span>|<span data-ttu-id="fd2cc-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd2cc-155">DateTimeOffset</span></span>|<span data-ttu-id="fd2cc-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-156">DateTime the object was created.</span></span> <span data-ttu-id="fd2cc-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-158">说明</span><span class="sxs-lookup"><span data-stu-id="fd2cc-158">description</span></span>|<span data-ttu-id="fd2cc-159">String</span><span class="sxs-lookup"><span data-stu-id="fd2cc-159">String</span></span>|<span data-ttu-id="fd2cc-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fd2cc-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-162">displayName</span><span class="sxs-lookup"><span data-stu-id="fd2cc-162">displayName</span></span>|<span data-ttu-id="fd2cc-163">String</span><span class="sxs-lookup"><span data-stu-id="fd2cc-163">String</span></span>|<span data-ttu-id="fd2cc-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fd2cc-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-166">version</span><span class="sxs-lookup"><span data-stu-id="fd2cc-166">version</span></span>|<span data-ttu-id="fd2cc-167">Int32</span><span class="sxs-lookup"><span data-stu-id="fd2cc-167">Int32</span></span>|<span data-ttu-id="fd2cc-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-168">Version of the device configuration.</span></span> <span data-ttu-id="fd2cc-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-170">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="fd2cc-170">airPrintDestinations</span></span>|<span data-ttu-id="fd2cc-171">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-171">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="fd2cc-172">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-172">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="fd2cc-173">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-173">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd2cc-174">关系</span><span class="sxs-lookup"><span data-stu-id="fd2cc-174">Relationships</span></span>
|<span data-ttu-id="fd2cc-175">关系</span><span class="sxs-lookup"><span data-stu-id="fd2cc-175">Relationship</span></span>|<span data-ttu-id="fd2cc-176">类型</span><span class="sxs-lookup"><span data-stu-id="fd2cc-176">Type</span></span>|<span data-ttu-id="fd2cc-177">说明</span><span class="sxs-lookup"><span data-stu-id="fd2cc-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd2cc-178">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="fd2cc-178">groupAssignments</span></span>|<span data-ttu-id="fd2cc-179">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-179">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="fd2cc-180">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-180">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="fd2cc-181">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-182">assignments</span><span class="sxs-lookup"><span data-stu-id="fd2cc-182">assignments</span></span>|<span data-ttu-id="fd2cc-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="fd2cc-184">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-184">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="fd2cc-185">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="fd2cc-186">deviceStatuses</span></span>|<span data-ttu-id="fd2cc-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="fd2cc-188">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-188">Device configuration installation status by device.</span></span> <span data-ttu-id="fd2cc-189">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-189">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-190">userStatuses</span><span class="sxs-lookup"><span data-stu-id="fd2cc-190">userStatuses</span></span>|<span data-ttu-id="fd2cc-191">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-191">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="fd2cc-192">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-192">Device configuration installation status by user.</span></span> <span data-ttu-id="fd2cc-193">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-193">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-194">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="fd2cc-194">deviceStatusOverview</span></span>|[<span data-ttu-id="fd2cc-195">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fd2cc-195">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="fd2cc-196">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-196">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-197">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="fd2cc-197">userStatusOverview</span></span>|[<span data-ttu-id="fd2cc-198">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="fd2cc-198">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="fd2cc-199">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-199">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd2cc-200">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="fd2cc-200">deviceSettingStateSummaries</span></span>|<span data-ttu-id="fd2cc-201">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd2cc-201">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="fd2cc-202">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd2cc-202">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd2cc-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd2cc-203">JSON Representation</span></span>
<span data-ttu-id="fd2cc-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd2cc-204">Here is a JSON representation of the resource.</span></span>
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



