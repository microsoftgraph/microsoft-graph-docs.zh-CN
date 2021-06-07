---
title: iosCertificateProfile 资源类型
description: 设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fec643e344f29ea5db889aa172eb81fcd12be5c7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758846"
---
# <a name="ioscertificateprofile-resource-type"></a><span data-ttu-id="4b366-103">iosCertificateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b366-103">iosCertificateProfile resource type</span></span>

<span data-ttu-id="4b366-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b366-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b366-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b366-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="4b366-106">Device Configuration.</span></span>


<span data-ttu-id="4b366-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4b366-108">方法</span><span class="sxs-lookup"><span data-stu-id="4b366-108">Methods</span></span>
|<span data-ttu-id="4b366-109">方法</span><span class="sxs-lookup"><span data-stu-id="4b366-109">Method</span></span>|<span data-ttu-id="4b366-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b366-110">Return Type</span></span>|<span data-ttu-id="4b366-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b366-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b366-112">列出 iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="4b366-112">List iosCertificateProfiles</span></span>](../api/intune-deviceconfig-ioscertificateprofile-list.md)|<span data-ttu-id="4b366-113">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b366-113">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) collection</span></span>|<span data-ttu-id="4b366-114">列出 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b366-114">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>|
|[<span data-ttu-id="4b366-115">获取 iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4b366-115">Get iosCertificateProfile</span></span>](../api/intune-deviceconfig-ioscertificateprofile-get.md)|[<span data-ttu-id="4b366-116">iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4b366-116">iosCertificateProfile</span></span>](../resources/intune-deviceconfig-ioscertificateprofile.md)|<span data-ttu-id="4b366-117">读取 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b366-117">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b366-118">属性</span><span class="sxs-lookup"><span data-stu-id="4b366-118">Properties</span></span>
|<span data-ttu-id="4b366-119">属性</span><span class="sxs-lookup"><span data-stu-id="4b366-119">Property</span></span>|<span data-ttu-id="4b366-120">类型</span><span class="sxs-lookup"><span data-stu-id="4b366-120">Type</span></span>|<span data-ttu-id="4b366-121">说明</span><span class="sxs-lookup"><span data-stu-id="4b366-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b366-122">id</span><span class="sxs-lookup"><span data-stu-id="4b366-122">id</span></span>|<span data-ttu-id="4b366-123">String</span><span class="sxs-lookup"><span data-stu-id="4b366-123">String</span></span>|<span data-ttu-id="4b366-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4b366-124">Key of the entity.</span></span> <span data-ttu-id="4b366-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b366-126">lastModifiedDateTime</span></span>|<span data-ttu-id="4b366-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b366-127">DateTimeOffset</span></span>|<span data-ttu-id="4b366-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4b366-128">DateTime the object was last modified.</span></span> <span data-ttu-id="4b366-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b366-130">createdDateTime</span></span>|<span data-ttu-id="4b366-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b366-131">DateTimeOffset</span></span>|<span data-ttu-id="4b366-132">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4b366-132">DateTime the object was created.</span></span> <span data-ttu-id="4b366-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-134">description</span><span class="sxs-lookup"><span data-stu-id="4b366-134">description</span></span>|<span data-ttu-id="4b366-135">String</span><span class="sxs-lookup"><span data-stu-id="4b366-135">String</span></span>|<span data-ttu-id="4b366-136">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4b366-136">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b366-137">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4b366-138">displayName</span></span>|<span data-ttu-id="4b366-139">String</span><span class="sxs-lookup"><span data-stu-id="4b366-139">String</span></span>|<span data-ttu-id="4b366-140">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4b366-140">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b366-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-142">version</span><span class="sxs-lookup"><span data-stu-id="4b366-142">version</span></span>|<span data-ttu-id="4b366-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4b366-143">Int32</span></span>|<span data-ttu-id="4b366-144">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4b366-144">Version of the device configuration.</span></span> <span data-ttu-id="4b366-145">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b366-146">关系</span><span class="sxs-lookup"><span data-stu-id="4b366-146">Relationships</span></span>
|<span data-ttu-id="4b366-147">关系</span><span class="sxs-lookup"><span data-stu-id="4b366-147">Relationship</span></span>|<span data-ttu-id="4b366-148">类型</span><span class="sxs-lookup"><span data-stu-id="4b366-148">Type</span></span>|<span data-ttu-id="4b366-149">说明</span><span class="sxs-lookup"><span data-stu-id="4b366-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b366-150">assignments</span><span class="sxs-lookup"><span data-stu-id="4b366-150">assignments</span></span>|<span data-ttu-id="4b366-151">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b366-151">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4b366-152">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="4b366-152">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="4b366-153">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="4b366-154">deviceStatuses</span></span>|<span data-ttu-id="4b366-155">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b366-155">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="4b366-156">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="4b366-156">Device configuration installation status by device.</span></span> <span data-ttu-id="4b366-157">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="4b366-158">userStatuses</span></span>|<span data-ttu-id="4b366-159">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b366-159">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="4b366-160">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="4b366-160">Device configuration installation status by user.</span></span> <span data-ttu-id="4b366-161">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-162">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="4b366-162">deviceStatusOverview</span></span>|[<span data-ttu-id="4b366-163">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="4b366-163">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="4b366-164">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-164">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-165">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="4b366-165">userStatusOverview</span></span>|[<span data-ttu-id="4b366-166">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4b366-166">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="4b366-167">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-167">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b366-168">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="4b366-168">deviceSettingStateSummaries</span></span>|<span data-ttu-id="4b366-169">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b366-169">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="4b366-170">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b366-170">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b366-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b366-171">JSON Representation</span></span>
<span data-ttu-id="4b366-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b366-172">Here is a JSON representation of the resource.</span></span>
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




