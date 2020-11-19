---
title: deviceEnrollmentPlatformRestrictionsConfiguration 资源类型
description: 限制用户可以注册的设备类型的设备注册配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5fd3c392bc752db695611d9a55c1fe5cd634ec64
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266555"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="4cde5-103">deviceEnrollmentPlatformRestrictionsConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cde5-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

<span data-ttu-id="4cde5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cde5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cde5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4cde5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cde5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4cde5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cde5-107">限制用户可以注册的设备类型的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="4cde5-107">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="4cde5-108">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cde5-108">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4cde5-109">方法</span><span class="sxs-lookup"><span data-stu-id="4cde5-109">Methods</span></span>
|<span data-ttu-id="4cde5-110">方法</span><span class="sxs-lookup"><span data-stu-id="4cde5-110">Method</span></span>|<span data-ttu-id="4cde5-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="4cde5-111">Return Type</span></span>|<span data-ttu-id="4cde5-112">说明</span><span class="sxs-lookup"><span data-stu-id="4cde5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4cde5-113">列出 deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="4cde5-113">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="4cde5-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4cde5-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="4cde5-115">列出 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4cde5-115">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4cde5-116">获取 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-116">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="4cde5-117">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-117">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="4cde5-118">读取 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4cde5-118">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="4cde5-119">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-119">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="4cde5-120">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-120">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="4cde5-121">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4cde5-121">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="4cde5-122">删除 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-122">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="4cde5-123">无</span><span class="sxs-lookup"><span data-stu-id="4cde5-123">None</span></span>|<span data-ttu-id="4cde5-124">删除 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="4cde5-124">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="4cde5-125">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-125">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="4cde5-126">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cde5-126">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="4cde5-127">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4cde5-127">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4cde5-128">属性</span><span class="sxs-lookup"><span data-stu-id="4cde5-128">Properties</span></span>
|<span data-ttu-id="4cde5-129">属性</span><span class="sxs-lookup"><span data-stu-id="4cde5-129">Property</span></span>|<span data-ttu-id="4cde5-130">类型</span><span class="sxs-lookup"><span data-stu-id="4cde5-130">Type</span></span>|<span data-ttu-id="4cde5-131">说明</span><span class="sxs-lookup"><span data-stu-id="4cde5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cde5-132">id</span><span class="sxs-lookup"><span data-stu-id="4cde5-132">id</span></span>|<span data-ttu-id="4cde5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4cde5-133">String</span></span>|<span data-ttu-id="4cde5-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="4cde5-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4cde5-135">displayName</span></span>|<span data-ttu-id="4cde5-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4cde5-136">String</span></span>|<span data-ttu-id="4cde5-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="4cde5-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-138">description</span><span class="sxs-lookup"><span data-stu-id="4cde5-138">description</span></span>|<span data-ttu-id="4cde5-139">字符串</span><span class="sxs-lookup"><span data-stu-id="4cde5-139">String</span></span>|<span data-ttu-id="4cde5-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="4cde5-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-141">priority</span><span class="sxs-lookup"><span data-stu-id="4cde5-141">priority</span></span>|<span data-ttu-id="4cde5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4cde5-142">Int32</span></span>|<span data-ttu-id="4cde5-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="4cde5-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="4cde5-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="4cde5-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="4cde5-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cde5-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cde5-146">createdDateTime</span></span>|<span data-ttu-id="4cde5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cde5-147">DateTimeOffset</span></span>|<span data-ttu-id="4cde5-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="4cde5-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cde5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4cde5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cde5-150">DateTimeOffset</span></span>|<span data-ttu-id="4cde5-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="4cde5-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-152">version</span><span class="sxs-lookup"><span data-stu-id="4cde5-152">version</span></span>|<span data-ttu-id="4cde5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4cde5-153">Int32</span></span>|<span data-ttu-id="4cde5-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="4cde5-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4cde5-155">roleScopeTagIds</span></span>|<span data-ttu-id="4cde5-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="4cde5-156">String collection</span></span>|<span data-ttu-id="4cde5-157">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="4cde5-157">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="4cde5-158">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cde5-158">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4cde5-159">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-159">iosRestriction</span></span>|[<span data-ttu-id="4cde5-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-161">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-161">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-162">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-162">windowsRestriction</span></span>|[<span data-ttu-id="4cde5-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-164">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-164">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-165">windowsHomeSkuRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-165">windowsHomeSkuRestriction</span></span>|[<span data-ttu-id="4cde5-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-167">基于平台、平台操作系统版本和设备所有权的 Windows 主页 Sku 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-167">Windows Home Sku restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-168">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-168">windowsMobileRestriction</span></span>|[<span data-ttu-id="4cde5-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-170">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-170">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-171">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-171">androidRestriction</span></span>|[<span data-ttu-id="4cde5-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-173">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-173">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-174">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-174">androidForWorkRestriction</span></span>|[<span data-ttu-id="4cde5-175">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-175">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-176">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-176">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-177">aospRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-177">aospRestriction</span></span>|[<span data-ttu-id="4cde5-178">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-178">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-179">基于平台、平台操作系统版本和设备所有权的 AOSP 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-179">AOSP restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-180">macRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-180">macRestriction</span></span>|[<span data-ttu-id="4cde5-181">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-181">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-182">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-182">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="4cde5-183">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-183">macOSRestriction</span></span>|[<span data-ttu-id="4cde5-184">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4cde5-184">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="4cde5-185">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="4cde5-185">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cde5-186">关系</span><span class="sxs-lookup"><span data-stu-id="4cde5-186">Relationships</span></span>
|<span data-ttu-id="4cde5-187">关系</span><span class="sxs-lookup"><span data-stu-id="4cde5-187">Relationship</span></span>|<span data-ttu-id="4cde5-188">类型</span><span class="sxs-lookup"><span data-stu-id="4cde5-188">Type</span></span>|<span data-ttu-id="4cde5-189">说明</span><span class="sxs-lookup"><span data-stu-id="4cde5-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cde5-190">assignments</span><span class="sxs-lookup"><span data-stu-id="4cde5-190">assignments</span></span>|<span data-ttu-id="4cde5-191">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4cde5-191">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4cde5-192">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="4cde5-192">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cde5-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cde5-193">JSON Representation</span></span>
<span data-ttu-id="4cde5-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cde5-194">Here is a JSON representation of the resource.</span></span>
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
    ],
    "blockedSkus": [
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
    ],
    "blockedSkus": [
      "String"
    ]
  },
  "windowsHomeSkuRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ],
    "blockedSkus": [
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
    ],
    "blockedSkus": [
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
    ],
    "blockedSkus": [
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
    ],
    "blockedSkus": [
      "String"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ],
    "blockedSkus": [
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
    ],
    "blockedSkus": [
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
    ],
    "blockedSkus": [
      "String"
    ]
  }
}
```




