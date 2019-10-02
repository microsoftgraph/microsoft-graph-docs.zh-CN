---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2894b6cd7f753399fab696772bb8a2a2ebf91e3f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362630"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="5193f-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="5193f-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="5193f-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5193f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5193f-105">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5193f-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5193f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5193f-106">Prerequisites</span></span>
<span data-ttu-id="5193f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5193f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5193f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5193f-109">Permission type</span></span>|<span data-ttu-id="5193f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5193f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5193f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5193f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5193f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5193f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5193f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5193f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5193f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5193f-114">Not supported.</span></span>|
|<span data-ttu-id="5193f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5193f-115">Application</span></span>|<span data-ttu-id="5193f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5193f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5193f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5193f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5193f-118">请求头</span><span class="sxs-lookup"><span data-stu-id="5193f-118">Request headers</span></span>
|<span data-ttu-id="5193f-119">标头</span><span class="sxs-lookup"><span data-stu-id="5193f-119">Header</span></span>|<span data-ttu-id="5193f-120">值</span><span class="sxs-lookup"><span data-stu-id="5193f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5193f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5193f-121">Authorization</span></span>|<span data-ttu-id="5193f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5193f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5193f-123">接受</span><span class="sxs-lookup"><span data-stu-id="5193f-123">Accept</span></span>|<span data-ttu-id="5193f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5193f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5193f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5193f-125">Request body</span></span>
<span data-ttu-id="5193f-126">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5193f-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="5193f-127">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5193f-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="5193f-128">属性</span><span class="sxs-lookup"><span data-stu-id="5193f-128">Property</span></span>|<span data-ttu-id="5193f-129">类型</span><span class="sxs-lookup"><span data-stu-id="5193f-129">Type</span></span>|<span data-ttu-id="5193f-130">说明</span><span class="sxs-lookup"><span data-stu-id="5193f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5193f-131">id</span><span class="sxs-lookup"><span data-stu-id="5193f-131">id</span></span>|<span data-ttu-id="5193f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="5193f-132">String</span></span>|<span data-ttu-id="5193f-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5193f-134">displayName</span></span>|<span data-ttu-id="5193f-135">String</span><span class="sxs-lookup"><span data-stu-id="5193f-135">String</span></span>|<span data-ttu-id="5193f-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-137">说明</span><span class="sxs-lookup"><span data-stu-id="5193f-137">description</span></span>|<span data-ttu-id="5193f-138">String</span><span class="sxs-lookup"><span data-stu-id="5193f-138">String</span></span>|<span data-ttu-id="5193f-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-140">priority</span><span class="sxs-lookup"><span data-stu-id="5193f-140">priority</span></span>|<span data-ttu-id="5193f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5193f-141">Int32</span></span>|<span data-ttu-id="5193f-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5193f-143">createdDateTime</span></span>|<span data-ttu-id="5193f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5193f-144">DateTimeOffset</span></span>|<span data-ttu-id="5193f-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5193f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="5193f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5193f-147">DateTimeOffset</span></span>|<span data-ttu-id="5193f-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-149">version</span><span class="sxs-lookup"><span data-stu-id="5193f-149">version</span></span>|<span data-ttu-id="5193f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5193f-150">Int32</span></span>|<span data-ttu-id="5193f-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5193f-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5193f-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-152">iosRestriction</span></span>|[<span data-ttu-id="5193f-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5193f-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5193f-154">Not yet documented</span></span>|
|<span data-ttu-id="5193f-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-155">windowsRestriction</span></span>|[<span data-ttu-id="5193f-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5193f-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5193f-157">Not yet documented</span></span>|
|<span data-ttu-id="5193f-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="5193f-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5193f-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5193f-160">Not yet documented</span></span>|
|<span data-ttu-id="5193f-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-161">androidRestriction</span></span>|[<span data-ttu-id="5193f-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5193f-163">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5193f-163">Not yet documented</span></span>|
|<span data-ttu-id="5193f-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-164">macOSRestriction</span></span>|[<span data-ttu-id="5193f-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5193f-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5193f-166">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5193f-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5193f-167">响应</span><span class="sxs-lookup"><span data-stu-id="5193f-167">Response</span></span>
<span data-ttu-id="5193f-168">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5193f-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5193f-169">示例</span><span class="sxs-lookup"><span data-stu-id="5193f-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="5193f-170">请求</span><span class="sxs-lookup"><span data-stu-id="5193f-170">Request</span></span>
<span data-ttu-id="5193f-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5193f-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5193f-172">响应</span><span class="sxs-lookup"><span data-stu-id="5193f-172">Response</span></span>
<span data-ttu-id="5193f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5193f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




