---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e36bfd5edc4e1d05dad5f6349530cdb71f6aa60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984578"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="b3bd0-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3bd0-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="b3bd0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3bd0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3bd0-106">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3bd0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3bd0-107">Prerequisites</span></span>
<span data-ttu-id="b3bd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3bd0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3bd0-110">Permission type</span></span>|<span data-ttu-id="b3bd0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3bd0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3bd0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3bd0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3bd0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3bd0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3bd0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3bd0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3bd0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-115">Not supported.</span></span>|
|<span data-ttu-id="b3bd0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3bd0-116">Application</span></span>|<span data-ttu-id="b3bd0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3bd0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3bd0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3bd0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3bd0-119">Request headers</span></span>
|<span data-ttu-id="b3bd0-120">标头</span><span class="sxs-lookup"><span data-stu-id="b3bd0-120">Header</span></span>|<span data-ttu-id="b3bd0-121">值</span><span class="sxs-lookup"><span data-stu-id="b3bd0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3bd0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3bd0-122">Authorization</span></span>|<span data-ttu-id="b3bd0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3bd0-124">接受</span><span class="sxs-lookup"><span data-stu-id="b3bd0-124">Accept</span></span>|<span data-ttu-id="b3bd0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3bd0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3bd0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3bd0-126">Request body</span></span>
<span data-ttu-id="b3bd0-127">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="b3bd0-128">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="b3bd0-129">属性</span><span class="sxs-lookup"><span data-stu-id="b3bd0-129">Property</span></span>|<span data-ttu-id="b3bd0-130">类型</span><span class="sxs-lookup"><span data-stu-id="b3bd0-130">Type</span></span>|<span data-ttu-id="b3bd0-131">说明</span><span class="sxs-lookup"><span data-stu-id="b3bd0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3bd0-132">id</span><span class="sxs-lookup"><span data-stu-id="b3bd0-132">id</span></span>|<span data-ttu-id="b3bd0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b3bd0-133">String</span></span>|<span data-ttu-id="b3bd0-134">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b3bd0-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b3bd0-135">displayName</span></span>|<span data-ttu-id="b3bd0-136">String</span><span class="sxs-lookup"><span data-stu-id="b3bd0-136">String</span></span>|<span data-ttu-id="b3bd0-137">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="b3bd0-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-138">说明</span><span class="sxs-lookup"><span data-stu-id="b3bd0-138">description</span></span>|<span data-ttu-id="b3bd0-139">String</span><span class="sxs-lookup"><span data-stu-id="b3bd0-139">String</span></span>|<span data-ttu-id="b3bd0-140">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="b3bd0-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-141">priority</span><span class="sxs-lookup"><span data-stu-id="b3bd0-141">priority</span></span>|<span data-ttu-id="b3bd0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bd0-142">Int32</span></span>|<span data-ttu-id="b3bd0-143">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="b3bd0-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="b3bd0-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3bd0-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3bd0-146">createdDateTime</span></span>|<span data-ttu-id="b3bd0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3bd0-147">DateTimeOffset</span></span>|<span data-ttu-id="b3bd0-148">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="b3bd0-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3bd0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b3bd0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3bd0-150">DateTimeOffset</span></span>|<span data-ttu-id="b3bd0-151">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="b3bd0-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-152">version</span><span class="sxs-lookup"><span data-stu-id="b3bd0-152">version</span></span>|<span data-ttu-id="b3bd0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bd0-153">Int32</span></span>|<span data-ttu-id="b3bd0-154">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="b3bd0-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3bd0-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-155">iosRestriction</span></span>|[<span data-ttu-id="b3bd0-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-157">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="b3bd0-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-158">windowsRestriction</span></span>|[<span data-ttu-id="b3bd0-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-160">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="b3bd0-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="b3bd0-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-163">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="b3bd0-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-164">androidRestriction</span></span>|[<span data-ttu-id="b3bd0-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-166">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="b3bd0-167">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="b3bd0-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-169">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="b3bd0-170">macRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-170">macRestriction</span></span>|[<span data-ttu-id="b3bd0-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-172">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="b3bd0-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-173">macOSRestriction</span></span>|[<span data-ttu-id="b3bd0-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bd0-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b3bd0-175">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="b3bd0-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="b3bd0-176">响应</span><span class="sxs-lookup"><span data-stu-id="b3bd0-176">Response</span></span>
<span data-ttu-id="b3bd0-177">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-177">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3bd0-178">示例</span><span class="sxs-lookup"><span data-stu-id="b3bd0-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3bd0-179">请求</span><span class="sxs-lookup"><span data-stu-id="b3bd0-179">Request</span></span>
<span data-ttu-id="b3bd0-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="b3bd0-181">响应</span><span class="sxs-lookup"><span data-stu-id="b3bd0-181">Response</span></span>
<span data-ttu-id="b3bd0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3bd0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2403

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```





