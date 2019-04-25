---
title: 创建 deviceEnrollmentPlatformRestrictionsConfiguration
description: 创建新的 deviceEnrollmentPlatformRestrictionsConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 204b18b654e8cc13e1808d27643cd477d188a0b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561675"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="06950-103">创建 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="06950-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="06950-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06950-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06950-105">创建新的 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06950-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06950-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="06950-106">Prerequisites</span></span>
<span data-ttu-id="06950-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06950-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06950-109">Permission type</span></span>|<span data-ttu-id="06950-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06950-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06950-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06950-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06950-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06950-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="06950-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06950-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06950-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06950-114">Not supported.</span></span>|
|<span data-ttu-id="06950-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06950-115">Application</span></span>|<span data-ttu-id="06950-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06950-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06950-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06950-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06950-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="06950-118">Request headers</span></span>
|<span data-ttu-id="06950-119">标头</span><span class="sxs-lookup"><span data-stu-id="06950-119">Header</span></span>|<span data-ttu-id="06950-120">值</span><span class="sxs-lookup"><span data-stu-id="06950-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06950-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06950-121">Authorization</span></span>|<span data-ttu-id="06950-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06950-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06950-123">接受</span><span class="sxs-lookup"><span data-stu-id="06950-123">Accept</span></span>|<span data-ttu-id="06950-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06950-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06950-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="06950-125">Request body</span></span>
<span data-ttu-id="06950-126">在请求正文中，提供 deviceEnrollmentPlatformRestrictionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06950-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="06950-127">下表显示创建 deviceEnrollmentPlatformRestrictionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06950-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="06950-128">属性</span><span class="sxs-lookup"><span data-stu-id="06950-128">Property</span></span>|<span data-ttu-id="06950-129">类型</span><span class="sxs-lookup"><span data-stu-id="06950-129">Type</span></span>|<span data-ttu-id="06950-130">说明</span><span class="sxs-lookup"><span data-stu-id="06950-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06950-131">id</span><span class="sxs-lookup"><span data-stu-id="06950-131">id</span></span>|<span data-ttu-id="06950-132">字符串</span><span class="sxs-lookup"><span data-stu-id="06950-132">String</span></span>|<span data-ttu-id="06950-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-134">displayName</span><span class="sxs-lookup"><span data-stu-id="06950-134">displayName</span></span>|<span data-ttu-id="06950-135">String</span><span class="sxs-lookup"><span data-stu-id="06950-135">String</span></span>|<span data-ttu-id="06950-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-137">description</span><span class="sxs-lookup"><span data-stu-id="06950-137">description</span></span>|<span data-ttu-id="06950-138">String</span><span class="sxs-lookup"><span data-stu-id="06950-138">String</span></span>|<span data-ttu-id="06950-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-140">priority</span><span class="sxs-lookup"><span data-stu-id="06950-140">priority</span></span>|<span data-ttu-id="06950-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06950-141">Int32</span></span>|<span data-ttu-id="06950-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06950-143">createdDateTime</span></span>|<span data-ttu-id="06950-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06950-144">DateTimeOffset</span></span>|<span data-ttu-id="06950-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06950-146">lastModifiedDateTime</span></span>|<span data-ttu-id="06950-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06950-147">DateTimeOffset</span></span>|<span data-ttu-id="06950-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-149">version</span><span class="sxs-lookup"><span data-stu-id="06950-149">version</span></span>|<span data-ttu-id="06950-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06950-150">Int32</span></span>|<span data-ttu-id="06950-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06950-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06950-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-152">iosRestriction</span></span>|[<span data-ttu-id="06950-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06950-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06950-154">Not yet documented</span></span>|
|<span data-ttu-id="06950-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-155">windowsRestriction</span></span>|[<span data-ttu-id="06950-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06950-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06950-157">Not yet documented</span></span>|
|<span data-ttu-id="06950-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="06950-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06950-160">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06950-160">Not yet documented</span></span>|
|<span data-ttu-id="06950-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-161">androidRestriction</span></span>|[<span data-ttu-id="06950-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06950-163">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06950-163">Not yet documented</span></span>|
|<span data-ttu-id="06950-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-164">macOSRestriction</span></span>|[<span data-ttu-id="06950-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06950-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="06950-166">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06950-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06950-167">响应</span><span class="sxs-lookup"><span data-stu-id="06950-167">Response</span></span>
<span data-ttu-id="06950-168">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06950-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06950-169">示例</span><span class="sxs-lookup"><span data-stu-id="06950-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="06950-170">请求</span><span class="sxs-lookup"><span data-stu-id="06950-170">Request</span></span>
<span data-ttu-id="06950-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06950-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06950-172">响应</span><span class="sxs-lookup"><span data-stu-id="06950-172">Response</span></span>
<span data-ttu-id="06950-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06950-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



