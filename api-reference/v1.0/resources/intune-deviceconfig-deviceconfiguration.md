---
title: deviceConfiguration 资源类型
description: 设备配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b054e2472965f59d8350a52fe22134ab98e00fdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028432"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="683ac-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="683ac-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="683ac-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="683ac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="683ac-105">设备配置。</span><span class="sxs-lookup"><span data-stu-id="683ac-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="683ac-106">方法</span><span class="sxs-lookup"><span data-stu-id="683ac-106">Methods</span></span>
|<span data-ttu-id="683ac-107">方法</span><span class="sxs-lookup"><span data-stu-id="683ac-107">Method</span></span>|<span data-ttu-id="683ac-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="683ac-108">Return Type</span></span>|<span data-ttu-id="683ac-109">说明</span><span class="sxs-lookup"><span data-stu-id="683ac-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="683ac-110">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="683ac-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="683ac-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="683ac-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="683ac-112">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="683ac-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="683ac-113">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="683ac-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="683ac-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="683ac-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="683ac-115">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="683ac-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="683ac-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="683ac-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="683ac-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="683ac-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="683ac-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="683ac-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="683ac-119">属性</span><span class="sxs-lookup"><span data-stu-id="683ac-119">Properties</span></span>
|<span data-ttu-id="683ac-120">属性</span><span class="sxs-lookup"><span data-stu-id="683ac-120">Property</span></span>|<span data-ttu-id="683ac-121">类型</span><span class="sxs-lookup"><span data-stu-id="683ac-121">Type</span></span>|<span data-ttu-id="683ac-122">说明</span><span class="sxs-lookup"><span data-stu-id="683ac-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="683ac-123">id</span><span class="sxs-lookup"><span data-stu-id="683ac-123">id</span></span>|<span data-ttu-id="683ac-124">字符串</span><span class="sxs-lookup"><span data-stu-id="683ac-124">String</span></span>|<span data-ttu-id="683ac-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="683ac-125">Key of the entity.</span></span>|
|<span data-ttu-id="683ac-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="683ac-126">lastModifiedDateTime</span></span>|<span data-ttu-id="683ac-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="683ac-127">DateTimeOffset</span></span>|<span data-ttu-id="683ac-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="683ac-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="683ac-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="683ac-129">createdDateTime</span></span>|<span data-ttu-id="683ac-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="683ac-130">DateTimeOffset</span></span>|<span data-ttu-id="683ac-131">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="683ac-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="683ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="683ac-132">description</span></span>|<span data-ttu-id="683ac-133">String</span><span class="sxs-lookup"><span data-stu-id="683ac-133">String</span></span>|<span data-ttu-id="683ac-134">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="683ac-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="683ac-135">displayName</span><span class="sxs-lookup"><span data-stu-id="683ac-135">displayName</span></span>|<span data-ttu-id="683ac-136">String</span><span class="sxs-lookup"><span data-stu-id="683ac-136">String</span></span>|<span data-ttu-id="683ac-137">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="683ac-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="683ac-138">version</span><span class="sxs-lookup"><span data-stu-id="683ac-138">version</span></span>|<span data-ttu-id="683ac-139">Int32</span><span class="sxs-lookup"><span data-stu-id="683ac-139">Int32</span></span>|<span data-ttu-id="683ac-140">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="683ac-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="683ac-141">关系</span><span class="sxs-lookup"><span data-stu-id="683ac-141">Relationships</span></span>
|<span data-ttu-id="683ac-142">关系</span><span class="sxs-lookup"><span data-stu-id="683ac-142">Relationship</span></span>|<span data-ttu-id="683ac-143">类型</span><span class="sxs-lookup"><span data-stu-id="683ac-143">Type</span></span>|<span data-ttu-id="683ac-144">说明</span><span class="sxs-lookup"><span data-stu-id="683ac-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="683ac-145">assignments</span><span class="sxs-lookup"><span data-stu-id="683ac-145">assignments</span></span>|<span data-ttu-id="683ac-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="683ac-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="683ac-147">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="683ac-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="683ac-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="683ac-148">deviceStatuses</span></span>|<span data-ttu-id="683ac-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="683ac-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="683ac-150">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="683ac-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="683ac-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="683ac-151">userStatuses</span></span>|<span data-ttu-id="683ac-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="683ac-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="683ac-153">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="683ac-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="683ac-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="683ac-154">deviceStatusOverview</span></span>|[<span data-ttu-id="683ac-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="683ac-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="683ac-156">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="683ac-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="683ac-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="683ac-157">userStatusOverview</span></span>|[<span data-ttu-id="683ac-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="683ac-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="683ac-159">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="683ac-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="683ac-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="683ac-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="683ac-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="683ac-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="683ac-162">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="683ac-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="683ac-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="683ac-163">JSON Representation</span></span>
<span data-ttu-id="683ac-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="683ac-164">Here is a JSON representation of the resource.</span></span>
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



