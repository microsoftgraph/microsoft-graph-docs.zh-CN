---
title: deviceEnrollmentPlatformRestrictionsConfiguration 资源类型
description: 限制用户可以注册的设备类型的设备注册配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 009d43eeab219cc482dd1258c1e33426dec81cb1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940447"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="785ff-103">deviceEnrollmentPlatformRestrictionsConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="785ff-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

> <span data-ttu-id="785ff-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="785ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="785ff-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="785ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="785ff-106">限制用户可以注册的设备类型的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="785ff-106">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="785ff-107">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="785ff-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="785ff-108">方法</span><span class="sxs-lookup"><span data-stu-id="785ff-108">Methods</span></span>
|<span data-ttu-id="785ff-109">方法</span><span class="sxs-lookup"><span data-stu-id="785ff-109">Method</span></span>|<span data-ttu-id="785ff-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="785ff-110">Return Type</span></span>|<span data-ttu-id="785ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="785ff-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="785ff-112">列出 deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="785ff-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="785ff-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="785ff-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="785ff-114">列出 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="785ff-114">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="785ff-115">获取 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="785ff-116">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-116">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="785ff-117">读取 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="785ff-117">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="785ff-118">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="785ff-119">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-119">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="785ff-120">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="785ff-120">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="785ff-121">删除 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="785ff-122">无</span><span class="sxs-lookup"><span data-stu-id="785ff-122">None</span></span>|<span data-ttu-id="785ff-123">删除 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="785ff-123">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="785ff-124">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="785ff-125">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="785ff-125">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="785ff-126">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="785ff-126">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="785ff-127">属性</span><span class="sxs-lookup"><span data-stu-id="785ff-127">Properties</span></span>
|<span data-ttu-id="785ff-128">属性</span><span class="sxs-lookup"><span data-stu-id="785ff-128">Property</span></span>|<span data-ttu-id="785ff-129">类型</span><span class="sxs-lookup"><span data-stu-id="785ff-129">Type</span></span>|<span data-ttu-id="785ff-130">说明</span><span class="sxs-lookup"><span data-stu-id="785ff-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="785ff-131">id</span><span class="sxs-lookup"><span data-stu-id="785ff-131">id</span></span>|<span data-ttu-id="785ff-132">字符串</span><span class="sxs-lookup"><span data-stu-id="785ff-132">String</span></span>|<span data-ttu-id="785ff-133">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="785ff-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-134">displayName</span><span class="sxs-lookup"><span data-stu-id="785ff-134">displayName</span></span>|<span data-ttu-id="785ff-135">String</span><span class="sxs-lookup"><span data-stu-id="785ff-135">String</span></span>|<span data-ttu-id="785ff-136">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="785ff-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-137">说明</span><span class="sxs-lookup"><span data-stu-id="785ff-137">description</span></span>|<span data-ttu-id="785ff-138">String</span><span class="sxs-lookup"><span data-stu-id="785ff-138">String</span></span>|<span data-ttu-id="785ff-139">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="785ff-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-140">priority</span><span class="sxs-lookup"><span data-stu-id="785ff-140">priority</span></span>|<span data-ttu-id="785ff-141">Int32</span><span class="sxs-lookup"><span data-stu-id="785ff-141">Int32</span></span>|<span data-ttu-id="785ff-142">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="785ff-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="785ff-143">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="785ff-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="785ff-144">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="785ff-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="785ff-145">createdDateTime</span></span>|<span data-ttu-id="785ff-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="785ff-146">DateTimeOffset</span></span>|<span data-ttu-id="785ff-147">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="785ff-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="785ff-148">lastModifiedDateTime</span></span>|<span data-ttu-id="785ff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="785ff-149">DateTimeOffset</span></span>|<span data-ttu-id="785ff-150">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="785ff-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-151">version</span><span class="sxs-lookup"><span data-stu-id="785ff-151">version</span></span>|<span data-ttu-id="785ff-152">Int32</span><span class="sxs-lookup"><span data-stu-id="785ff-152">Int32</span></span>|<span data-ttu-id="785ff-153">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="785ff-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="785ff-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-154">iosRestriction</span></span>|[<span data-ttu-id="785ff-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-156">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-156">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="785ff-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-157">windowsRestriction</span></span>|[<span data-ttu-id="785ff-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-159">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-159">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="785ff-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="785ff-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-162">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-162">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="785ff-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-163">androidRestriction</span></span>|[<span data-ttu-id="785ff-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-165">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-165">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="785ff-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="785ff-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-168">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-168">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="785ff-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-169">macRestriction</span></span>|[<span data-ttu-id="785ff-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-171">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-171">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="785ff-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-172">macOSRestriction</span></span>|[<span data-ttu-id="785ff-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="785ff-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="785ff-174">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="785ff-174">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="785ff-175">关系</span><span class="sxs-lookup"><span data-stu-id="785ff-175">Relationships</span></span>
|<span data-ttu-id="785ff-176">关系</span><span class="sxs-lookup"><span data-stu-id="785ff-176">Relationship</span></span>|<span data-ttu-id="785ff-177">类型</span><span class="sxs-lookup"><span data-stu-id="785ff-177">Type</span></span>|<span data-ttu-id="785ff-178">说明</span><span class="sxs-lookup"><span data-stu-id="785ff-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="785ff-179">assignments</span><span class="sxs-lookup"><span data-stu-id="785ff-179">assignments</span></span>|<span data-ttu-id="785ff-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="785ff-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="785ff-181">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="785ff-181">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="785ff-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="785ff-182">JSON Representation</span></span>
<span data-ttu-id="785ff-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="785ff-183">Here is a JSON representation of the resource.</span></span>
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
    "osMaximumVersion": "String"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  }
}
```




