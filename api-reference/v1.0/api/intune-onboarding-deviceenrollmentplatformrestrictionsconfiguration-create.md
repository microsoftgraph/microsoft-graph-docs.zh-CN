---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbf7119a6e9819ce392241ae163992c83daec0be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52744811"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="06975-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="06975-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="06975-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06975-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06975-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06975-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06975-106">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06975-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06975-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="06975-107">Prerequisites</span></span>
<span data-ttu-id="06975-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06975-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="06975-110">Permission type</span></span>|<span data-ttu-id="06975-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06975-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06975-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06975-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06975-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06975-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="06975-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06975-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06975-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="06975-115">Not supported.</span></span>|
|<span data-ttu-id="06975-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="06975-116">Application</span></span>|<span data-ttu-id="06975-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06975-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06975-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06975-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06975-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06975-119">Request headers</span></span>
|<span data-ttu-id="06975-120">标头</span><span class="sxs-lookup"><span data-stu-id="06975-120">Header</span></span>|<span data-ttu-id="06975-121">值</span><span class="sxs-lookup"><span data-stu-id="06975-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06975-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06975-122">Authorization</span></span>|<span data-ttu-id="06975-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06975-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06975-124">接受</span><span class="sxs-lookup"><span data-stu-id="06975-124">Accept</span></span>|<span data-ttu-id="06975-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06975-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06975-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="06975-126">Request body</span></span>
<span data-ttu-id="06975-127">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06975-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="06975-128">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06975-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="06975-129">属性</span><span class="sxs-lookup"><span data-stu-id="06975-129">Property</span></span>|<span data-ttu-id="06975-130">类型</span><span class="sxs-lookup"><span data-stu-id="06975-130">Type</span></span>|<span data-ttu-id="06975-131">说明</span><span class="sxs-lookup"><span data-stu-id="06975-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06975-132">id</span><span class="sxs-lookup"><span data-stu-id="06975-132">id</span></span>|<span data-ttu-id="06975-133">String</span><span class="sxs-lookup"><span data-stu-id="06975-133">String</span></span>|<span data-ttu-id="06975-134">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-135">displayName</span><span class="sxs-lookup"><span data-stu-id="06975-135">displayName</span></span>|<span data-ttu-id="06975-136">String</span><span class="sxs-lookup"><span data-stu-id="06975-136">String</span></span>|<span data-ttu-id="06975-137">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-138">说明</span><span class="sxs-lookup"><span data-stu-id="06975-138">description</span></span>|<span data-ttu-id="06975-139">String</span><span class="sxs-lookup"><span data-stu-id="06975-139">String</span></span>|<span data-ttu-id="06975-140">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-141">priority</span><span class="sxs-lookup"><span data-stu-id="06975-141">priority</span></span>|<span data-ttu-id="06975-142">Int32</span><span class="sxs-lookup"><span data-stu-id="06975-142">Int32</span></span>|<span data-ttu-id="06975-143">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="06975-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="06975-144">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="06975-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="06975-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06975-146">createdDateTime</span></span>|<span data-ttu-id="06975-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06975-147">DateTimeOffset</span></span>|<span data-ttu-id="06975-148">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06975-149">lastModifiedDateTime</span></span>|<span data-ttu-id="06975-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06975-150">DateTimeOffset</span></span>|<span data-ttu-id="06975-151">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-152">version</span><span class="sxs-lookup"><span data-stu-id="06975-152">version</span></span>|<span data-ttu-id="06975-153">Int32</span><span class="sxs-lookup"><span data-stu-id="06975-153">Int32</span></span>|<span data-ttu-id="06975-154">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06975-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06975-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-155">iosRestriction</span></span>|[<span data-ttu-id="06975-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06975-157">基于平台、平台操作系统版本和设备所有权的 IOS 限制</span><span class="sxs-lookup"><span data-stu-id="06975-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="06975-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-158">windowsRestriction</span></span>|[<span data-ttu-id="06975-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06975-160">Windows平台、平台操作系统版本和设备所有权的限制</span><span class="sxs-lookup"><span data-stu-id="06975-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="06975-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="06975-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06975-163">Windows平台、平台操作系统版本和设备所有权设置移动限制</span><span class="sxs-lookup"><span data-stu-id="06975-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="06975-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-164">androidRestriction</span></span>|[<span data-ttu-id="06975-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06975-166">基于平台、平台操作系统版本和设备所有权的 Android 限制</span><span class="sxs-lookup"><span data-stu-id="06975-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="06975-167">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-167">macOSRestriction</span></span>|[<span data-ttu-id="06975-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06975-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06975-169">基于平台、平台操作系统版本和设备所有权的 Mac 限制</span><span class="sxs-lookup"><span data-stu-id="06975-169">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="06975-170">响应</span><span class="sxs-lookup"><span data-stu-id="06975-170">Response</span></span>
<span data-ttu-id="06975-171">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06975-171">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06975-172">示例</span><span class="sxs-lookup"><span data-stu-id="06975-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="06975-173">请求</span><span class="sxs-lookup"><span data-stu-id="06975-173">Request</span></span>
<span data-ttu-id="06975-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06975-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1650

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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="06975-175">响应</span><span class="sxs-lookup"><span data-stu-id="06975-175">Response</span></span>
<span data-ttu-id="06975-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06975-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1822

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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```




