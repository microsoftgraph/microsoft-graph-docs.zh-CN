---
title: deviceConfiguration 资源类型
description: 设备配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f4fa3abbfd7b4cb71db0f4f28dabce0157c046c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570339"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="8ac0a-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ac0a-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="8ac0a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ac0a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ac0a-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8ac0a-107">方法</span><span class="sxs-lookup"><span data-stu-id="8ac0a-107">Methods</span></span>
|<span data-ttu-id="8ac0a-108">方法</span><span class="sxs-lookup"><span data-stu-id="8ac0a-108">Method</span></span>|<span data-ttu-id="8ac0a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8ac0a-109">Return Type</span></span>|<span data-ttu-id="8ac0a-110">说明</span><span class="sxs-lookup"><span data-stu-id="8ac0a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ac0a-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="8ac0a-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="8ac0a-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="8ac0a-113">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8ac0a-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ac0a-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="8ac0a-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ac0a-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="8ac0a-116">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8ac0a-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="8ac0a-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="8ac0a-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8ac0a-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8ac0a-119">Not yet documented</span></span>|
|[<span data-ttu-id="8ac0a-120">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="8ac0a-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="8ac0a-121">无</span><span class="sxs-lookup"><span data-stu-id="8ac0a-121">None</span></span>|<span data-ttu-id="8ac0a-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8ac0a-122">Not yet documented</span></span>|
|[<span data-ttu-id="8ac0a-123">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="8ac0a-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="8ac0a-124">无</span><span class="sxs-lookup"><span data-stu-id="8ac0a-124">None</span></span>|<span data-ttu-id="8ac0a-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8ac0a-125">Not yet documented</span></span>|
|[<span data-ttu-id="8ac0a-126">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="8ac0a-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="8ac0a-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="8ac0a-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8ac0a-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8ac0a-129">属性</span><span class="sxs-lookup"><span data-stu-id="8ac0a-129">Properties</span></span>
|<span data-ttu-id="8ac0a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8ac0a-130">Property</span></span>|<span data-ttu-id="8ac0a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8ac0a-131">Type</span></span>|<span data-ttu-id="8ac0a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8ac0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac0a-133">id</span><span class="sxs-lookup"><span data-stu-id="8ac0a-133">id</span></span>|<span data-ttu-id="8ac0a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8ac0a-134">String</span></span>|<span data-ttu-id="8ac0a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-135">Key of the entity.</span></span>|
|<span data-ttu-id="8ac0a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ac0a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8ac0a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ac0a-137">DateTimeOffset</span></span>|<span data-ttu-id="8ac0a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8ac0a-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ac0a-139">roleScopeTagIds</span></span>|<span data-ttu-id="8ac0a-140">String collection</span><span class="sxs-lookup"><span data-stu-id="8ac0a-140">String collection</span></span>|<span data-ttu-id="8ac0a-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="8ac0a-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ac0a-142">supportsScopeTags</span></span>|<span data-ttu-id="8ac0a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ac0a-143">Boolean</span></span>|<span data-ttu-id="8ac0a-144">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ac0a-145">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ac0a-146">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ac0a-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-147">This property is read-only.</span></span>|
|<span data-ttu-id="8ac0a-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ac0a-148">createdDateTime</span></span>|<span data-ttu-id="8ac0a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ac0a-149">DateTimeOffset</span></span>|<span data-ttu-id="8ac0a-150">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-150">DateTime the object was created.</span></span>|
|<span data-ttu-id="8ac0a-151">说明</span><span class="sxs-lookup"><span data-stu-id="8ac0a-151">description</span></span>|<span data-ttu-id="8ac0a-152">String</span><span class="sxs-lookup"><span data-stu-id="8ac0a-152">String</span></span>|<span data-ttu-id="8ac0a-153">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-153">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8ac0a-154">displayName</span><span class="sxs-lookup"><span data-stu-id="8ac0a-154">displayName</span></span>|<span data-ttu-id="8ac0a-155">String</span><span class="sxs-lookup"><span data-stu-id="8ac0a-155">String</span></span>|<span data-ttu-id="8ac0a-156">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-156">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8ac0a-157">version</span><span class="sxs-lookup"><span data-stu-id="8ac0a-157">version</span></span>|<span data-ttu-id="8ac0a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8ac0a-158">Int32</span></span>|<span data-ttu-id="8ac0a-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-159">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ac0a-160">关系</span><span class="sxs-lookup"><span data-stu-id="8ac0a-160">Relationships</span></span>
|<span data-ttu-id="8ac0a-161">关系</span><span class="sxs-lookup"><span data-stu-id="8ac0a-161">Relationship</span></span>|<span data-ttu-id="8ac0a-162">类型</span><span class="sxs-lookup"><span data-stu-id="8ac0a-162">Type</span></span>|<span data-ttu-id="8ac0a-163">说明</span><span class="sxs-lookup"><span data-stu-id="8ac0a-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac0a-164">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="8ac0a-164">groupAssignments</span></span>|<span data-ttu-id="8ac0a-165">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-165">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="8ac0a-166">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-166">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="8ac0a-167">assignments</span><span class="sxs-lookup"><span data-stu-id="8ac0a-167">assignments</span></span>|<span data-ttu-id="8ac0a-168">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-168">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8ac0a-169">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-169">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="8ac0a-170">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8ac0a-170">deviceStatuses</span></span>|<span data-ttu-id="8ac0a-171">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-171">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8ac0a-172">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-172">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="8ac0a-173">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8ac0a-173">userStatuses</span></span>|<span data-ttu-id="8ac0a-174">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-174">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8ac0a-175">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-175">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="8ac0a-176">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8ac0a-176">deviceStatusOverview</span></span>|[<span data-ttu-id="8ac0a-177">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ac0a-177">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="8ac0a-178">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="8ac0a-178">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="8ac0a-179">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8ac0a-179">userStatusOverview</span></span>|[<span data-ttu-id="8ac0a-180">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="8ac0a-180">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="8ac0a-181">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="8ac0a-181">Device Configuration users status overview</span></span>|
|<span data-ttu-id="8ac0a-182">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="8ac0a-182">deviceSettingStateSummaries</span></span>|<span data-ttu-id="8ac0a-183">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ac0a-183">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8ac0a-184">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="8ac0a-184">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ac0a-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ac0a-185">JSON Representation</span></span>
<span data-ttu-id="8ac0a-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ac0a-186">Here is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```





