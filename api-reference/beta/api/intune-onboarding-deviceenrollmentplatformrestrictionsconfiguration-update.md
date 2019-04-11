---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2897815a7324f88d4c10c4e5c940bc2d6b078cc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772648"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="f7b64-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7b64-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="f7b64-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7b64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7b64-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7b64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7b64-106">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f7b64-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7b64-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7b64-107">Prerequisites</span></span>
<span data-ttu-id="f7b64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7b64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7b64-110">Permission type</span></span>|<span data-ttu-id="f7b64-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7b64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7b64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7b64-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b64-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f7b64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7b64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b64-115">Not supported.</span></span>|
|<span data-ttu-id="f7b64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7b64-116">Application</span></span>|<span data-ttu-id="f7b64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7b64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7b64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7b64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7b64-119">Request headers</span></span>
|<span data-ttu-id="f7b64-120">标头</span><span class="sxs-lookup"><span data-stu-id="f7b64-120">Header</span></span>|<span data-ttu-id="f7b64-121">值</span><span class="sxs-lookup"><span data-stu-id="f7b64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7b64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7b64-122">Authorization</span></span>|<span data-ttu-id="f7b64-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7b64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7b64-124">接受</span><span class="sxs-lookup"><span data-stu-id="f7b64-124">Accept</span></span>|<span data-ttu-id="f7b64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7b64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7b64-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7b64-126">Request body</span></span>
<span data-ttu-id="f7b64-127">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7b64-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="f7b64-128">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7b64-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="f7b64-129">属性</span><span class="sxs-lookup"><span data-stu-id="f7b64-129">Property</span></span>|<span data-ttu-id="f7b64-130">类型</span><span class="sxs-lookup"><span data-stu-id="f7b64-130">Type</span></span>|<span data-ttu-id="f7b64-131">说明</span><span class="sxs-lookup"><span data-stu-id="f7b64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7b64-132">id</span><span class="sxs-lookup"><span data-stu-id="f7b64-132">id</span></span>|<span data-ttu-id="f7b64-133">String</span><span class="sxs-lookup"><span data-stu-id="f7b64-133">String</span></span>|<span data-ttu-id="f7b64-134">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的注册状态页面配置的 Id</span><span class="sxs-lookup"><span data-stu-id="f7b64-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f7b64-135">displayName</span></span>|<span data-ttu-id="f7b64-136">String</span><span class="sxs-lookup"><span data-stu-id="f7b64-136">String</span></span>|<span data-ttu-id="f7b64-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7b64-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-138">description</span><span class="sxs-lookup"><span data-stu-id="f7b64-138">description</span></span>|<span data-ttu-id="f7b64-139">String</span><span class="sxs-lookup"><span data-stu-id="f7b64-139">String</span></span>|<span data-ttu-id="f7b64-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7b64-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-141">priority</span><span class="sxs-lookup"><span data-stu-id="f7b64-141">priority</span></span>|<span data-ttu-id="f7b64-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f7b64-142">Int32</span></span>|<span data-ttu-id="f7b64-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7b64-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7b64-144">createdDateTime</span></span>|<span data-ttu-id="f7b64-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7b64-145">DateTimeOffset</span></span>|<span data-ttu-id="f7b64-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7b64-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7b64-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f7b64-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7b64-148">DateTimeOffset</span></span>|<span data-ttu-id="f7b64-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7b64-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-150">version</span><span class="sxs-lookup"><span data-stu-id="f7b64-150">version</span></span>|<span data-ttu-id="f7b64-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f7b64-151">Int32</span></span>|<span data-ttu-id="f7b64-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7b64-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f7b64-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-153">iosRestriction</span></span>|[<span data-ttu-id="f7b64-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-155">Not yet documented</span></span>|
|<span data-ttu-id="f7b64-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-156">windowsRestriction</span></span>|[<span data-ttu-id="f7b64-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-158">Not yet documented</span></span>|
|<span data-ttu-id="f7b64-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="f7b64-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-161">Not yet documented</span></span>|
|<span data-ttu-id="f7b64-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-162">androidRestriction</span></span>|[<span data-ttu-id="f7b64-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-164">Not yet documented</span></span>|
|<span data-ttu-id="f7b64-165">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="f7b64-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-167">Not yet documented</span></span>|
|<span data-ttu-id="f7b64-168">macRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-168">macRestriction</span></span>|[<span data-ttu-id="f7b64-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-170">Not yet documented</span></span>|
|<span data-ttu-id="f7b64-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-171">macOSRestriction</span></span>|[<span data-ttu-id="f7b64-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f7b64-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f7b64-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7b64-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7b64-174">响应</span><span class="sxs-lookup"><span data-stu-id="f7b64-174">Response</span></span>
<span data-ttu-id="f7b64-175">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7b64-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b64-176">示例</span><span class="sxs-lookup"><span data-stu-id="f7b64-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7b64-177">请求</span><span class="sxs-lookup"><span data-stu-id="f7b64-177">Request</span></span>
<span data-ttu-id="f7b64-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7b64-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7b64-179">响应</span><span class="sxs-lookup"><span data-stu-id="f7b64-179">Response</span></span>
<span data-ttu-id="f7b64-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7b64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





