---
title: deviceConfiguration 资源类型
description: 设备配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1927b4af889fb98e2e9c33561b9ff63042df5b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465739"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="97159-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="97159-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="97159-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97159-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97159-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97159-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97159-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="97159-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="97159-107">方法</span><span class="sxs-lookup"><span data-stu-id="97159-107">Methods</span></span>
|<span data-ttu-id="97159-108">方法</span><span class="sxs-lookup"><span data-stu-id="97159-108">Method</span></span>|<span data-ttu-id="97159-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="97159-109">Return Type</span></span>|<span data-ttu-id="97159-110">说明</span><span class="sxs-lookup"><span data-stu-id="97159-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97159-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="97159-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="97159-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97159-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="97159-113">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97159-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="97159-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="97159-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="97159-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="97159-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="97159-116">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97159-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="97159-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="97159-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="97159-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97159-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="97159-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97159-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="97159-120">属性</span><span class="sxs-lookup"><span data-stu-id="97159-120">Properties</span></span>
|<span data-ttu-id="97159-121">属性</span><span class="sxs-lookup"><span data-stu-id="97159-121">Property</span></span>|<span data-ttu-id="97159-122">类型</span><span class="sxs-lookup"><span data-stu-id="97159-122">Type</span></span>|<span data-ttu-id="97159-123">说明</span><span class="sxs-lookup"><span data-stu-id="97159-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97159-124">id</span><span class="sxs-lookup"><span data-stu-id="97159-124">id</span></span>|<span data-ttu-id="97159-125">字符串</span><span class="sxs-lookup"><span data-stu-id="97159-125">String</span></span>|<span data-ttu-id="97159-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97159-126">Key of the entity.</span></span>|
|<span data-ttu-id="97159-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97159-127">lastModifiedDateTime</span></span>|<span data-ttu-id="97159-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97159-128">DateTimeOffset</span></span>|<span data-ttu-id="97159-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97159-129">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="97159-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97159-130">createdDateTime</span></span>|<span data-ttu-id="97159-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97159-131">DateTimeOffset</span></span>|<span data-ttu-id="97159-132">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97159-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="97159-133">description</span><span class="sxs-lookup"><span data-stu-id="97159-133">description</span></span>|<span data-ttu-id="97159-134">String</span><span class="sxs-lookup"><span data-stu-id="97159-134">String</span></span>|<span data-ttu-id="97159-135">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="97159-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="97159-136">displayName</span><span class="sxs-lookup"><span data-stu-id="97159-136">displayName</span></span>|<span data-ttu-id="97159-137">String</span><span class="sxs-lookup"><span data-stu-id="97159-137">String</span></span>|<span data-ttu-id="97159-138">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="97159-138">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="97159-139">version</span><span class="sxs-lookup"><span data-stu-id="97159-139">version</span></span>|<span data-ttu-id="97159-140">Int32</span><span class="sxs-lookup"><span data-stu-id="97159-140">Int32</span></span>|<span data-ttu-id="97159-141">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="97159-141">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97159-142">关系</span><span class="sxs-lookup"><span data-stu-id="97159-142">Relationships</span></span>
|<span data-ttu-id="97159-143">关系</span><span class="sxs-lookup"><span data-stu-id="97159-143">Relationship</span></span>|<span data-ttu-id="97159-144">类型</span><span class="sxs-lookup"><span data-stu-id="97159-144">Type</span></span>|<span data-ttu-id="97159-145">说明</span><span class="sxs-lookup"><span data-stu-id="97159-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97159-146">assignments</span><span class="sxs-lookup"><span data-stu-id="97159-146">assignments</span></span>|<span data-ttu-id="97159-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97159-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="97159-148">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="97159-148">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="97159-149">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="97159-149">deviceStatuses</span></span>|<span data-ttu-id="97159-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97159-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="97159-151">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="97159-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="97159-152">userStatuses</span><span class="sxs-lookup"><span data-stu-id="97159-152">userStatuses</span></span>|<span data-ttu-id="97159-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97159-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="97159-154">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="97159-154">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="97159-155">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="97159-155">deviceStatusOverview</span></span>|[<span data-ttu-id="97159-156">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="97159-156">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="97159-157">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="97159-157">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="97159-158">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="97159-158">userStatusOverview</span></span>|[<span data-ttu-id="97159-159">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="97159-159">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="97159-160">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="97159-160">Device Configuration users status overview</span></span>|
|<span data-ttu-id="97159-161">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="97159-161">deviceSettingStateSummaries</span></span>|<span data-ttu-id="97159-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97159-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="97159-163">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="97159-163">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97159-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97159-164">JSON Representation</span></span>
<span data-ttu-id="97159-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97159-165">Here is a JSON representation of the resource.</span></span>
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







