---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5d2afdd841cd6ed4d279f38a6963ac33a9c7103
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177546"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="93218-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="93218-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="93218-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93218-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93218-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93218-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93218-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93218-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93218-107">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93218-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93218-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="93218-108">Prerequisites</span></span>
<span data-ttu-id="93218-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93218-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="93218-111">Permission type</span></span>|<span data-ttu-id="93218-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93218-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93218-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93218-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93218-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93218-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93218-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93218-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93218-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="93218-116">Not supported.</span></span>|
|<span data-ttu-id="93218-117">Application</span><span class="sxs-lookup"><span data-stu-id="93218-117">Application</span></span>|<span data-ttu-id="93218-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93218-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93218-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93218-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="93218-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="93218-120">Request headers</span></span>
|<span data-ttu-id="93218-121">标头</span><span class="sxs-lookup"><span data-stu-id="93218-121">Header</span></span>|<span data-ttu-id="93218-122">值</span><span class="sxs-lookup"><span data-stu-id="93218-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93218-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93218-123">Authorization</span></span>|<span data-ttu-id="93218-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93218-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93218-125">接受</span><span class="sxs-lookup"><span data-stu-id="93218-125">Accept</span></span>|<span data-ttu-id="93218-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93218-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93218-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93218-127">Request body</span></span>
<span data-ttu-id="93218-128">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93218-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="93218-129">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93218-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="93218-130">属性</span><span class="sxs-lookup"><span data-stu-id="93218-130">Property</span></span>|<span data-ttu-id="93218-131">类型</span><span class="sxs-lookup"><span data-stu-id="93218-131">Type</span></span>|<span data-ttu-id="93218-132">说明</span><span class="sxs-lookup"><span data-stu-id="93218-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93218-133">id</span><span class="sxs-lookup"><span data-stu-id="93218-133">id</span></span>|<span data-ttu-id="93218-134">字符串</span><span class="sxs-lookup"><span data-stu-id="93218-134">String</span></span>|<span data-ttu-id="93218-135">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="93218-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-136">displayName</span><span class="sxs-lookup"><span data-stu-id="93218-136">displayName</span></span>|<span data-ttu-id="93218-137">String</span><span class="sxs-lookup"><span data-stu-id="93218-137">String</span></span>|<span data-ttu-id="93218-138">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="93218-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-139">说明</span><span class="sxs-lookup"><span data-stu-id="93218-139">description</span></span>|<span data-ttu-id="93218-140">String</span><span class="sxs-lookup"><span data-stu-id="93218-140">String</span></span>|<span data-ttu-id="93218-141">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="93218-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-142">priority</span><span class="sxs-lookup"><span data-stu-id="93218-142">priority</span></span>|<span data-ttu-id="93218-143">Int32</span><span class="sxs-lookup"><span data-stu-id="93218-143">Int32</span></span>|<span data-ttu-id="93218-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="93218-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="93218-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="93218-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="93218-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93218-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93218-147">createdDateTime</span></span>|<span data-ttu-id="93218-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93218-148">DateTimeOffset</span></span>|<span data-ttu-id="93218-149">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="93218-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93218-150">lastModifiedDateTime</span></span>|<span data-ttu-id="93218-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93218-151">DateTimeOffset</span></span>|<span data-ttu-id="93218-152">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="93218-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-153">version</span><span class="sxs-lookup"><span data-stu-id="93218-153">version</span></span>|<span data-ttu-id="93218-154">Int32</span><span class="sxs-lookup"><span data-stu-id="93218-154">Int32</span></span>|<span data-ttu-id="93218-155">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="93218-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93218-156">roleScopeTagIds</span></span>|<span data-ttu-id="93218-157">字符串集合</span><span class="sxs-lookup"><span data-stu-id="93218-157">String collection</span></span>|<span data-ttu-id="93218-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="93218-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="93218-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93218-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="93218-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-160">iosRestriction</span></span>|[<span data-ttu-id="93218-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-162">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="93218-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="93218-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-163">windowsRestriction</span></span>|[<span data-ttu-id="93218-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-165">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="93218-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="93218-166">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-166">windowsMobileRestriction</span></span>|[<span data-ttu-id="93218-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-168">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="93218-168">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="93218-169">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-169">androidRestriction</span></span>|[<span data-ttu-id="93218-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-171">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="93218-171">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="93218-172">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-172">androidForWorkRestriction</span></span>|[<span data-ttu-id="93218-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-174">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="93218-174">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="93218-175">macRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-175">macRestriction</span></span>|[<span data-ttu-id="93218-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-177">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="93218-177">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="93218-178">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-178">macOSRestriction</span></span>|[<span data-ttu-id="93218-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="93218-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="93218-180">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="93218-180">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="93218-181">响应</span><span class="sxs-lookup"><span data-stu-id="93218-181">Response</span></span>
<span data-ttu-id="93218-182">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93218-182">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93218-183">示例</span><span class="sxs-lookup"><span data-stu-id="93218-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="93218-184">请求</span><span class="sxs-lookup"><span data-stu-id="93218-184">Request</span></span>
<span data-ttu-id="93218-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93218-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 2825

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
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="93218-186">响应</span><span class="sxs-lookup"><span data-stu-id="93218-186">Response</span></span>
<span data-ttu-id="93218-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93218-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2997

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
    ]
  }
}
```



