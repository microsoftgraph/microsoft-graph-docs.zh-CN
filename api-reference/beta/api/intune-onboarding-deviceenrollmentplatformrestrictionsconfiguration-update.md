---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 970462a8f993e8ef01f5c1359e865b625bfec611
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402298"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="180d0-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="180d0-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="180d0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="180d0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="180d0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="180d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="180d0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="180d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="180d0-107">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="180d0-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="180d0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="180d0-108">Prerequisites</span></span>
<span data-ttu-id="180d0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="180d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="180d0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="180d0-111">Permission type</span></span>|<span data-ttu-id="180d0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="180d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="180d0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="180d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="180d0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180d0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="180d0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="180d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="180d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="180d0-116">Not supported.</span></span>|
|<span data-ttu-id="180d0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="180d0-117">Application</span></span>|<span data-ttu-id="180d0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="180d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="180d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="180d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="180d0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="180d0-120">Request headers</span></span>
|<span data-ttu-id="180d0-121">标头</span><span class="sxs-lookup"><span data-stu-id="180d0-121">Header</span></span>|<span data-ttu-id="180d0-122">值</span><span class="sxs-lookup"><span data-stu-id="180d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="180d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="180d0-123">Authorization</span></span>|<span data-ttu-id="180d0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="180d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="180d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="180d0-125">Accept</span></span>|<span data-ttu-id="180d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="180d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="180d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="180d0-127">Request body</span></span>
<span data-ttu-id="180d0-128">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="180d0-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="180d0-129">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="180d0-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="180d0-130">属性</span><span class="sxs-lookup"><span data-stu-id="180d0-130">Property</span></span>|<span data-ttu-id="180d0-131">类型</span><span class="sxs-lookup"><span data-stu-id="180d0-131">Type</span></span>|<span data-ttu-id="180d0-132">说明</span><span class="sxs-lookup"><span data-stu-id="180d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180d0-133">id</span><span class="sxs-lookup"><span data-stu-id="180d0-133">id</span></span>|<span data-ttu-id="180d0-134">String</span><span class="sxs-lookup"><span data-stu-id="180d0-134">String</span></span>|<span data-ttu-id="180d0-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="180d0-136">displayName</span></span>|<span data-ttu-id="180d0-137">String</span><span class="sxs-lookup"><span data-stu-id="180d0-137">String</span></span>|<span data-ttu-id="180d0-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-139">description</span><span class="sxs-lookup"><span data-stu-id="180d0-139">description</span></span>|<span data-ttu-id="180d0-140">String</span><span class="sxs-lookup"><span data-stu-id="180d0-140">String</span></span>|<span data-ttu-id="180d0-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-142">priority</span><span class="sxs-lookup"><span data-stu-id="180d0-142">priority</span></span>|<span data-ttu-id="180d0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="180d0-143">Int32</span></span>|<span data-ttu-id="180d0-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="180d0-145">createdDateTime</span></span>|<span data-ttu-id="180d0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180d0-146">DateTimeOffset</span></span>|<span data-ttu-id="180d0-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="180d0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="180d0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180d0-149">DateTimeOffset</span></span>|<span data-ttu-id="180d0-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-151">version</span><span class="sxs-lookup"><span data-stu-id="180d0-151">version</span></span>|<span data-ttu-id="180d0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="180d0-152">Int32</span></span>|<span data-ttu-id="180d0-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="180d0-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="180d0-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-154">iosRestriction</span></span>|[<span data-ttu-id="180d0-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-156">Not yet documented</span></span>|
|<span data-ttu-id="180d0-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-157">windowsRestriction</span></span>|[<span data-ttu-id="180d0-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-159">Not yet documented</span></span>|
|<span data-ttu-id="180d0-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="180d0-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-162">Not yet documented</span></span>|
|<span data-ttu-id="180d0-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-163">androidRestriction</span></span>|[<span data-ttu-id="180d0-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-165">Not yet documented</span></span>|
|<span data-ttu-id="180d0-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="180d0-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-168">Not yet documented</span></span>|
|<span data-ttu-id="180d0-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-169">macRestriction</span></span>|[<span data-ttu-id="180d0-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-171">Not yet documented</span></span>|
|<span data-ttu-id="180d0-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-172">macOSRestriction</span></span>|[<span data-ttu-id="180d0-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="180d0-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="180d0-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="180d0-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="180d0-175">响应</span><span class="sxs-lookup"><span data-stu-id="180d0-175">Response</span></span>
<span data-ttu-id="180d0-176">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="180d0-176">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="180d0-177">示例</span><span class="sxs-lookup"><span data-stu-id="180d0-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="180d0-178">请求</span><span class="sxs-lookup"><span data-stu-id="180d0-178">Request</span></span>
<span data-ttu-id="180d0-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="180d0-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="180d0-180">响应</span><span class="sxs-lookup"><span data-stu-id="180d0-180">Response</span></span>
<span data-ttu-id="180d0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="180d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




