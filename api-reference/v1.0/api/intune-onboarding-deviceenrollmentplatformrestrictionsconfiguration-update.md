---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcb8af7e91a04598d257a4db674891fbd4cf33c2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362573"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="523da-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="523da-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="523da-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="523da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="523da-105">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="523da-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="523da-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="523da-106">Prerequisites</span></span>
<span data-ttu-id="523da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="523da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="523da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="523da-109">Permission type</span></span>|<span data-ttu-id="523da-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="523da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="523da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="523da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="523da-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="523da-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="523da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="523da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="523da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="523da-114">Not supported.</span></span>|
|<span data-ttu-id="523da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="523da-115">Application</span></span>|<span data-ttu-id="523da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="523da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="523da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="523da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="523da-118">请求头</span><span class="sxs-lookup"><span data-stu-id="523da-118">Request headers</span></span>
|<span data-ttu-id="523da-119">标头</span><span class="sxs-lookup"><span data-stu-id="523da-119">Header</span></span>|<span data-ttu-id="523da-120">值</span><span class="sxs-lookup"><span data-stu-id="523da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="523da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="523da-121">Authorization</span></span>|<span data-ttu-id="523da-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="523da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="523da-123">接受</span><span class="sxs-lookup"><span data-stu-id="523da-123">Accept</span></span>|<span data-ttu-id="523da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="523da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="523da-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="523da-125">Request body</span></span>
<span data-ttu-id="523da-126">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="523da-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="523da-127">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="523da-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="523da-128">属性</span><span class="sxs-lookup"><span data-stu-id="523da-128">Property</span></span>|<span data-ttu-id="523da-129">类型</span><span class="sxs-lookup"><span data-stu-id="523da-129">Type</span></span>|<span data-ttu-id="523da-130">说明</span><span class="sxs-lookup"><span data-stu-id="523da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="523da-131">id</span><span class="sxs-lookup"><span data-stu-id="523da-131">id</span></span>|<span data-ttu-id="523da-132">字符串</span><span class="sxs-lookup"><span data-stu-id="523da-132">String</span></span>|<span data-ttu-id="523da-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-134">displayName</span><span class="sxs-lookup"><span data-stu-id="523da-134">displayName</span></span>|<span data-ttu-id="523da-135">String</span><span class="sxs-lookup"><span data-stu-id="523da-135">String</span></span>|<span data-ttu-id="523da-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-137">说明</span><span class="sxs-lookup"><span data-stu-id="523da-137">description</span></span>|<span data-ttu-id="523da-138">String</span><span class="sxs-lookup"><span data-stu-id="523da-138">String</span></span>|<span data-ttu-id="523da-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-140">priority</span><span class="sxs-lookup"><span data-stu-id="523da-140">priority</span></span>|<span data-ttu-id="523da-141">Int32</span><span class="sxs-lookup"><span data-stu-id="523da-141">Int32</span></span>|<span data-ttu-id="523da-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="523da-143">createdDateTime</span></span>|<span data-ttu-id="523da-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="523da-144">DateTimeOffset</span></span>|<span data-ttu-id="523da-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="523da-146">lastModifiedDateTime</span></span>|<span data-ttu-id="523da-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="523da-147">DateTimeOffset</span></span>|<span data-ttu-id="523da-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-149">version</span><span class="sxs-lookup"><span data-stu-id="523da-149">version</span></span>|<span data-ttu-id="523da-150">Int32</span><span class="sxs-lookup"><span data-stu-id="523da-150">Int32</span></span>|<span data-ttu-id="523da-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="523da-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="523da-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-152">iosRestriction</span></span>|[<span data-ttu-id="523da-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="523da-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="523da-154">Not yet documented</span></span>|
|<span data-ttu-id="523da-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-155">windowsRestriction</span></span>|[<span data-ttu-id="523da-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="523da-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="523da-157">Not yet documented</span></span>|
|<span data-ttu-id="523da-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="523da-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="523da-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="523da-160">Not yet documented</span></span>|
|<span data-ttu-id="523da-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-161">androidRestriction</span></span>|[<span data-ttu-id="523da-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="523da-163">尚未记录</span><span class="sxs-lookup"><span data-stu-id="523da-163">Not yet documented</span></span>|
|<span data-ttu-id="523da-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-164">macOSRestriction</span></span>|[<span data-ttu-id="523da-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="523da-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="523da-166">尚未记录</span><span class="sxs-lookup"><span data-stu-id="523da-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="523da-167">响应</span><span class="sxs-lookup"><span data-stu-id="523da-167">Response</span></span>
<span data-ttu-id="523da-168">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="523da-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="523da-169">示例</span><span class="sxs-lookup"><span data-stu-id="523da-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="523da-170">请求</span><span class="sxs-lookup"><span data-stu-id="523da-170">Request</span></span>
<span data-ttu-id="523da-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="523da-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="523da-172">响应</span><span class="sxs-lookup"><span data-stu-id="523da-172">Response</span></span>
<span data-ttu-id="523da-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="523da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




