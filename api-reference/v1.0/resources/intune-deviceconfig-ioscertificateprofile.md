---
title: iosCertificateProfile 资源类型
description: 设备配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e3708e482fff1ac9287c80eefacc57b8d38c9be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532505"
---
# <a name="ioscertificateprofile-resource-type"></a><span data-ttu-id="c6e46-103">iosCertificateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6e46-103">iosCertificateProfile resource type</span></span>

<span data-ttu-id="c6e46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6e46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6e46-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6e46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6e46-106">设备配置。</span><span class="sxs-lookup"><span data-stu-id="c6e46-106">Device Configuration.</span></span>


<span data-ttu-id="c6e46-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c6e46-108">Methods</span><span class="sxs-lookup"><span data-stu-id="c6e46-108">Methods</span></span>
|<span data-ttu-id="c6e46-109">方法</span><span class="sxs-lookup"><span data-stu-id="c6e46-109">Method</span></span>|<span data-ttu-id="c6e46-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6e46-110">Return Type</span></span>|<span data-ttu-id="c6e46-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6e46-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6e46-112">列出 iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="c6e46-112">List iosCertificateProfiles</span></span>](../api/intune-deviceconfig-ioscertificateprofile-list.md)|<span data-ttu-id="c6e46-113">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6e46-113">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) collection</span></span>|<span data-ttu-id="c6e46-114">列出 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6e46-114">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>|
|[<span data-ttu-id="c6e46-115">获取 iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c6e46-115">Get iosCertificateProfile</span></span>](../api/intune-deviceconfig-ioscertificateprofile-get.md)|[<span data-ttu-id="c6e46-116">iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c6e46-116">iosCertificateProfile</span></span>](../resources/intune-deviceconfig-ioscertificateprofile.md)|<span data-ttu-id="c6e46-117">读取 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6e46-117">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6e46-118">属性</span><span class="sxs-lookup"><span data-stu-id="c6e46-118">Properties</span></span>
|<span data-ttu-id="c6e46-119">属性</span><span class="sxs-lookup"><span data-stu-id="c6e46-119">Property</span></span>|<span data-ttu-id="c6e46-120">类型</span><span class="sxs-lookup"><span data-stu-id="c6e46-120">Type</span></span>|<span data-ttu-id="c6e46-121">说明</span><span class="sxs-lookup"><span data-stu-id="c6e46-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e46-122">id</span><span class="sxs-lookup"><span data-stu-id="c6e46-122">id</span></span>|<span data-ttu-id="c6e46-123">字符串</span><span class="sxs-lookup"><span data-stu-id="c6e46-123">String</span></span>|<span data-ttu-id="c6e46-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c6e46-124">Key of the entity.</span></span> <span data-ttu-id="c6e46-125">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6e46-126">lastModifiedDateTime</span></span>|<span data-ttu-id="c6e46-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6e46-127">DateTimeOffset</span></span>|<span data-ttu-id="c6e46-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c6e46-128">DateTime the object was last modified.</span></span> <span data-ttu-id="c6e46-129">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6e46-130">createdDateTime</span></span>|<span data-ttu-id="c6e46-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6e46-131">DateTimeOffset</span></span>|<span data-ttu-id="c6e46-132">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c6e46-132">DateTime the object was created.</span></span> <span data-ttu-id="c6e46-133">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-134">说明</span><span class="sxs-lookup"><span data-stu-id="c6e46-134">description</span></span>|<span data-ttu-id="c6e46-135">String</span><span class="sxs-lookup"><span data-stu-id="c6e46-135">String</span></span>|<span data-ttu-id="c6e46-136">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c6e46-136">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c6e46-137">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c6e46-138">displayName</span></span>|<span data-ttu-id="c6e46-139">String</span><span class="sxs-lookup"><span data-stu-id="c6e46-139">String</span></span>|<span data-ttu-id="c6e46-140">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c6e46-140">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c6e46-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-142">version</span><span class="sxs-lookup"><span data-stu-id="c6e46-142">version</span></span>|<span data-ttu-id="c6e46-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c6e46-143">Int32</span></span>|<span data-ttu-id="c6e46-144">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c6e46-144">Version of the device configuration.</span></span> <span data-ttu-id="c6e46-145">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6e46-146">关系</span><span class="sxs-lookup"><span data-stu-id="c6e46-146">Relationships</span></span>
|<span data-ttu-id="c6e46-147">关系</span><span class="sxs-lookup"><span data-stu-id="c6e46-147">Relationship</span></span>|<span data-ttu-id="c6e46-148">类型</span><span class="sxs-lookup"><span data-stu-id="c6e46-148">Type</span></span>|<span data-ttu-id="c6e46-149">说明</span><span class="sxs-lookup"><span data-stu-id="c6e46-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e46-150">assignments</span><span class="sxs-lookup"><span data-stu-id="c6e46-150">assignments</span></span>|<span data-ttu-id="c6e46-151">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6e46-151">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c6e46-152">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c6e46-152">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="c6e46-153">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c6e46-154">deviceStatuses</span></span>|<span data-ttu-id="c6e46-155">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6e46-155">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c6e46-156">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c6e46-156">Device configuration installation status by device.</span></span> <span data-ttu-id="c6e46-157">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c6e46-158">userStatuses</span></span>|<span data-ttu-id="c6e46-159">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6e46-159">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c6e46-160">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c6e46-160">Device configuration installation status by user.</span></span> <span data-ttu-id="c6e46-161">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-162">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c6e46-162">deviceStatusOverview</span></span>|[<span data-ttu-id="c6e46-163">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c6e46-163">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c6e46-164">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-164">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-165">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c6e46-165">userStatusOverview</span></span>|[<span data-ttu-id="c6e46-166">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c6e46-166">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c6e46-167">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-167">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6e46-168">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c6e46-168">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c6e46-169">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6e46-169">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c6e46-170">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6e46-170">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6e46-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6e46-171">JSON Representation</span></span>
<span data-ttu-id="c6e46-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6e46-172">Here is a JSON representation of the resource.</span></span>
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




