---
title: iosCertificateProfile 资源类型
description: 设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9363e5b7f0b154b0a2a04d9111acd1ad5b5ab0fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056651"
---
# <a name="ioscertificateprofile-resource-type"></a><span data-ttu-id="0ee59-103">iosCertificateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ee59-103">iosCertificateProfile resource type</span></span>

<span data-ttu-id="0ee59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ee59-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ee59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee59-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="0ee59-106">Device Configuration.</span></span>


<span data-ttu-id="0ee59-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0ee59-108">方法</span><span class="sxs-lookup"><span data-stu-id="0ee59-108">Methods</span></span>
|<span data-ttu-id="0ee59-109">方法</span><span class="sxs-lookup"><span data-stu-id="0ee59-109">Method</span></span>|<span data-ttu-id="0ee59-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ee59-110">Return Type</span></span>|<span data-ttu-id="0ee59-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ee59-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0ee59-112">列出 iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="0ee59-112">List iosCertificateProfiles</span></span>](../api/intune-deviceconfig-ioscertificateprofile-list.md)|<span data-ttu-id="0ee59-113">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ee59-113">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) collection</span></span>|<span data-ttu-id="0ee59-114">列出 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ee59-114">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>|
|[<span data-ttu-id="0ee59-115">获取 iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0ee59-115">Get iosCertificateProfile</span></span>](../api/intune-deviceconfig-ioscertificateprofile-get.md)|[<span data-ttu-id="0ee59-116">iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0ee59-116">iosCertificateProfile</span></span>](../resources/intune-deviceconfig-ioscertificateprofile.md)|<span data-ttu-id="0ee59-117">读取 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ee59-117">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ee59-118">属性</span><span class="sxs-lookup"><span data-stu-id="0ee59-118">Properties</span></span>
|<span data-ttu-id="0ee59-119">属性</span><span class="sxs-lookup"><span data-stu-id="0ee59-119">Property</span></span>|<span data-ttu-id="0ee59-120">类型</span><span class="sxs-lookup"><span data-stu-id="0ee59-120">Type</span></span>|<span data-ttu-id="0ee59-121">说明</span><span class="sxs-lookup"><span data-stu-id="0ee59-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee59-122">id</span><span class="sxs-lookup"><span data-stu-id="0ee59-122">id</span></span>|<span data-ttu-id="0ee59-123">String</span><span class="sxs-lookup"><span data-stu-id="0ee59-123">String</span></span>|<span data-ttu-id="0ee59-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ee59-124">Key of the entity.</span></span> <span data-ttu-id="0ee59-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee59-126">lastModifiedDateTime</span></span>|<span data-ttu-id="0ee59-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee59-127">DateTimeOffset</span></span>|<span data-ttu-id="0ee59-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ee59-128">DateTime the object was last modified.</span></span> <span data-ttu-id="0ee59-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee59-130">createdDateTime</span></span>|<span data-ttu-id="0ee59-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee59-131">DateTimeOffset</span></span>|<span data-ttu-id="0ee59-132">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ee59-132">DateTime the object was created.</span></span> <span data-ttu-id="0ee59-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-134">description</span><span class="sxs-lookup"><span data-stu-id="0ee59-134">description</span></span>|<span data-ttu-id="0ee59-135">String</span><span class="sxs-lookup"><span data-stu-id="0ee59-135">String</span></span>|<span data-ttu-id="0ee59-136">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0ee59-136">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ee59-137">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee59-138">displayName</span></span>|<span data-ttu-id="0ee59-139">String</span><span class="sxs-lookup"><span data-stu-id="0ee59-139">String</span></span>|<span data-ttu-id="0ee59-140">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0ee59-140">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ee59-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-142">version</span><span class="sxs-lookup"><span data-stu-id="0ee59-142">version</span></span>|<span data-ttu-id="0ee59-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0ee59-143">Int32</span></span>|<span data-ttu-id="0ee59-144">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0ee59-144">Version of the device configuration.</span></span> <span data-ttu-id="0ee59-145">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ee59-146">关系</span><span class="sxs-lookup"><span data-stu-id="0ee59-146">Relationships</span></span>
|<span data-ttu-id="0ee59-147">关系</span><span class="sxs-lookup"><span data-stu-id="0ee59-147">Relationship</span></span>|<span data-ttu-id="0ee59-148">类型</span><span class="sxs-lookup"><span data-stu-id="0ee59-148">Type</span></span>|<span data-ttu-id="0ee59-149">说明</span><span class="sxs-lookup"><span data-stu-id="0ee59-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee59-150">assignments</span><span class="sxs-lookup"><span data-stu-id="0ee59-150">assignments</span></span>|<span data-ttu-id="0ee59-151">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ee59-151">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0ee59-152">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0ee59-152">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0ee59-153">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0ee59-154">deviceStatuses</span></span>|<span data-ttu-id="0ee59-155">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ee59-155">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0ee59-156">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0ee59-156">Device configuration installation status by device.</span></span> <span data-ttu-id="0ee59-157">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0ee59-158">userStatuses</span></span>|<span data-ttu-id="0ee59-159">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ee59-159">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0ee59-160">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0ee59-160">Device configuration installation status by user.</span></span> <span data-ttu-id="0ee59-161">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-162">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0ee59-162">deviceStatusOverview</span></span>|[<span data-ttu-id="0ee59-163">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0ee59-163">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0ee59-164">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-164">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-165">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0ee59-165">userStatusOverview</span></span>|[<span data-ttu-id="0ee59-166">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0ee59-166">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0ee59-167">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-167">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ee59-168">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0ee59-168">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0ee59-169">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ee59-169">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0ee59-170">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ee59-170">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ee59-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ee59-171">JSON Representation</span></span>
<span data-ttu-id="0ee59-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee59-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```









