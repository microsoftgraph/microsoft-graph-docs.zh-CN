---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28a59aad2d47c87a2a8eafc25d3def37b60fee92
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874604"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="9c994-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c994-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="9c994-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c994-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c994-105">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c994-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c994-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c994-106">Prerequisites</span></span>
<span data-ttu-id="9c994-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9c994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c994-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c994-109">Permission type</span></span>|<span data-ttu-id="9c994-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c994-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c994-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c994-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c994-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c994-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9c994-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c994-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c994-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c994-114">Not supported.</span></span>|
|<span data-ttu-id="9c994-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c994-115">Application</span></span>|<span data-ttu-id="9c994-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c994-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c994-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c994-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9c994-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c994-118">Request headers</span></span>
|<span data-ttu-id="9c994-119">标头</span><span class="sxs-lookup"><span data-stu-id="9c994-119">Header</span></span>|<span data-ttu-id="9c994-120">值</span><span class="sxs-lookup"><span data-stu-id="9c994-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c994-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c994-121">Authorization</span></span>|<span data-ttu-id="9c994-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c994-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c994-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9c994-123">Accept</span></span>|<span data-ttu-id="9c994-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9c994-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c994-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c994-125">Request body</span></span>
<span data-ttu-id="9c994-126">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c994-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="9c994-127">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c994-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="9c994-128">属性</span><span class="sxs-lookup"><span data-stu-id="9c994-128">Property</span></span>|<span data-ttu-id="9c994-129">类型</span><span class="sxs-lookup"><span data-stu-id="9c994-129">Type</span></span>|<span data-ttu-id="9c994-130">说明</span><span class="sxs-lookup"><span data-stu-id="9c994-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c994-131">id</span><span class="sxs-lookup"><span data-stu-id="9c994-131">id</span></span>|<span data-ttu-id="9c994-132">String</span><span class="sxs-lookup"><span data-stu-id="9c994-132">String</span></span>|<span data-ttu-id="9c994-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9c994-134">displayName</span></span>|<span data-ttu-id="9c994-135">String</span><span class="sxs-lookup"><span data-stu-id="9c994-135">String</span></span>|<span data-ttu-id="9c994-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-137">description</span><span class="sxs-lookup"><span data-stu-id="9c994-137">description</span></span>|<span data-ttu-id="9c994-138">String</span><span class="sxs-lookup"><span data-stu-id="9c994-138">String</span></span>|<span data-ttu-id="9c994-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-140">priority</span><span class="sxs-lookup"><span data-stu-id="9c994-140">priority</span></span>|<span data-ttu-id="9c994-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9c994-141">Int32</span></span>|<span data-ttu-id="9c994-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c994-143">createdDateTime</span></span>|<span data-ttu-id="9c994-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c994-144">DateTimeOffset</span></span>|<span data-ttu-id="9c994-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c994-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9c994-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c994-147">DateTimeOffset</span></span>|<span data-ttu-id="9c994-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-149">version</span><span class="sxs-lookup"><span data-stu-id="9c994-149">version</span></span>|<span data-ttu-id="9c994-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9c994-150">Int32</span></span>|<span data-ttu-id="9c994-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c994-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9c994-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-152">iosRestriction</span></span>|[<span data-ttu-id="9c994-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9c994-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9c994-154">Not yet documented</span></span>|
|<span data-ttu-id="9c994-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-155">windowsRestriction</span></span>|[<span data-ttu-id="9c994-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9c994-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9c994-157">Not yet documented</span></span>|
|<span data-ttu-id="9c994-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="9c994-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9c994-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9c994-160">Not yet documented</span></span>|
|<span data-ttu-id="9c994-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-161">androidRestriction</span></span>|[<span data-ttu-id="9c994-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9c994-163">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9c994-163">Not yet documented</span></span>|
|<span data-ttu-id="9c994-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-164">macOSRestriction</span></span>|[<span data-ttu-id="9c994-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9c994-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9c994-166">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9c994-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c994-167">响应</span><span class="sxs-lookup"><span data-stu-id="9c994-167">Response</span></span>
<span data-ttu-id="9c994-168">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c994-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c994-169">示例</span><span class="sxs-lookup"><span data-stu-id="9c994-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c994-170">请求</span><span class="sxs-lookup"><span data-stu-id="9c994-170">Request</span></span>
<span data-ttu-id="9c994-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c994-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c994-172">响应</span><span class="sxs-lookup"><span data-stu-id="9c994-172">Response</span></span>
<span data-ttu-id="9c994-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c994-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



