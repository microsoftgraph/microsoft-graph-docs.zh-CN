---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8b877e81512bf6994cc29b9bcec1e7f943f98c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255897"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="148e8-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="148e8-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="148e8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="148e8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148e8-105">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="148e8-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="148e8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="148e8-106">Prerequisites</span></span>
<span data-ttu-id="148e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="148e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="148e8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="148e8-109">Permission type</span></span>|<span data-ttu-id="148e8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="148e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="148e8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="148e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="148e8-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148e8-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="148e8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="148e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="148e8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="148e8-114">Not supported.</span></span>|
|<span data-ttu-id="148e8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="148e8-115">Application</span></span>|<span data-ttu-id="148e8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="148e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="148e8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="148e8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="148e8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="148e8-118">Request headers</span></span>
|<span data-ttu-id="148e8-119">标头</span><span class="sxs-lookup"><span data-stu-id="148e8-119">Header</span></span>|<span data-ttu-id="148e8-120">值</span><span class="sxs-lookup"><span data-stu-id="148e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="148e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="148e8-121">Authorization</span></span>|<span data-ttu-id="148e8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="148e8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="148e8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="148e8-123">Accept</span></span>|<span data-ttu-id="148e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="148e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="148e8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="148e8-125">Request body</span></span>
<span data-ttu-id="148e8-126">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="148e8-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="148e8-127">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="148e8-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="148e8-128">属性</span><span class="sxs-lookup"><span data-stu-id="148e8-128">Property</span></span>|<span data-ttu-id="148e8-129">类型</span><span class="sxs-lookup"><span data-stu-id="148e8-129">Type</span></span>|<span data-ttu-id="148e8-130">说明</span><span class="sxs-lookup"><span data-stu-id="148e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148e8-131">id</span><span class="sxs-lookup"><span data-stu-id="148e8-131">id</span></span>|<span data-ttu-id="148e8-132">String</span><span class="sxs-lookup"><span data-stu-id="148e8-132">String</span></span>|<span data-ttu-id="148e8-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="148e8-134">displayName</span></span>|<span data-ttu-id="148e8-135">String</span><span class="sxs-lookup"><span data-stu-id="148e8-135">String</span></span>|<span data-ttu-id="148e8-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-137">description</span><span class="sxs-lookup"><span data-stu-id="148e8-137">description</span></span>|<span data-ttu-id="148e8-138">String</span><span class="sxs-lookup"><span data-stu-id="148e8-138">String</span></span>|<span data-ttu-id="148e8-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-140">priority</span><span class="sxs-lookup"><span data-stu-id="148e8-140">priority</span></span>|<span data-ttu-id="148e8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="148e8-141">Int32</span></span>|<span data-ttu-id="148e8-142">尚未记录 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="148e8-143">createdDateTime</span></span>|<span data-ttu-id="148e8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148e8-144">DateTimeOffset</span></span>|<span data-ttu-id="148e8-145">尚未记录 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="148e8-146">lastModifiedDateTime</span></span>|<span data-ttu-id="148e8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148e8-147">DateTimeOffset</span></span>|<span data-ttu-id="148e8-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-149">version</span><span class="sxs-lookup"><span data-stu-id="148e8-149">version</span></span>|<span data-ttu-id="148e8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="148e8-150">Int32</span></span>|<span data-ttu-id="148e8-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148e8-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="148e8-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-152">iosRestriction</span></span>|[<span data-ttu-id="148e8-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="148e8-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="148e8-154">Not yet documented</span></span>|
|<span data-ttu-id="148e8-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-155">windowsRestriction</span></span>|[<span data-ttu-id="148e8-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="148e8-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="148e8-157">Not yet documented</span></span>|
|<span data-ttu-id="148e8-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="148e8-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="148e8-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="148e8-160">Not yet documented</span></span>|
|<span data-ttu-id="148e8-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-161">androidRestriction</span></span>|[<span data-ttu-id="148e8-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="148e8-163">尚未记录</span><span class="sxs-lookup"><span data-stu-id="148e8-163">Not yet documented</span></span>|
|<span data-ttu-id="148e8-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-164">macOSRestriction</span></span>|[<span data-ttu-id="148e8-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="148e8-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="148e8-166">尚未记录</span><span class="sxs-lookup"><span data-stu-id="148e8-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="148e8-167">响应</span><span class="sxs-lookup"><span data-stu-id="148e8-167">Response</span></span>
<span data-ttu-id="148e8-168">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="148e8-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="148e8-169">示例</span><span class="sxs-lookup"><span data-stu-id="148e8-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="148e8-170">请求</span><span class="sxs-lookup"><span data-stu-id="148e8-170">Request</span></span>
<span data-ttu-id="148e8-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="148e8-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="148e8-172">响应</span><span class="sxs-lookup"><span data-stu-id="148e8-172">Response</span></span>
<span data-ttu-id="148e8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="148e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



