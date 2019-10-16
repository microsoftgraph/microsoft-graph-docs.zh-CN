---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f72bb2799d8a1220ee20ded59a5ffbf0bdbb3af
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536124"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="2418f-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="2418f-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="2418f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2418f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2418f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2418f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2418f-106">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2418f-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2418f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2418f-107">Prerequisites</span></span>
<span data-ttu-id="2418f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2418f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2418f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2418f-110">Permission type</span></span>|<span data-ttu-id="2418f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2418f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2418f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2418f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2418f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2418f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2418f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2418f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2418f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2418f-115">Not supported.</span></span>|
|<span data-ttu-id="2418f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2418f-116">Application</span></span>|<span data-ttu-id="2418f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2418f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2418f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2418f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2418f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2418f-119">Request headers</span></span>
|<span data-ttu-id="2418f-120">标头</span><span class="sxs-lookup"><span data-stu-id="2418f-120">Header</span></span>|<span data-ttu-id="2418f-121">值</span><span class="sxs-lookup"><span data-stu-id="2418f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2418f-122">授权</span><span class="sxs-lookup"><span data-stu-id="2418f-122">Authorization</span></span>|<span data-ttu-id="2418f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2418f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2418f-124">接受</span><span class="sxs-lookup"><span data-stu-id="2418f-124">Accept</span></span>|<span data-ttu-id="2418f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2418f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2418f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2418f-126">Request body</span></span>
<span data-ttu-id="2418f-127">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2418f-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="2418f-128">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2418f-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="2418f-129">属性</span><span class="sxs-lookup"><span data-stu-id="2418f-129">Property</span></span>|<span data-ttu-id="2418f-130">类型</span><span class="sxs-lookup"><span data-stu-id="2418f-130">Type</span></span>|<span data-ttu-id="2418f-131">说明</span><span class="sxs-lookup"><span data-stu-id="2418f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2418f-132">id</span><span class="sxs-lookup"><span data-stu-id="2418f-132">id</span></span>|<span data-ttu-id="2418f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2418f-133">String</span></span>|<span data-ttu-id="2418f-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="2418f-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2418f-135">displayName</span></span>|<span data-ttu-id="2418f-136">String</span><span class="sxs-lookup"><span data-stu-id="2418f-136">String</span></span>|<span data-ttu-id="2418f-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="2418f-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-138">说明</span><span class="sxs-lookup"><span data-stu-id="2418f-138">description</span></span>|<span data-ttu-id="2418f-139">String</span><span class="sxs-lookup"><span data-stu-id="2418f-139">String</span></span>|<span data-ttu-id="2418f-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="2418f-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-141">priority</span><span class="sxs-lookup"><span data-stu-id="2418f-141">priority</span></span>|<span data-ttu-id="2418f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2418f-142">Int32</span></span>|<span data-ttu-id="2418f-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="2418f-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="2418f-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="2418f-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="2418f-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2418f-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2418f-146">createdDateTime</span></span>|<span data-ttu-id="2418f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2418f-147">DateTimeOffset</span></span>|<span data-ttu-id="2418f-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="2418f-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2418f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2418f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2418f-150">DateTimeOffset</span></span>|<span data-ttu-id="2418f-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="2418f-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-152">version</span><span class="sxs-lookup"><span data-stu-id="2418f-152">version</span></span>|<span data-ttu-id="2418f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2418f-153">Int32</span></span>|<span data-ttu-id="2418f-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="2418f-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2418f-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-155">iosRestriction</span></span>|[<span data-ttu-id="2418f-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-157">基于平台、平台操作系统版本和设备所有权的 Ios 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2418f-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-158">windowsRestriction</span></span>|[<span data-ttu-id="2418f-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-160">基于平台、平台操作系统版本和设备所有权的 Windows 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2418f-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="2418f-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-163">基于平台、平台操作系统版本和设备所有权的 Windows mobile 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2418f-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-164">androidRestriction</span></span>|[<span data-ttu-id="2418f-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-166">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2418f-167">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="2418f-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-169">基于平台、平台操作系统版本和设备所有权的 Android for work 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2418f-170">macRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-170">macRestriction</span></span>|[<span data-ttu-id="2418f-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-172">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="2418f-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-173">macOSRestriction</span></span>|[<span data-ttu-id="2418f-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2418f-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="2418f-175">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="2418f-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="2418f-176">响应</span><span class="sxs-lookup"><span data-stu-id="2418f-176">Response</span></span>
<span data-ttu-id="2418f-177">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2418f-177">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2418f-178">示例</span><span class="sxs-lookup"><span data-stu-id="2418f-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="2418f-179">请求</span><span class="sxs-lookup"><span data-stu-id="2418f-179">Request</span></span>
<span data-ttu-id="2418f-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2418f-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="2418f-181">响应</span><span class="sxs-lookup"><span data-stu-id="2418f-181">Response</span></span>
<span data-ttu-id="2418f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2418f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






