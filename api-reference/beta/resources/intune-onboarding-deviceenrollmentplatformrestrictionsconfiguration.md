---
title: deviceEnrollmentPlatformRestrictionsConfiguration 资源类型
description: 限制用户可以注册的设备类型的设备注册配置
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e359388c99084c6b9544a3d1874ec11a6315596e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177672"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="37c96-103">deviceEnrollmentPlatformRestrictionsConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="37c96-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

<span data-ttu-id="37c96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37c96-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37c96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37c96-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37c96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37c96-107">限制用户可以注册的设备类型的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="37c96-107">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="37c96-108">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c96-108">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="37c96-109">方法</span><span class="sxs-lookup"><span data-stu-id="37c96-109">Methods</span></span>
|<span data-ttu-id="37c96-110">方法</span><span class="sxs-lookup"><span data-stu-id="37c96-110">Method</span></span>|<span data-ttu-id="37c96-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="37c96-111">Return Type</span></span>|<span data-ttu-id="37c96-112">说明</span><span class="sxs-lookup"><span data-stu-id="37c96-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37c96-113">列出 deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="37c96-113">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="37c96-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37c96-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="37c96-115">列出 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="37c96-115">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="37c96-116">获取 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-116">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="37c96-117">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-117">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="37c96-118">读取 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="37c96-118">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="37c96-119">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-119">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="37c96-120">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-120">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="37c96-121">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37c96-121">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="37c96-122">删除 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-122">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="37c96-123">无</span><span class="sxs-lookup"><span data-stu-id="37c96-123">None</span></span>|<span data-ttu-id="37c96-124">删除 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="37c96-124">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="37c96-125">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-125">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="37c96-126">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c96-126">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="37c96-127">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="37c96-127">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37c96-128">属性</span><span class="sxs-lookup"><span data-stu-id="37c96-128">Properties</span></span>
|<span data-ttu-id="37c96-129">属性</span><span class="sxs-lookup"><span data-stu-id="37c96-129">Property</span></span>|<span data-ttu-id="37c96-130">类型</span><span class="sxs-lookup"><span data-stu-id="37c96-130">Type</span></span>|<span data-ttu-id="37c96-131">说明</span><span class="sxs-lookup"><span data-stu-id="37c96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c96-132">id</span><span class="sxs-lookup"><span data-stu-id="37c96-132">id</span></span>|<span data-ttu-id="37c96-133">字符串</span><span class="sxs-lookup"><span data-stu-id="37c96-133">String</span></span>|<span data-ttu-id="37c96-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="37c96-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-135">displayName</span><span class="sxs-lookup"><span data-stu-id="37c96-135">displayName</span></span>|<span data-ttu-id="37c96-136">String</span><span class="sxs-lookup"><span data-stu-id="37c96-136">String</span></span>|<span data-ttu-id="37c96-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="37c96-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-138">说明</span><span class="sxs-lookup"><span data-stu-id="37c96-138">description</span></span>|<span data-ttu-id="37c96-139">String</span><span class="sxs-lookup"><span data-stu-id="37c96-139">String</span></span>|<span data-ttu-id="37c96-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="37c96-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-141">priority</span><span class="sxs-lookup"><span data-stu-id="37c96-141">priority</span></span>|<span data-ttu-id="37c96-142">Int32</span><span class="sxs-lookup"><span data-stu-id="37c96-142">Int32</span></span>|<span data-ttu-id="37c96-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="37c96-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="37c96-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="37c96-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="37c96-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c96-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37c96-146">createdDateTime</span></span>|<span data-ttu-id="37c96-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c96-147">DateTimeOffset</span></span>|<span data-ttu-id="37c96-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="37c96-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37c96-149">lastModifiedDateTime</span></span>|<span data-ttu-id="37c96-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c96-150">DateTimeOffset</span></span>|<span data-ttu-id="37c96-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="37c96-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-152">version</span><span class="sxs-lookup"><span data-stu-id="37c96-152">version</span></span>|<span data-ttu-id="37c96-153">Int32</span><span class="sxs-lookup"><span data-stu-id="37c96-153">Int32</span></span>|<span data-ttu-id="37c96-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="37c96-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37c96-155">roleScopeTagIds</span></span>|<span data-ttu-id="37c96-156">字符串集合</span><span class="sxs-lookup"><span data-stu-id="37c96-156">String collection</span></span>|<span data-ttu-id="37c96-157">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="37c96-157">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="37c96-158">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c96-158">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="37c96-159">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-159">iosRestriction</span></span>|[<span data-ttu-id="37c96-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-161">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-161">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="37c96-162">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-162">windowsRestriction</span></span>|[<span data-ttu-id="37c96-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-164">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-164">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="37c96-165">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-165">windowsMobileRestriction</span></span>|[<span data-ttu-id="37c96-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-167">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-167">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="37c96-168">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-168">androidRestriction</span></span>|[<span data-ttu-id="37c96-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-170">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-170">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="37c96-171">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-171">androidForWorkRestriction</span></span>|[<span data-ttu-id="37c96-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-173">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-173">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="37c96-174">macRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-174">macRestriction</span></span>|[<span data-ttu-id="37c96-175">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-175">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-176">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-176">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="37c96-177">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-177">macOSRestriction</span></span>|[<span data-ttu-id="37c96-178">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="37c96-178">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="37c96-179">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="37c96-179">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="37c96-180">关系</span><span class="sxs-lookup"><span data-stu-id="37c96-180">Relationships</span></span>
|<span data-ttu-id="37c96-181">关系</span><span class="sxs-lookup"><span data-stu-id="37c96-181">Relationship</span></span>|<span data-ttu-id="37c96-182">类型</span><span class="sxs-lookup"><span data-stu-id="37c96-182">Type</span></span>|<span data-ttu-id="37c96-183">说明</span><span class="sxs-lookup"><span data-stu-id="37c96-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c96-184">assignments</span><span class="sxs-lookup"><span data-stu-id="37c96-184">assignments</span></span>|<span data-ttu-id="37c96-185">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37c96-185">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="37c96-186">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="37c96-186">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37c96-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37c96-187">JSON Representation</span></span>
<span data-ttu-id="37c96-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37c96-188">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
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



