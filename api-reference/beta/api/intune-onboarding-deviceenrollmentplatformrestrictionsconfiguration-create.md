---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfd552e24ba640775cc0470703dc0e6e39108e2f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148811"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="63ed6-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="63ed6-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="63ed6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63ed6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63ed6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63ed6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63ed6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63ed6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63ed6-107">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63ed6-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63ed6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="63ed6-108">Prerequisites</span></span>
<span data-ttu-id="63ed6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63ed6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63ed6-111">Permission type</span></span>|<span data-ttu-id="63ed6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63ed6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63ed6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63ed6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63ed6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63ed6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63ed6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63ed6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63ed6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63ed6-116">Not supported.</span></span>|
|<span data-ttu-id="63ed6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63ed6-117">Application</span></span>|<span data-ttu-id="63ed6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63ed6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63ed6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63ed6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63ed6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="63ed6-120">Request headers</span></span>
|<span data-ttu-id="63ed6-121">标头</span><span class="sxs-lookup"><span data-stu-id="63ed6-121">Header</span></span>|<span data-ttu-id="63ed6-122">值</span><span class="sxs-lookup"><span data-stu-id="63ed6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63ed6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63ed6-123">Authorization</span></span>|<span data-ttu-id="63ed6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63ed6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63ed6-125">接受</span><span class="sxs-lookup"><span data-stu-id="63ed6-125">Accept</span></span>|<span data-ttu-id="63ed6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63ed6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63ed6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63ed6-127">Request body</span></span>
<span data-ttu-id="63ed6-128">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63ed6-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="63ed6-129">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63ed6-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="63ed6-130">属性</span><span class="sxs-lookup"><span data-stu-id="63ed6-130">Property</span></span>|<span data-ttu-id="63ed6-131">类型</span><span class="sxs-lookup"><span data-stu-id="63ed6-131">Type</span></span>|<span data-ttu-id="63ed6-132">说明</span><span class="sxs-lookup"><span data-stu-id="63ed6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63ed6-133">id</span><span class="sxs-lookup"><span data-stu-id="63ed6-133">id</span></span>|<span data-ttu-id="63ed6-134">String</span><span class="sxs-lookup"><span data-stu-id="63ed6-134">String</span></span>|<span data-ttu-id="63ed6-135">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="63ed6-136">displayName</span></span>|<span data-ttu-id="63ed6-137">String</span><span class="sxs-lookup"><span data-stu-id="63ed6-137">String</span></span>|<span data-ttu-id="63ed6-138">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-139">说明</span><span class="sxs-lookup"><span data-stu-id="63ed6-139">description</span></span>|<span data-ttu-id="63ed6-140">String</span><span class="sxs-lookup"><span data-stu-id="63ed6-140">String</span></span>|<span data-ttu-id="63ed6-141">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-142">priority</span><span class="sxs-lookup"><span data-stu-id="63ed6-142">priority</span></span>|<span data-ttu-id="63ed6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="63ed6-143">Int32</span></span>|<span data-ttu-id="63ed6-144">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="63ed6-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="63ed6-145">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="63ed6-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="63ed6-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63ed6-147">createdDateTime</span></span>|<span data-ttu-id="63ed6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63ed6-148">DateTimeOffset</span></span>|<span data-ttu-id="63ed6-149">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63ed6-150">lastModifiedDateTime</span></span>|<span data-ttu-id="63ed6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63ed6-151">DateTimeOffset</span></span>|<span data-ttu-id="63ed6-152">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-153">version</span><span class="sxs-lookup"><span data-stu-id="63ed6-153">version</span></span>|<span data-ttu-id="63ed6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="63ed6-154">Int32</span></span>|<span data-ttu-id="63ed6-155">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63ed6-156">roleScopeTagIds</span></span>|<span data-ttu-id="63ed6-157">String collection</span><span class="sxs-lookup"><span data-stu-id="63ed6-157">String collection</span></span>|<span data-ttu-id="63ed6-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="63ed6-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="63ed6-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ed6-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="63ed6-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-160">iosRestriction</span></span>|[<span data-ttu-id="63ed6-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-162">基于平台、平台操作系统版本和设备所有权的 IOS 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-163">windowsRestriction</span></span>|[<span data-ttu-id="63ed6-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-165">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-166">windowsHomeSkuRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-166">windowsHomeSkuRestriction</span></span>|[<span data-ttu-id="63ed6-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-168">基于平台、平台操作系统版本和设备所有权的 Windows Home Sku 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-168">Windows Home Sku restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-169">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-169">windowsMobileRestriction</span></span>|[<span data-ttu-id="63ed6-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-171">基于平台、平台操作系统版本和设备所有权的 Windows 移动限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-171">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-172">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-172">androidRestriction</span></span>|[<span data-ttu-id="63ed6-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-174">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-174">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-175">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-175">androidForWorkRestriction</span></span>|[<span data-ttu-id="63ed6-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-177">Android for work restrictions based on platform， platform operating system version， and device ownership</span><span class="sxs-lookup"><span data-stu-id="63ed6-177">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-178">aospRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-178">aospRestriction</span></span>|[<span data-ttu-id="63ed6-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-180">基于平台、平台操作系统版本和设备所有权的 AOSP 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-180">AOSP restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-181">macRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-181">macRestriction</span></span>|[<span data-ttu-id="63ed6-182">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-182">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-183">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-183">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="63ed6-184">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-184">macOSRestriction</span></span>|[<span data-ttu-id="63ed6-185">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="63ed6-185">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="63ed6-186">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="63ed6-186">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="63ed6-187">响应</span><span class="sxs-lookup"><span data-stu-id="63ed6-187">Response</span></span>
<span data-ttu-id="63ed6-188">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63ed6-188">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63ed6-189">示例</span><span class="sxs-lookup"><span data-stu-id="63ed6-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="63ed6-190">请求</span><span class="sxs-lookup"><span data-stu-id="63ed6-190">Request</span></span>
<span data-ttu-id="63ed6-191">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63ed6-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 4081

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "windowsHomeSkuRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="63ed6-192">响应</span><span class="sxs-lookup"><span data-stu-id="63ed6-192">Response</span></span>
<span data-ttu-id="63ed6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63ed6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4253

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "windowsHomeSkuRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  }
}
```




