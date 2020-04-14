---
title: deviceEnrollmentPlatformRestrictionsConfiguration 资源类型
description: 限制用户可以注册的设备类型的设备注册配置
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86c8b1a18a8a76b639b5ddc366112f0861a75e72
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455118"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="6da89-103">deviceEnrollmentPlatformRestrictionsConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6da89-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

<span data-ttu-id="6da89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6da89-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6da89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6da89-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6da89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6da89-107">限制用户可以注册的设备类型的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="6da89-107">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="6da89-108">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6da89-108">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6da89-109">方法</span><span class="sxs-lookup"><span data-stu-id="6da89-109">Methods</span></span>
|<span data-ttu-id="6da89-110">方法</span><span class="sxs-lookup"><span data-stu-id="6da89-110">Method</span></span>|<span data-ttu-id="6da89-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6da89-111">Return Type</span></span>|<span data-ttu-id="6da89-112">说明</span><span class="sxs-lookup"><span data-stu-id="6da89-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6da89-113">列出 deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="6da89-113">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="6da89-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6da89-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="6da89-115">列出 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6da89-115">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6da89-116">获取 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-116">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="6da89-117">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-117">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="6da89-118">读取 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6da89-118">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6da89-119">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-119">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="6da89-120">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-120">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="6da89-121">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6da89-121">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6da89-122">删除 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-122">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="6da89-123">无</span><span class="sxs-lookup"><span data-stu-id="6da89-123">None</span></span>|<span data-ttu-id="6da89-124">删除 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6da89-124">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="6da89-125">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-125">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="6da89-126">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da89-126">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="6da89-127">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6da89-127">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6da89-128">属性</span><span class="sxs-lookup"><span data-stu-id="6da89-128">Properties</span></span>
|<span data-ttu-id="6da89-129">属性</span><span class="sxs-lookup"><span data-stu-id="6da89-129">Property</span></span>|<span data-ttu-id="6da89-130">类型</span><span class="sxs-lookup"><span data-stu-id="6da89-130">Type</span></span>|<span data-ttu-id="6da89-131">说明</span><span class="sxs-lookup"><span data-stu-id="6da89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da89-132">id</span><span class="sxs-lookup"><span data-stu-id="6da89-132">id</span></span>|<span data-ttu-id="6da89-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6da89-133">String</span></span>|<span data-ttu-id="6da89-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="6da89-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6da89-135">displayName</span></span>|<span data-ttu-id="6da89-136">String</span><span class="sxs-lookup"><span data-stu-id="6da89-136">String</span></span>|<span data-ttu-id="6da89-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="6da89-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-138">description</span><span class="sxs-lookup"><span data-stu-id="6da89-138">description</span></span>|<span data-ttu-id="6da89-139">String</span><span class="sxs-lookup"><span data-stu-id="6da89-139">String</span></span>|<span data-ttu-id="6da89-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="6da89-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-141">priority</span><span class="sxs-lookup"><span data-stu-id="6da89-141">priority</span></span>|<span data-ttu-id="6da89-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6da89-142">Int32</span></span>|<span data-ttu-id="6da89-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="6da89-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="6da89-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="6da89-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="6da89-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6da89-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6da89-146">createdDateTime</span></span>|<span data-ttu-id="6da89-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da89-147">DateTimeOffset</span></span>|<span data-ttu-id="6da89-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="6da89-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6da89-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6da89-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da89-150">DateTimeOffset</span></span>|<span data-ttu-id="6da89-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="6da89-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-152">version</span><span class="sxs-lookup"><span data-stu-id="6da89-152">version</span></span>|<span data-ttu-id="6da89-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6da89-153">Int32</span></span>|<span data-ttu-id="6da89-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="6da89-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6da89-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-155">iosRestriction</span></span>|[<span data-ttu-id="6da89-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-157">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6da89-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-158">windowsRestriction</span></span>|[<span data-ttu-id="6da89-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-160">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6da89-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="6da89-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-163">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6da89-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-164">androidRestriction</span></span>|[<span data-ttu-id="6da89-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-166">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6da89-167">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="6da89-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-169">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6da89-170">macRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-170">macRestriction</span></span>|[<span data-ttu-id="6da89-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-172">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6da89-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-173">macOSRestriction</span></span>|[<span data-ttu-id="6da89-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6da89-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6da89-175">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="6da89-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da89-176">关系</span><span class="sxs-lookup"><span data-stu-id="6da89-176">Relationships</span></span>
|<span data-ttu-id="6da89-177">关系</span><span class="sxs-lookup"><span data-stu-id="6da89-177">Relationship</span></span>|<span data-ttu-id="6da89-178">类型</span><span class="sxs-lookup"><span data-stu-id="6da89-178">Type</span></span>|<span data-ttu-id="6da89-179">说明</span><span class="sxs-lookup"><span data-stu-id="6da89-179">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da89-180">assignments</span><span class="sxs-lookup"><span data-stu-id="6da89-180">assignments</span></span>|<span data-ttu-id="6da89-181">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6da89-181">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6da89-182">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="6da89-182">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6da89-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6da89-183">JSON Representation</span></span>
<span data-ttu-id="6da89-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6da89-184">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ]
  }
}
```



