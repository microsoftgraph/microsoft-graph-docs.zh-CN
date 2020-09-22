---
title: iosUpdateConfiguration 资源类型
description: IOS 更新配置，允许配置一周内的时间范围，用于安装 iOS 更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffdf3097d846ba71b1049ad390b5c3cc3130b6f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091682"
---
# <a name="iosupdateconfiguration-resource-type"></a><span data-ttu-id="19a71-103">iosUpdateConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="19a71-103">iosUpdateConfiguration resource type</span></span>

<span data-ttu-id="19a71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19a71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19a71-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19a71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19a71-106">IOS 更新配置，允许配置一周内的时间范围，用于安装 iOS 更新。</span><span class="sxs-lookup"><span data-stu-id="19a71-106">IOS Update Configuration, allows you to configure time window within week to install iOS updates</span></span>


<span data-ttu-id="19a71-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="19a71-108">方法</span><span class="sxs-lookup"><span data-stu-id="19a71-108">Methods</span></span>
|<span data-ttu-id="19a71-109">方法</span><span class="sxs-lookup"><span data-stu-id="19a71-109">Method</span></span>|<span data-ttu-id="19a71-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="19a71-110">Return Type</span></span>|<span data-ttu-id="19a71-111">说明</span><span class="sxs-lookup"><span data-stu-id="19a71-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19a71-112">List iosUpdateConfigurations</span><span class="sxs-lookup"><span data-stu-id="19a71-112">List iosUpdateConfigurations</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-list.md)|<span data-ttu-id="19a71-113">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19a71-113">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) collection</span></span>|<span data-ttu-id="19a71-114">列出 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19a71-114">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="19a71-115">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-115">Get iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-get.md)|[<span data-ttu-id="19a71-116">iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-116">iosUpdateConfiguration</span></span>](../resources/intune-deviceconfig-iosupdateconfiguration.md)|<span data-ttu-id="19a71-117">读取 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19a71-117">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>|
|[<span data-ttu-id="19a71-118">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-118">Create iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-create.md)|[<span data-ttu-id="19a71-119">iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-119">iosUpdateConfiguration</span></span>](../resources/intune-deviceconfig-iosupdateconfiguration.md)|<span data-ttu-id="19a71-120">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19a71-120">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>|
|[<span data-ttu-id="19a71-121">Delete iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-121">Delete iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-delete.md)|<span data-ttu-id="19a71-122">无</span><span class="sxs-lookup"><span data-stu-id="19a71-122">None</span></span>|<span data-ttu-id="19a71-123">删除 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="19a71-123">Deletes a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>|
|[<span data-ttu-id="19a71-124">Update iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-124">Update iosUpdateConfiguration</span></span>](../api/intune-deviceconfig-iosupdateconfiguration-update.md)|[<span data-ttu-id="19a71-125">iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="19a71-125">iosUpdateConfiguration</span></span>](../resources/intune-deviceconfig-iosupdateconfiguration.md)|<span data-ttu-id="19a71-126">更新 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="19a71-126">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19a71-127">属性</span><span class="sxs-lookup"><span data-stu-id="19a71-127">Properties</span></span>
|<span data-ttu-id="19a71-128">属性</span><span class="sxs-lookup"><span data-stu-id="19a71-128">Property</span></span>|<span data-ttu-id="19a71-129">类型</span><span class="sxs-lookup"><span data-stu-id="19a71-129">Type</span></span>|<span data-ttu-id="19a71-130">说明</span><span class="sxs-lookup"><span data-stu-id="19a71-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a71-131">id</span><span class="sxs-lookup"><span data-stu-id="19a71-131">id</span></span>|<span data-ttu-id="19a71-132">String</span><span class="sxs-lookup"><span data-stu-id="19a71-132">String</span></span>|<span data-ttu-id="19a71-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="19a71-133">Key of the entity.</span></span> <span data-ttu-id="19a71-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19a71-135">lastModifiedDateTime</span></span>|<span data-ttu-id="19a71-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a71-136">DateTimeOffset</span></span>|<span data-ttu-id="19a71-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="19a71-137">DateTime the object was last modified.</span></span> <span data-ttu-id="19a71-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19a71-139">createdDateTime</span></span>|<span data-ttu-id="19a71-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a71-140">DateTimeOffset</span></span>|<span data-ttu-id="19a71-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="19a71-141">DateTime the object was created.</span></span> <span data-ttu-id="19a71-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-143">description</span><span class="sxs-lookup"><span data-stu-id="19a71-143">description</span></span>|<span data-ttu-id="19a71-144">String</span><span class="sxs-lookup"><span data-stu-id="19a71-144">String</span></span>|<span data-ttu-id="19a71-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="19a71-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19a71-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-147">displayName</span><span class="sxs-lookup"><span data-stu-id="19a71-147">displayName</span></span>|<span data-ttu-id="19a71-148">String</span><span class="sxs-lookup"><span data-stu-id="19a71-148">String</span></span>|<span data-ttu-id="19a71-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="19a71-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19a71-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-151">version</span><span class="sxs-lookup"><span data-stu-id="19a71-151">version</span></span>|<span data-ttu-id="19a71-152">Int32</span><span class="sxs-lookup"><span data-stu-id="19a71-152">Int32</span></span>|<span data-ttu-id="19a71-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="19a71-153">Version of the device configuration.</span></span> <span data-ttu-id="19a71-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="19a71-155">activeHoursStart</span></span>|<span data-ttu-id="19a71-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="19a71-156">TimeOfDay</span></span>|<span data-ttu-id="19a71-157">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="19a71-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="19a71-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="19a71-158">activeHoursEnd</span></span>|<span data-ttu-id="19a71-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="19a71-159">TimeOfDay</span></span>|<span data-ttu-id="19a71-160">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="19a71-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="19a71-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="19a71-161">scheduledInstallDays</span></span>|<span data-ttu-id="19a71-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19a71-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="19a71-163">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="19a71-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="19a71-164">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="19a71-164">This collection can contain a maximum of 7 elements.</span></span>|
|<span data-ttu-id="19a71-165">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="19a71-165">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="19a71-166">Int32</span><span class="sxs-lookup"><span data-stu-id="19a71-166">Int32</span></span>|<span data-ttu-id="19a71-167">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="19a71-167">UTC Time Offset indicated in minutes</span></span>|

## <a name="relationships"></a><span data-ttu-id="19a71-168">关系</span><span class="sxs-lookup"><span data-stu-id="19a71-168">Relationships</span></span>
|<span data-ttu-id="19a71-169">关系</span><span class="sxs-lookup"><span data-stu-id="19a71-169">Relationship</span></span>|<span data-ttu-id="19a71-170">类型</span><span class="sxs-lookup"><span data-stu-id="19a71-170">Type</span></span>|<span data-ttu-id="19a71-171">说明</span><span class="sxs-lookup"><span data-stu-id="19a71-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a71-172">assignments</span><span class="sxs-lookup"><span data-stu-id="19a71-172">assignments</span></span>|<span data-ttu-id="19a71-173">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19a71-173">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="19a71-174">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="19a71-174">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="19a71-175">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-175">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-176">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="19a71-176">deviceStatuses</span></span>|<span data-ttu-id="19a71-177">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19a71-177">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="19a71-178">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="19a71-178">Device configuration installation status by device.</span></span> <span data-ttu-id="19a71-179">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-180">userStatuses</span><span class="sxs-lookup"><span data-stu-id="19a71-180">userStatuses</span></span>|<span data-ttu-id="19a71-181">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19a71-181">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="19a71-182">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="19a71-182">Device configuration installation status by user.</span></span> <span data-ttu-id="19a71-183">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-184">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="19a71-184">deviceStatusOverview</span></span>|[<span data-ttu-id="19a71-185">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="19a71-185">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="19a71-186">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-186">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-187">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="19a71-187">userStatusOverview</span></span>|[<span data-ttu-id="19a71-188">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="19a71-188">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="19a71-189">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-189">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19a71-190">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="19a71-190">deviceSettingStateSummaries</span></span>|<span data-ttu-id="19a71-191">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19a71-191">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="19a71-192">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19a71-192">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19a71-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19a71-193">JSON Representation</span></span>
<span data-ttu-id="19a71-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19a71-194">Here is a JSON representation of the resource.</span></span>
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
     "Warning: /api-reference/v1.0/resources/intune-deviceconfig-iosupdateconfiguration.md/microsoft.graph.iosUpdateConfiguration/scheduledInstallDays:
     Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->








