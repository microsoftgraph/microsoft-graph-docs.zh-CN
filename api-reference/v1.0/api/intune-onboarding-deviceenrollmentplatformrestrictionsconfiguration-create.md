---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9bbac90b39141d201792f78dcc9883bc1eb23d2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033186"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="3bb14-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bb14-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="3bb14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bb14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bb14-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bb14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bb14-106">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bb14-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bb14-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3bb14-107">Prerequisites</span></span>
<span data-ttu-id="3bb14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bb14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bb14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bb14-110">Permission type</span></span>|<span data-ttu-id="3bb14-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3bb14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bb14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bb14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3bb14-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb14-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3bb14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bb14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bb14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bb14-115">Not supported.</span></span>|
|<span data-ttu-id="3bb14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bb14-116">Application</span></span>|<span data-ttu-id="3bb14-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bb14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bb14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bb14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3bb14-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bb14-119">Request headers</span></span>
|<span data-ttu-id="3bb14-120">标头</span><span class="sxs-lookup"><span data-stu-id="3bb14-120">Header</span></span>|<span data-ttu-id="3bb14-121">值</span><span class="sxs-lookup"><span data-stu-id="3bb14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bb14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bb14-122">Authorization</span></span>|<span data-ttu-id="3bb14-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3bb14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bb14-124">接受</span><span class="sxs-lookup"><span data-stu-id="3bb14-124">Accept</span></span>|<span data-ttu-id="3bb14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bb14-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bb14-126">Request body</span></span>
<span data-ttu-id="3bb14-127">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bb14-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="3bb14-128">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3bb14-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="3bb14-129">属性</span><span class="sxs-lookup"><span data-stu-id="3bb14-129">Property</span></span>|<span data-ttu-id="3bb14-130">类型</span><span class="sxs-lookup"><span data-stu-id="3bb14-130">Type</span></span>|<span data-ttu-id="3bb14-131">说明</span><span class="sxs-lookup"><span data-stu-id="3bb14-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bb14-132">id</span><span class="sxs-lookup"><span data-stu-id="3bb14-132">id</span></span>|<span data-ttu-id="3bb14-133">String</span><span class="sxs-lookup"><span data-stu-id="3bb14-133">String</span></span>|<span data-ttu-id="3bb14-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3bb14-135">displayName</span></span>|<span data-ttu-id="3bb14-136">String</span><span class="sxs-lookup"><span data-stu-id="3bb14-136">String</span></span>|<span data-ttu-id="3bb14-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-138">description</span><span class="sxs-lookup"><span data-stu-id="3bb14-138">description</span></span>|<span data-ttu-id="3bb14-139">String</span><span class="sxs-lookup"><span data-stu-id="3bb14-139">String</span></span>|<span data-ttu-id="3bb14-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-141">priority</span><span class="sxs-lookup"><span data-stu-id="3bb14-141">priority</span></span>|<span data-ttu-id="3bb14-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3bb14-142">Int32</span></span>|<span data-ttu-id="3bb14-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bb14-144">createdDateTime</span></span>|<span data-ttu-id="3bb14-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bb14-145">DateTimeOffset</span></span>|<span data-ttu-id="3bb14-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bb14-147">lastModifiedDateTime</span></span>|<span data-ttu-id="3bb14-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bb14-148">DateTimeOffset</span></span>|<span data-ttu-id="3bb14-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-150">version</span><span class="sxs-lookup"><span data-stu-id="3bb14-150">version</span></span>|<span data-ttu-id="3bb14-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3bb14-151">Int32</span></span>|<span data-ttu-id="3bb14-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb14-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bb14-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-153">iosRestriction</span></span>|[<span data-ttu-id="3bb14-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3bb14-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3bb14-155">Not yet documented</span></span>|
|<span data-ttu-id="3bb14-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-156">windowsRestriction</span></span>|[<span data-ttu-id="3bb14-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3bb14-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3bb14-158">Not yet documented</span></span>|
|<span data-ttu-id="3bb14-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="3bb14-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3bb14-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3bb14-161">Not yet documented</span></span>|
|<span data-ttu-id="3bb14-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-162">androidRestriction</span></span>|[<span data-ttu-id="3bb14-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3bb14-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3bb14-164">Not yet documented</span></span>|
|<span data-ttu-id="3bb14-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-165">macOSRestriction</span></span>|[<span data-ttu-id="3bb14-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3bb14-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3bb14-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3bb14-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3bb14-168">响应</span><span class="sxs-lookup"><span data-stu-id="3bb14-168">Response</span></span>
<span data-ttu-id="3bb14-169">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bb14-169">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bb14-170">示例</span><span class="sxs-lookup"><span data-stu-id="3bb14-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bb14-171">请求</span><span class="sxs-lookup"><span data-stu-id="3bb14-171">Request</span></span>
<span data-ttu-id="3bb14-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bb14-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3bb14-173">响应</span><span class="sxs-lookup"><span data-stu-id="3bb14-173">Response</span></span>
<span data-ttu-id="3bb14-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3bb14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









