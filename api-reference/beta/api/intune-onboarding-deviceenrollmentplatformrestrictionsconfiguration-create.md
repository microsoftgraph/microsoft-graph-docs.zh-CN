---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
ms.openlocfilehash: e28bea6cc182684ec10abddf97801772c111bf0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043848"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="451e1-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="451e1-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="451e1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="451e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="451e1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="451e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="451e1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="451e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="451e1-107">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="451e1-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="451e1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="451e1-108">Prerequisites</span></span>
<span data-ttu-id="451e1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="451e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="451e1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="451e1-111">Permission type</span></span>|<span data-ttu-id="451e1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="451e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="451e1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="451e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="451e1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="451e1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="451e1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="451e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="451e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="451e1-116">Not supported.</span></span>|
|<span data-ttu-id="451e1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="451e1-117">Application</span></span>|<span data-ttu-id="451e1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="451e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="451e1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="451e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="451e1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="451e1-120">Request headers</span></span>
|<span data-ttu-id="451e1-121">标头</span><span class="sxs-lookup"><span data-stu-id="451e1-121">Header</span></span>|<span data-ttu-id="451e1-122">值</span><span class="sxs-lookup"><span data-stu-id="451e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="451e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="451e1-123">Authorization</span></span>|<span data-ttu-id="451e1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="451e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="451e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="451e1-125">Accept</span></span>|<span data-ttu-id="451e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="451e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="451e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="451e1-127">Request body</span></span>
<span data-ttu-id="451e1-128">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="451e1-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="451e1-129">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="451e1-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="451e1-130">属性</span><span class="sxs-lookup"><span data-stu-id="451e1-130">Property</span></span>|<span data-ttu-id="451e1-131">类型</span><span class="sxs-lookup"><span data-stu-id="451e1-131">Type</span></span>|<span data-ttu-id="451e1-132">说明</span><span class="sxs-lookup"><span data-stu-id="451e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="451e1-133">id</span><span class="sxs-lookup"><span data-stu-id="451e1-133">id</span></span>|<span data-ttu-id="451e1-134">String</span><span class="sxs-lookup"><span data-stu-id="451e1-134">String</span></span>|<span data-ttu-id="451e1-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="451e1-136">displayName</span></span>|<span data-ttu-id="451e1-137">String</span><span class="sxs-lookup"><span data-stu-id="451e1-137">String</span></span>|<span data-ttu-id="451e1-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-139">description</span><span class="sxs-lookup"><span data-stu-id="451e1-139">description</span></span>|<span data-ttu-id="451e1-140">String</span><span class="sxs-lookup"><span data-stu-id="451e1-140">String</span></span>|<span data-ttu-id="451e1-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-142">priority</span><span class="sxs-lookup"><span data-stu-id="451e1-142">priority</span></span>|<span data-ttu-id="451e1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="451e1-143">Int32</span></span>|<span data-ttu-id="451e1-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="451e1-145">createdDateTime</span></span>|<span data-ttu-id="451e1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="451e1-146">DateTimeOffset</span></span>|<span data-ttu-id="451e1-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="451e1-148">lastModifiedDateTime</span></span>|<span data-ttu-id="451e1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="451e1-149">DateTimeOffset</span></span>|<span data-ttu-id="451e1-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-151">version</span><span class="sxs-lookup"><span data-stu-id="451e1-151">version</span></span>|<span data-ttu-id="451e1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="451e1-152">Int32</span></span>|<span data-ttu-id="451e1-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="451e1-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="451e1-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-154">iosRestriction</span></span>|[<span data-ttu-id="451e1-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-156">Not yet documented</span></span>|
|<span data-ttu-id="451e1-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-157">windowsRestriction</span></span>|[<span data-ttu-id="451e1-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-159">Not yet documented</span></span>|
|<span data-ttu-id="451e1-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="451e1-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-162">Not yet documented</span></span>|
|<span data-ttu-id="451e1-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-163">androidRestriction</span></span>|[<span data-ttu-id="451e1-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-165">Not yet documented</span></span>|
|<span data-ttu-id="451e1-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="451e1-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-168">Not yet documented</span></span>|
|<span data-ttu-id="451e1-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-169">macRestriction</span></span>|[<span data-ttu-id="451e1-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-171">Not yet documented</span></span>|
|<span data-ttu-id="451e1-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-172">macOSRestriction</span></span>|[<span data-ttu-id="451e1-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="451e1-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="451e1-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="451e1-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="451e1-175">响应</span><span class="sxs-lookup"><span data-stu-id="451e1-175">Response</span></span>
<span data-ttu-id="451e1-176">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="451e1-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="451e1-177">示例</span><span class="sxs-lookup"><span data-stu-id="451e1-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="451e1-178">请求</span><span class="sxs-lookup"><span data-stu-id="451e1-178">Request</span></span>
<span data-ttu-id="451e1-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="451e1-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 2295

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="451e1-180">响应</span><span class="sxs-lookup"><span data-stu-id="451e1-180">Response</span></span>
<span data-ttu-id="451e1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="451e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





