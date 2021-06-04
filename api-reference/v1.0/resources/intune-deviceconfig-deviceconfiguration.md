---
title: deviceConfiguration 资源类型
description: 设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82f1de5e835ceba2a15559411a07638dee2602bd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742907"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="5eb18-103">deviceConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eb18-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="5eb18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eb18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5eb18-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5eb18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eb18-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="5eb18-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="5eb18-107">Methods</span><span class="sxs-lookup"><span data-stu-id="5eb18-107">Methods</span></span>
|<span data-ttu-id="5eb18-108">方法</span><span class="sxs-lookup"><span data-stu-id="5eb18-108">Method</span></span>|<span data-ttu-id="5eb18-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5eb18-109">Return Type</span></span>|<span data-ttu-id="5eb18-110">Description</span><span class="sxs-lookup"><span data-stu-id="5eb18-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5eb18-111">List deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="5eb18-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="5eb18-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb18-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="5eb18-113">列出 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eb18-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="5eb18-114">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5eb18-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="5eb18-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5eb18-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="5eb18-116">读取 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eb18-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="5eb18-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="5eb18-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="5eb18-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb18-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5eb18-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5eb18-119">Not yet documented</span></span>|
|[<span data-ttu-id="5eb18-120">getOmaSettingPlainTextValue 函数</span><span class="sxs-lookup"><span data-stu-id="5eb18-120">getOmaSettingPlainTextValue function</span></span>](../api/intune-deviceconfig-deviceconfiguration-getomasettingplaintextvalue.md)|<span data-ttu-id="5eb18-121">String</span><span class="sxs-lookup"><span data-stu-id="5eb18-121">String</span></span>|<span data-ttu-id="5eb18-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5eb18-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5eb18-123">属性</span><span class="sxs-lookup"><span data-stu-id="5eb18-123">Properties</span></span>
|<span data-ttu-id="5eb18-124">属性</span><span class="sxs-lookup"><span data-stu-id="5eb18-124">Property</span></span>|<span data-ttu-id="5eb18-125">类型</span><span class="sxs-lookup"><span data-stu-id="5eb18-125">Type</span></span>|<span data-ttu-id="5eb18-126">说明</span><span class="sxs-lookup"><span data-stu-id="5eb18-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb18-127">id</span><span class="sxs-lookup"><span data-stu-id="5eb18-127">id</span></span>|<span data-ttu-id="5eb18-128">String</span><span class="sxs-lookup"><span data-stu-id="5eb18-128">String</span></span>|<span data-ttu-id="5eb18-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5eb18-129">Key of the entity.</span></span>|
|<span data-ttu-id="5eb18-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb18-130">lastModifiedDateTime</span></span>|<span data-ttu-id="5eb18-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb18-131">DateTimeOffset</span></span>|<span data-ttu-id="5eb18-132">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5eb18-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5eb18-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb18-133">createdDateTime</span></span>|<span data-ttu-id="5eb18-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb18-134">DateTimeOffset</span></span>|<span data-ttu-id="5eb18-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5eb18-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="5eb18-136">说明</span><span class="sxs-lookup"><span data-stu-id="5eb18-136">description</span></span>|<span data-ttu-id="5eb18-137">String</span><span class="sxs-lookup"><span data-stu-id="5eb18-137">String</span></span>|<span data-ttu-id="5eb18-138">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="5eb18-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="5eb18-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5eb18-139">displayName</span></span>|<span data-ttu-id="5eb18-140">String</span><span class="sxs-lookup"><span data-stu-id="5eb18-140">String</span></span>|<span data-ttu-id="5eb18-141">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="5eb18-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5eb18-142">version</span><span class="sxs-lookup"><span data-stu-id="5eb18-142">version</span></span>|<span data-ttu-id="5eb18-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5eb18-143">Int32</span></span>|<span data-ttu-id="5eb18-144">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5eb18-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eb18-145">关系</span><span class="sxs-lookup"><span data-stu-id="5eb18-145">Relationships</span></span>
|<span data-ttu-id="5eb18-146">关系</span><span class="sxs-lookup"><span data-stu-id="5eb18-146">Relationship</span></span>|<span data-ttu-id="5eb18-147">类型</span><span class="sxs-lookup"><span data-stu-id="5eb18-147">Type</span></span>|<span data-ttu-id="5eb18-148">Description</span><span class="sxs-lookup"><span data-stu-id="5eb18-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb18-149">assignments</span><span class="sxs-lookup"><span data-stu-id="5eb18-149">assignments</span></span>|<span data-ttu-id="5eb18-150">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb18-150">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5eb18-151">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="5eb18-151">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="5eb18-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5eb18-152">deviceStatuses</span></span>|<span data-ttu-id="5eb18-153">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb18-153">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="5eb18-154">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="5eb18-154">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="5eb18-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="5eb18-155">userStatuses</span></span>|<span data-ttu-id="5eb18-156">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb18-156">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="5eb18-157">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="5eb18-157">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="5eb18-158">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5eb18-158">deviceStatusOverview</span></span>|[<span data-ttu-id="5eb18-159">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5eb18-159">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="5eb18-160">设备配置设备状态概述</span><span class="sxs-lookup"><span data-stu-id="5eb18-160">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="5eb18-161">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5eb18-161">userStatusOverview</span></span>|[<span data-ttu-id="5eb18-162">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="5eb18-162">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="5eb18-163">设备配置用户状态概述</span><span class="sxs-lookup"><span data-stu-id="5eb18-163">Device Configuration users status overview</span></span>|
|<span data-ttu-id="5eb18-164">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="5eb18-164">deviceSettingStateSummaries</span></span>|<span data-ttu-id="5eb18-165">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb18-165">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="5eb18-166">设备配置设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="5eb18-166">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5eb18-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eb18-167">JSON Representation</span></span>
<span data-ttu-id="5eb18-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eb18-168">Here is a JSON representation of the resource.</span></span>
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




