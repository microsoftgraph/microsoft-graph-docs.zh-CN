---
title: deviceEnrollmentPlatformRestrictionsConfiguration 资源类型
description: 设备注册 限制用户可以注册的设备类型的配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 47d1265f6f593bdab8787fa14769e1d55cad023f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751606"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="2abb2-103">deviceEnrollmentPlatformRestrictionsConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="2abb2-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

<span data-ttu-id="2abb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2abb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2abb2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2abb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2abb2-106">设备注册 限制用户可以注册的设备类型的配置</span><span class="sxs-lookup"><span data-stu-id="2abb2-106">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="2abb2-107">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2abb2-108">Methods</span><span class="sxs-lookup"><span data-stu-id="2abb2-108">Methods</span></span>
|<span data-ttu-id="2abb2-109">方法</span><span class="sxs-lookup"><span data-stu-id="2abb2-109">Method</span></span>|<span data-ttu-id="2abb2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2abb2-110">Return Type</span></span>|<span data-ttu-id="2abb2-111">Description</span><span class="sxs-lookup"><span data-stu-id="2abb2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2abb2-112">列出 deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="2abb2-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="2abb2-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2abb2-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="2abb2-114">列出 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2abb2-114">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2abb2-115">获取 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="2abb2-116">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-116">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="2abb2-117">读取 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2abb2-117">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2abb2-118">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="2abb2-119">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-119">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="2abb2-120">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2abb2-120">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2abb2-121">删除 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="2abb2-122">无</span><span class="sxs-lookup"><span data-stu-id="2abb2-122">None</span></span>|<span data-ttu-id="2abb2-123">删除 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2abb2-123">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="2abb2-124">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="2abb2-125">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2abb2-125">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="2abb2-126">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2abb2-126">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2abb2-127">属性</span><span class="sxs-lookup"><span data-stu-id="2abb2-127">Properties</span></span>
|<span data-ttu-id="2abb2-128">属性</span><span class="sxs-lookup"><span data-stu-id="2abb2-128">Property</span></span>|<span data-ttu-id="2abb2-129">类型</span><span class="sxs-lookup"><span data-stu-id="2abb2-129">Type</span></span>|<span data-ttu-id="2abb2-130">说明</span><span class="sxs-lookup"><span data-stu-id="2abb2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2abb2-131">id</span><span class="sxs-lookup"><span data-stu-id="2abb2-131">id</span></span>|<span data-ttu-id="2abb2-132">String</span><span class="sxs-lookup"><span data-stu-id="2abb2-132">String</span></span>|<span data-ttu-id="2abb2-133">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2abb2-134">displayName</span></span>|<span data-ttu-id="2abb2-135">String</span><span class="sxs-lookup"><span data-stu-id="2abb2-135">String</span></span>|<span data-ttu-id="2abb2-136">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-137">说明</span><span class="sxs-lookup"><span data-stu-id="2abb2-137">description</span></span>|<span data-ttu-id="2abb2-138">String</span><span class="sxs-lookup"><span data-stu-id="2abb2-138">String</span></span>|<span data-ttu-id="2abb2-139">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-140">priority</span><span class="sxs-lookup"><span data-stu-id="2abb2-140">priority</span></span>|<span data-ttu-id="2abb2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2abb2-141">Int32</span></span>|<span data-ttu-id="2abb2-142">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="2abb2-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="2abb2-143">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="2abb2-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="2abb2-144">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2abb2-145">createdDateTime</span></span>|<span data-ttu-id="2abb2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2abb2-146">DateTimeOffset</span></span>|<span data-ttu-id="2abb2-147">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2abb2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2abb2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2abb2-149">DateTimeOffset</span></span>|<span data-ttu-id="2abb2-150">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-151">version</span><span class="sxs-lookup"><span data-stu-id="2abb2-151">version</span></span>|<span data-ttu-id="2abb2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2abb2-152">Int32</span></span>|<span data-ttu-id="2abb2-153">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2abb2-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-154">iosRestriction</span></span>|[<span data-ttu-id="2abb2-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2abb2-156">基于平台、平台操作系统版本和设备所有权的 IOS 限制</span><span class="sxs-lookup"><span data-stu-id="2abb2-156">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2abb2-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-157">windowsRestriction</span></span>|[<span data-ttu-id="2abb2-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2abb2-159">Windows平台、平台操作系统版本和设备所有权的限制</span><span class="sxs-lookup"><span data-stu-id="2abb2-159">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2abb2-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="2abb2-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2abb2-162">Windows平台、平台操作系统版本和设备所有权设置移动限制</span><span class="sxs-lookup"><span data-stu-id="2abb2-162">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2abb2-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-163">androidRestriction</span></span>|[<span data-ttu-id="2abb2-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2abb2-165">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="2abb2-165">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2abb2-166">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-166">macOSRestriction</span></span>|[<span data-ttu-id="2abb2-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2abb2-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2abb2-168">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="2abb2-168">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="2abb2-169">关系</span><span class="sxs-lookup"><span data-stu-id="2abb2-169">Relationships</span></span>
|<span data-ttu-id="2abb2-170">关系</span><span class="sxs-lookup"><span data-stu-id="2abb2-170">Relationship</span></span>|<span data-ttu-id="2abb2-171">类型</span><span class="sxs-lookup"><span data-stu-id="2abb2-171">Type</span></span>|<span data-ttu-id="2abb2-172">Description</span><span class="sxs-lookup"><span data-stu-id="2abb2-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2abb2-173">assignments</span><span class="sxs-lookup"><span data-stu-id="2abb2-173">assignments</span></span>|<span data-ttu-id="2abb2-174">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2abb2-174">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2abb2-175">设备配置文件的组分配列表 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2abb2-175">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2abb2-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2abb2-176">JSON Representation</span></span>
<span data-ttu-id="2abb2-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2abb2-177">Here is a JSON representation of the resource.</span></span>
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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  }
}
```




