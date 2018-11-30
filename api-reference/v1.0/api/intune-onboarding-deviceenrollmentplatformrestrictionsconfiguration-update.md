---
title: 更新 deviceEnrollmentPlatformRestrictionsConfiguration
description: 更新 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性。
ms.openlocfilehash: 2f78952d3eeae8f88e66ca1b5441141b7172153f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007809"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="45906-103">更新 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="45906-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="45906-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45906-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45906-105">更新 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="45906-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45906-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="45906-106">Prerequisites</span></span>
<span data-ttu-id="45906-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="45906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45906-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45906-109">Permission type</span></span>|<span data-ttu-id="45906-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45906-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45906-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45906-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45906-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45906-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45906-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45906-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45906-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45906-114">Not supported.</span></span>|
|<span data-ttu-id="45906-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45906-115">Application</span></span>|<span data-ttu-id="45906-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45906-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45906-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45906-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="45906-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="45906-118">Request headers</span></span>
|<span data-ttu-id="45906-119">标头</span><span class="sxs-lookup"><span data-stu-id="45906-119">Header</span></span>|<span data-ttu-id="45906-120">值</span><span class="sxs-lookup"><span data-stu-id="45906-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45906-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45906-121">Authorization</span></span>|<span data-ttu-id="45906-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45906-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45906-123">Accept</span><span class="sxs-lookup"><span data-stu-id="45906-123">Accept</span></span>|<span data-ttu-id="45906-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45906-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45906-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="45906-125">Request body</span></span>
<span data-ttu-id="45906-126">在请求正文中，提供 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45906-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="45906-127">下表显示创建 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="45906-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="45906-128">属性</span><span class="sxs-lookup"><span data-stu-id="45906-128">Property</span></span>|<span data-ttu-id="45906-129">类型</span><span class="sxs-lookup"><span data-stu-id="45906-129">Type</span></span>|<span data-ttu-id="45906-130">说明</span><span class="sxs-lookup"><span data-stu-id="45906-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45906-131">id</span><span class="sxs-lookup"><span data-stu-id="45906-131">id</span></span>|<span data-ttu-id="45906-132">String</span><span class="sxs-lookup"><span data-stu-id="45906-132">String</span></span>|<span data-ttu-id="45906-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-134">displayName</span><span class="sxs-lookup"><span data-stu-id="45906-134">displayName</span></span>|<span data-ttu-id="45906-135">String</span><span class="sxs-lookup"><span data-stu-id="45906-135">String</span></span>|<span data-ttu-id="45906-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-137">description</span><span class="sxs-lookup"><span data-stu-id="45906-137">description</span></span>|<span data-ttu-id="45906-138">String</span><span class="sxs-lookup"><span data-stu-id="45906-138">String</span></span>|<span data-ttu-id="45906-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-140">priority</span><span class="sxs-lookup"><span data-stu-id="45906-140">priority</span></span>|<span data-ttu-id="45906-141">Int32</span><span class="sxs-lookup"><span data-stu-id="45906-141">Int32</span></span>|<span data-ttu-id="45906-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45906-143">createdDateTime</span></span>|<span data-ttu-id="45906-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45906-144">DateTimeOffset</span></span>|<span data-ttu-id="45906-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45906-146">lastModifiedDateTime</span></span>|<span data-ttu-id="45906-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45906-147">DateTimeOffset</span></span>|<span data-ttu-id="45906-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-149">version</span><span class="sxs-lookup"><span data-stu-id="45906-149">version</span></span>|<span data-ttu-id="45906-150">Int32</span><span class="sxs-lookup"><span data-stu-id="45906-150">Int32</span></span>|<span data-ttu-id="45906-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45906-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="45906-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-152">iosRestriction</span></span>|[<span data-ttu-id="45906-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="45906-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45906-154">Not yet documented</span></span>|
|<span data-ttu-id="45906-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-155">windowsRestriction</span></span>|[<span data-ttu-id="45906-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="45906-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45906-157">Not yet documented</span></span>|
|<span data-ttu-id="45906-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="45906-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="45906-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45906-160">Not yet documented</span></span>|
|<span data-ttu-id="45906-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-161">androidRestriction</span></span>|[<span data-ttu-id="45906-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="45906-163">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45906-163">Not yet documented</span></span>|
|<span data-ttu-id="45906-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-164">macOSRestriction</span></span>|[<span data-ttu-id="45906-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="45906-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="45906-166">尚未记录</span><span class="sxs-lookup"><span data-stu-id="45906-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45906-167">响应</span><span class="sxs-lookup"><span data-stu-id="45906-167">Response</span></span>
<span data-ttu-id="45906-168">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45906-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45906-169">示例</span><span class="sxs-lookup"><span data-stu-id="45906-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="45906-170">请求</span><span class="sxs-lookup"><span data-stu-id="45906-170">Request</span></span>
<span data-ttu-id="45906-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45906-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45906-172">响应</span><span class="sxs-lookup"><span data-stu-id="45906-172">Response</span></span>
<span data-ttu-id="45906-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45906-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



