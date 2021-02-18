---
title: iosUpdateConfiguration 资源类型
description: IOS 更新配置，允许配置一周内的时间范围，用于安装 iOS 更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f099a83ba892edada8288936eac59542059e4f39
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292460"
---
# <a name="iosupdateconfiguration-resource-type"></a><span data-ttu-id="7fb9d-103">iosUpdateConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fb9d-103">iosUpdateConfiguration resource type</span></span>

<span data-ttu-id="7fb9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fb9d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fb9d-106">IOS 更新配置，允许配置一周内的时间范围，用于安装 iOS 更新。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-106">IOS Update Configuration, allows you to configure time window within week to install iOS updates</span></span>


<span data-ttu-id="7fb9d-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7fb9d-108">方法</span><span class="sxs-lookup"><span data-stu-id="7fb9d-108">Methods</span></span>
|<span data-ttu-id="7fb9d-109">方法</span><span class="sxs-lookup"><span data-stu-id="7fb9d-109">Method</span></span>|<span data-ttu-id="7fb9d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7fb9d-110">Return Type</span></span>|<span data-ttu-id="7fb9d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7fb9d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7fb9d-112">List iosUpdateConfigurations</span><span class="sxs-lookup"><span data-stu-id="7fb9d-112">List iosUpdateConfigurations</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-list.md)|<span data-ttu-id="7fb9d-113">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fb9d-113">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) collection</span></span>|<span data-ttu-id="7fb9d-114">列出 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-114">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7fb9d-115">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-115">Get iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-get.md)|[<span data-ttu-id="7fb9d-116">iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-116">iosUpdateConfiguration</span></span>](../resources/intune-deviceconfig-iosupdateconfiguration.md)|<span data-ttu-id="7fb9d-117">读取 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-117">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7fb9d-118">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-118">Create iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-create.md)|[<span data-ttu-id="7fb9d-119">iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-119">iosUpdateConfiguration</span></span>](../resources/intune-deviceconfig-iosupdateconfiguration.md)|<span data-ttu-id="7fb9d-120">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-120">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7fb9d-121">Delete iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-121">Delete iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-delete.md)|<span data-ttu-id="7fb9d-122">无</span><span class="sxs-lookup"><span data-stu-id="7fb9d-122">None</span></span>|<span data-ttu-id="7fb9d-123">删除 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-123">Deletes a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>|
|[<span data-ttu-id="7fb9d-124">Update iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-124">Update iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-update.md)|[<span data-ttu-id="7fb9d-125">iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fb9d-125">iosUpdateConfiguration</span></span>](../resources/intune-deviceconfig-iosupdateconfiguration.md)|<span data-ttu-id="7fb9d-126">更新 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-126">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7fb9d-127">属性</span><span class="sxs-lookup"><span data-stu-id="7fb9d-127">Properties</span></span>
|<span data-ttu-id="7fb9d-128">属性</span><span class="sxs-lookup"><span data-stu-id="7fb9d-128">Property</span></span>|<span data-ttu-id="7fb9d-129">类型</span><span class="sxs-lookup"><span data-stu-id="7fb9d-129">Type</span></span>|<span data-ttu-id="7fb9d-130">说明</span><span class="sxs-lookup"><span data-stu-id="7fb9d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fb9d-131">id</span><span class="sxs-lookup"><span data-stu-id="7fb9d-131">id</span></span>|<span data-ttu-id="7fb9d-132">String</span><span class="sxs-lookup"><span data-stu-id="7fb9d-132">String</span></span>|<span data-ttu-id="7fb9d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-133">Key of the entity.</span></span> <span data-ttu-id="7fb9d-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fb9d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7fb9d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fb9d-136">DateTimeOffset</span></span>|<span data-ttu-id="7fb9d-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7fb9d-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fb9d-139">createdDateTime</span></span>|<span data-ttu-id="7fb9d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fb9d-140">DateTimeOffset</span></span>|<span data-ttu-id="7fb9d-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-141">DateTime the object was created.</span></span> <span data-ttu-id="7fb9d-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-143">description</span><span class="sxs-lookup"><span data-stu-id="7fb9d-143">description</span></span>|<span data-ttu-id="7fb9d-144">String</span><span class="sxs-lookup"><span data-stu-id="7fb9d-144">String</span></span>|<span data-ttu-id="7fb9d-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7fb9d-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7fb9d-147">displayName</span></span>|<span data-ttu-id="7fb9d-148">String</span><span class="sxs-lookup"><span data-stu-id="7fb9d-148">String</span></span>|<span data-ttu-id="7fb9d-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7fb9d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-151">version</span><span class="sxs-lookup"><span data-stu-id="7fb9d-151">version</span></span>|<span data-ttu-id="7fb9d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb9d-152">Int32</span></span>|<span data-ttu-id="7fb9d-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-153">Version of the device configuration.</span></span> <span data-ttu-id="7fb9d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7fb9d-155">activeHoursStart</span></span>|<span data-ttu-id="7fb9d-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7fb9d-156">TimeOfDay</span></span>|<span data-ttu-id="7fb9d-157">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="7fb9d-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7fb9d-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7fb9d-158">activeHoursEnd</span></span>|<span data-ttu-id="7fb9d-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7fb9d-159">TimeOfDay</span></span>|<span data-ttu-id="7fb9d-160">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="7fb9d-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7fb9d-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="7fb9d-161">scheduledInstallDays</span></span>|<span data-ttu-id="7fb9d-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fb9d-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="7fb9d-163">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="7fb9d-164">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-164">This collection can contain a maximum of 7 elements.</span></span>|
|<span data-ttu-id="7fb9d-165">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="7fb9d-165">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="7fb9d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb9d-166">Int32</span></span>|<span data-ttu-id="7fb9d-167">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="7fb9d-167">UTC Time Offset indicated in minutes</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fb9d-168">关系</span><span class="sxs-lookup"><span data-stu-id="7fb9d-168">Relationships</span></span>
|<span data-ttu-id="7fb9d-169">关系</span><span class="sxs-lookup"><span data-stu-id="7fb9d-169">Relationship</span></span>|<span data-ttu-id="7fb9d-170">类型</span><span class="sxs-lookup"><span data-stu-id="7fb9d-170">Type</span></span>|<span data-ttu-id="7fb9d-171">说明</span><span class="sxs-lookup"><span data-stu-id="7fb9d-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fb9d-172">assignments</span><span class="sxs-lookup"><span data-stu-id="7fb9d-172">assignments</span></span>|<span data-ttu-id="7fb9d-173">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fb9d-173">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7fb9d-174">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-174">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="7fb9d-175">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-175">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-176">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7fb9d-176">deviceStatuses</span></span>|<span data-ttu-id="7fb9d-177">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fb9d-177">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7fb9d-178">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-178">Device configuration installation status by device.</span></span> <span data-ttu-id="7fb9d-179">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-180">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7fb9d-180">userStatuses</span></span>|<span data-ttu-id="7fb9d-181">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fb9d-181">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7fb9d-182">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-182">Device configuration installation status by user.</span></span> <span data-ttu-id="7fb9d-183">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-184">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7fb9d-184">deviceStatusOverview</span></span>|[<span data-ttu-id="7fb9d-185">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7fb9d-185">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7fb9d-186">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-186">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-187">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7fb9d-187">userStatusOverview</span></span>|[<span data-ttu-id="7fb9d-188">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7fb9d-188">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7fb9d-189">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-189">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fb9d-190">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7fb9d-190">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7fb9d-191">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fb9d-191">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7fb9d-192">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7fb9d-192">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fb9d-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fb9d-193">JSON Representation</span></span>
<span data-ttu-id="7fb9d-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fb9d-194">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
  ],
}
-->








