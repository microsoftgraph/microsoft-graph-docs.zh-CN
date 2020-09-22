---
title: deviceConfiguration 资源类型
description: 设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffcd58ee7dc23554908749d7c257fa8acccffe94
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075026"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="c9168-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9168-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="c9168-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9168-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9168-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9168-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9168-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="c9168-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c9168-107">方法</span><span class="sxs-lookup"><span data-stu-id="c9168-107">Methods</span></span>
|<span data-ttu-id="c9168-108">方法</span><span class="sxs-lookup"><span data-stu-id="c9168-108">Method</span></span>|<span data-ttu-id="c9168-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9168-109">Return Type</span></span>|<span data-ttu-id="c9168-110">说明</span><span class="sxs-lookup"><span data-stu-id="c9168-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9168-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="c9168-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="c9168-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9168-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="c9168-113">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9168-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c9168-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9168-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="c9168-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9168-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="c9168-116">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9168-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c9168-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="c9168-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="c9168-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9168-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c9168-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9168-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c9168-120">属性</span><span class="sxs-lookup"><span data-stu-id="c9168-120">Properties</span></span>
|<span data-ttu-id="c9168-121">属性</span><span class="sxs-lookup"><span data-stu-id="c9168-121">Property</span></span>|<span data-ttu-id="c9168-122">类型</span><span class="sxs-lookup"><span data-stu-id="c9168-122">Type</span></span>|<span data-ttu-id="c9168-123">说明</span><span class="sxs-lookup"><span data-stu-id="c9168-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9168-124">id</span><span class="sxs-lookup"><span data-stu-id="c9168-124">id</span></span>|<span data-ttu-id="c9168-125">String</span><span class="sxs-lookup"><span data-stu-id="c9168-125">String</span></span>|<span data-ttu-id="c9168-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9168-126">Key of the entity.</span></span>|
|<span data-ttu-id="c9168-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9168-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c9168-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9168-128">DateTimeOffset</span></span>|<span data-ttu-id="c9168-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9168-129">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c9168-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9168-130">createdDateTime</span></span>|<span data-ttu-id="c9168-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9168-131">DateTimeOffset</span></span>|<span data-ttu-id="c9168-132">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9168-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="c9168-133">description</span><span class="sxs-lookup"><span data-stu-id="c9168-133">description</span></span>|<span data-ttu-id="c9168-134">String</span><span class="sxs-lookup"><span data-stu-id="c9168-134">String</span></span>|<span data-ttu-id="c9168-135">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="c9168-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c9168-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c9168-136">displayName</span></span>|<span data-ttu-id="c9168-137">String</span><span class="sxs-lookup"><span data-stu-id="c9168-137">String</span></span>|<span data-ttu-id="c9168-138">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="c9168-138">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c9168-139">version</span><span class="sxs-lookup"><span data-stu-id="c9168-139">version</span></span>|<span data-ttu-id="c9168-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c9168-140">Int32</span></span>|<span data-ttu-id="c9168-141">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9168-141">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9168-142">关系</span><span class="sxs-lookup"><span data-stu-id="c9168-142">Relationships</span></span>
|<span data-ttu-id="c9168-143">关系</span><span class="sxs-lookup"><span data-stu-id="c9168-143">Relationship</span></span>|<span data-ttu-id="c9168-144">类型</span><span class="sxs-lookup"><span data-stu-id="c9168-144">Type</span></span>|<span data-ttu-id="c9168-145">说明</span><span class="sxs-lookup"><span data-stu-id="c9168-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9168-146">assignments</span><span class="sxs-lookup"><span data-stu-id="c9168-146">assignments</span></span>|<span data-ttu-id="c9168-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9168-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c9168-148">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c9168-148">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="c9168-149">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c9168-149">deviceStatuses</span></span>|<span data-ttu-id="c9168-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9168-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c9168-151">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c9168-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="c9168-152">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c9168-152">userStatuses</span></span>|<span data-ttu-id="c9168-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9168-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c9168-154">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c9168-154">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="c9168-155">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c9168-155">deviceStatusOverview</span></span>|[<span data-ttu-id="c9168-156">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c9168-156">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c9168-157">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="c9168-157">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="c9168-158">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c9168-158">userStatusOverview</span></span>|[<span data-ttu-id="c9168-159">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c9168-159">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c9168-160">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="c9168-160">Device Configuration users status overview</span></span>|
|<span data-ttu-id="c9168-161">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c9168-161">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c9168-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9168-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c9168-163">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="c9168-163">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9168-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9168-164">JSON Representation</span></span>
<span data-ttu-id="c9168-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9168-165">Here is a JSON representation of the resource.</span></span>
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









