---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8911bb53465ceaf8cf1ba344c3f8e6433ae09835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087276"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="25c78-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="25c78-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="25c78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25c78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25c78-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25c78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c78-106">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="25c78-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25c78-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="25c78-107">Prerequisites</span></span>
<span data-ttu-id="25c78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25c78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25c78-110">Permission type</span></span>|<span data-ttu-id="25c78-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="25c78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25c78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25c78-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c78-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="25c78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25c78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c78-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25c78-115">Not supported.</span></span>|
|<span data-ttu-id="25c78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25c78-116">Application</span></span>|<span data-ttu-id="25c78-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="25c78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25c78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="25c78-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25c78-119">Request headers</span></span>
|<span data-ttu-id="25c78-120">标头</span><span class="sxs-lookup"><span data-stu-id="25c78-120">Header</span></span>|<span data-ttu-id="25c78-121">值</span><span class="sxs-lookup"><span data-stu-id="25c78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25c78-122">Authorization</span></span>|<span data-ttu-id="25c78-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25c78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c78-124">接受</span><span class="sxs-lookup"><span data-stu-id="25c78-124">Accept</span></span>|<span data-ttu-id="25c78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25c78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c78-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="25c78-126">Request body</span></span>
<span data-ttu-id="25c78-127">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25c78-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="25c78-128">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25c78-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="25c78-129">属性</span><span class="sxs-lookup"><span data-stu-id="25c78-129">Property</span></span>|<span data-ttu-id="25c78-130">类型</span><span class="sxs-lookup"><span data-stu-id="25c78-130">Type</span></span>|<span data-ttu-id="25c78-131">说明</span><span class="sxs-lookup"><span data-stu-id="25c78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c78-132">id</span><span class="sxs-lookup"><span data-stu-id="25c78-132">id</span></span>|<span data-ttu-id="25c78-133">String</span><span class="sxs-lookup"><span data-stu-id="25c78-133">String</span></span>|<span data-ttu-id="25c78-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-135">displayName</span><span class="sxs-lookup"><span data-stu-id="25c78-135">displayName</span></span>|<span data-ttu-id="25c78-136">String</span><span class="sxs-lookup"><span data-stu-id="25c78-136">String</span></span>|<span data-ttu-id="25c78-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-138">description</span><span class="sxs-lookup"><span data-stu-id="25c78-138">description</span></span>|<span data-ttu-id="25c78-139">String</span><span class="sxs-lookup"><span data-stu-id="25c78-139">String</span></span>|<span data-ttu-id="25c78-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-141">priority</span><span class="sxs-lookup"><span data-stu-id="25c78-141">priority</span></span>|<span data-ttu-id="25c78-142">Int32</span><span class="sxs-lookup"><span data-stu-id="25c78-142">Int32</span></span>|<span data-ttu-id="25c78-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25c78-144">createdDateTime</span></span>|<span data-ttu-id="25c78-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c78-145">DateTimeOffset</span></span>|<span data-ttu-id="25c78-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25c78-147">lastModifiedDateTime</span></span>|<span data-ttu-id="25c78-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c78-148">DateTimeOffset</span></span>|<span data-ttu-id="25c78-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-150">version</span><span class="sxs-lookup"><span data-stu-id="25c78-150">version</span></span>|<span data-ttu-id="25c78-151">Int32</span><span class="sxs-lookup"><span data-stu-id="25c78-151">Int32</span></span>|<span data-ttu-id="25c78-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c78-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25c78-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-153">iosRestriction</span></span>|[<span data-ttu-id="25c78-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="25c78-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25c78-155">Not yet documented</span></span>|
|<span data-ttu-id="25c78-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-156">windowsRestriction</span></span>|[<span data-ttu-id="25c78-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="25c78-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25c78-158">Not yet documented</span></span>|
|<span data-ttu-id="25c78-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="25c78-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="25c78-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25c78-161">Not yet documented</span></span>|
|<span data-ttu-id="25c78-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-162">androidRestriction</span></span>|[<span data-ttu-id="25c78-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="25c78-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25c78-164">Not yet documented</span></span>|
|<span data-ttu-id="25c78-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-165">macOSRestriction</span></span>|[<span data-ttu-id="25c78-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="25c78-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="25c78-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25c78-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="25c78-168">响应</span><span class="sxs-lookup"><span data-stu-id="25c78-168">Response</span></span>
<span data-ttu-id="25c78-169">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25c78-169">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c78-170">示例</span><span class="sxs-lookup"><span data-stu-id="25c78-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c78-171">请求</span><span class="sxs-lookup"><span data-stu-id="25c78-171">Request</span></span>
<span data-ttu-id="25c78-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25c78-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="25c78-173">响应</span><span class="sxs-lookup"><span data-stu-id="25c78-173">Response</span></span>
<span data-ttu-id="25c78-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25c78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









