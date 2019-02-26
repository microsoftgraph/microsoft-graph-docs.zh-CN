---
title: deviceConfiguration 资源类型
description: 设备配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a3d0ecc27fc0fe29ed2ed3ca4080e3fea70d264
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250493"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="3a553-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a553-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="3a553-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a553-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a553-105">设备配置。</span><span class="sxs-lookup"><span data-stu-id="3a553-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="3a553-106">方法</span><span class="sxs-lookup"><span data-stu-id="3a553-106">Methods</span></span>
|<span data-ttu-id="3a553-107">方法</span><span class="sxs-lookup"><span data-stu-id="3a553-107">Method</span></span>|<span data-ttu-id="3a553-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3a553-108">Return Type</span></span>|<span data-ttu-id="3a553-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a553-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3a553-110">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="3a553-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="3a553-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a553-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="3a553-112">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a553-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3a553-113">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a553-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="3a553-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a553-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="3a553-115">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a553-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3a553-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="3a553-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="3a553-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a553-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3a553-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3a553-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3a553-119">属性</span><span class="sxs-lookup"><span data-stu-id="3a553-119">Properties</span></span>
|<span data-ttu-id="3a553-120">属性</span><span class="sxs-lookup"><span data-stu-id="3a553-120">Property</span></span>|<span data-ttu-id="3a553-121">类型</span><span class="sxs-lookup"><span data-stu-id="3a553-121">Type</span></span>|<span data-ttu-id="3a553-122">说明</span><span class="sxs-lookup"><span data-stu-id="3a553-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a553-123">id</span><span class="sxs-lookup"><span data-stu-id="3a553-123">id</span></span>|<span data-ttu-id="3a553-124">String</span><span class="sxs-lookup"><span data-stu-id="3a553-124">String</span></span>|<span data-ttu-id="3a553-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3a553-125">Key of the entity.</span></span>|
|<span data-ttu-id="3a553-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a553-126">lastModifiedDateTime</span></span>|<span data-ttu-id="3a553-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a553-127">DateTimeOffset</span></span>|<span data-ttu-id="3a553-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3a553-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3a553-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a553-129">createdDateTime</span></span>|<span data-ttu-id="3a553-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a553-130">DateTimeOffset</span></span>|<span data-ttu-id="3a553-131">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3a553-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="3a553-132">description</span><span class="sxs-lookup"><span data-stu-id="3a553-132">description</span></span>|<span data-ttu-id="3a553-133">String</span><span class="sxs-lookup"><span data-stu-id="3a553-133">String</span></span>|<span data-ttu-id="3a553-134">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="3a553-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="3a553-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3a553-135">displayName</span></span>|<span data-ttu-id="3a553-136">String</span><span class="sxs-lookup"><span data-stu-id="3a553-136">String</span></span>|<span data-ttu-id="3a553-137">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="3a553-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="3a553-138">version</span><span class="sxs-lookup"><span data-stu-id="3a553-138">version</span></span>|<span data-ttu-id="3a553-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3a553-139">Int32</span></span>|<span data-ttu-id="3a553-140">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3a553-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a553-141">关系</span><span class="sxs-lookup"><span data-stu-id="3a553-141">Relationships</span></span>
|<span data-ttu-id="3a553-142">关系</span><span class="sxs-lookup"><span data-stu-id="3a553-142">Relationship</span></span>|<span data-ttu-id="3a553-143">类型</span><span class="sxs-lookup"><span data-stu-id="3a553-143">Type</span></span>|<span data-ttu-id="3a553-144">说明</span><span class="sxs-lookup"><span data-stu-id="3a553-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a553-145">assignments</span><span class="sxs-lookup"><span data-stu-id="3a553-145">assignments</span></span>|<span data-ttu-id="3a553-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a553-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3a553-147">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="3a553-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="3a553-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3a553-148">deviceStatuses</span></span>|<span data-ttu-id="3a553-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a553-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3a553-150">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3a553-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="3a553-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3a553-151">userStatuses</span></span>|<span data-ttu-id="3a553-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a553-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3a553-153">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3a553-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="3a553-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3a553-154">deviceStatusOverview</span></span>|[<span data-ttu-id="3a553-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3a553-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3a553-156">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="3a553-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="3a553-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3a553-157">userStatusOverview</span></span>|[<span data-ttu-id="3a553-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3a553-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3a553-159">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="3a553-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="3a553-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3a553-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3a553-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a553-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3a553-162">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="3a553-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a553-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a553-163">JSON Representation</span></span>
<span data-ttu-id="3a553-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a553-164">Here is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



