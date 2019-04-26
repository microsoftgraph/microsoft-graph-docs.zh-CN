---
title: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3225f7fe36f5ec8a66df8424a06d8569b7c92efd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561626"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="0e9b7-103">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e9b7-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="0e9b7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e9b7-105">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e9b7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e9b7-106">Prerequisites</span></span>
<span data-ttu-id="0e9b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e9b7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e9b7-109">Permission type</span></span>|<span data-ttu-id="0e9b7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e9b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e9b7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e9b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e9b7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e9b7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0e9b7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e9b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e9b7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-114">Not supported.</span></span>|
|<span data-ttu-id="0e9b7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e9b7-115">Application</span></span>|<span data-ttu-id="0e9b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e9b7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e9b7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0e9b7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e9b7-118">Request headers</span></span>
|<span data-ttu-id="0e9b7-119">标头</span><span class="sxs-lookup"><span data-stu-id="0e9b7-119">Header</span></span>|<span data-ttu-id="0e9b7-120">值</span><span class="sxs-lookup"><span data-stu-id="0e9b7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e9b7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e9b7-121">Authorization</span></span>|<span data-ttu-id="0e9b7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e9b7-123">接受</span><span class="sxs-lookup"><span data-stu-id="0e9b7-123">Accept</span></span>|<span data-ttu-id="0e9b7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e9b7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e9b7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e9b7-125">Request body</span></span>
<span data-ttu-id="0e9b7-126">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="0e9b7-127">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="0e9b7-128">属性</span><span class="sxs-lookup"><span data-stu-id="0e9b7-128">Property</span></span>|<span data-ttu-id="0e9b7-129">类型</span><span class="sxs-lookup"><span data-stu-id="0e9b7-129">Type</span></span>|<span data-ttu-id="0e9b7-130">说明</span><span class="sxs-lookup"><span data-stu-id="0e9b7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e9b7-131">id</span><span class="sxs-lookup"><span data-stu-id="0e9b7-131">id</span></span>|<span data-ttu-id="0e9b7-132">字符串</span><span class="sxs-lookup"><span data-stu-id="0e9b7-132">String</span></span>|<span data-ttu-id="0e9b7-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0e9b7-134">displayName</span></span>|<span data-ttu-id="0e9b7-135">String</span><span class="sxs-lookup"><span data-stu-id="0e9b7-135">String</span></span>|<span data-ttu-id="0e9b7-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-137">description</span><span class="sxs-lookup"><span data-stu-id="0e9b7-137">description</span></span>|<span data-ttu-id="0e9b7-138">String</span><span class="sxs-lookup"><span data-stu-id="0e9b7-138">String</span></span>|<span data-ttu-id="0e9b7-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-140">priority</span><span class="sxs-lookup"><span data-stu-id="0e9b7-140">priority</span></span>|<span data-ttu-id="0e9b7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9b7-141">Int32</span></span>|<span data-ttu-id="0e9b7-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e9b7-143">createdDateTime</span></span>|<span data-ttu-id="0e9b7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e9b7-144">DateTimeOffset</span></span>|<span data-ttu-id="0e9b7-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e9b7-146">lastModifiedDateTime</span></span>|<span data-ttu-id="0e9b7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e9b7-147">DateTimeOffset</span></span>|<span data-ttu-id="0e9b7-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-149">version</span><span class="sxs-lookup"><span data-stu-id="0e9b7-149">version</span></span>|<span data-ttu-id="0e9b7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9b7-150">Int32</span></span>|<span data-ttu-id="0e9b7-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e9b7-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e9b7-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0e9b7-152">pinMinimumLength</span></span>|<span data-ttu-id="0e9b7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9b7-153">Int32</span></span>|<span data-ttu-id="0e9b7-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-154">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="0e9b7-155">pinMaximumLength</span></span>|<span data-ttu-id="0e9b7-156">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9b7-156">Int32</span></span>|<span data-ttu-id="0e9b7-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-157">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0e9b7-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="0e9b7-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="0e9b7-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="0e9b7-160">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-160">Not yet documented.</span></span> <span data-ttu-id="0e9b7-161">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0e9b7-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0e9b7-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="0e9b7-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="0e9b7-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="0e9b7-164">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-164">Not yet documented.</span></span> <span data-ttu-id="0e9b7-165">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0e9b7-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0e9b7-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="0e9b7-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="0e9b7-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="0e9b7-168">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-168">Not yet documented.</span></span> <span data-ttu-id="0e9b7-169">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0e9b7-170">state</span><span class="sxs-lookup"><span data-stu-id="0e9b7-170">state</span></span>|[<span data-ttu-id="0e9b7-171">启用</span><span class="sxs-lookup"><span data-stu-id="0e9b7-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="0e9b7-172">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-172">Not yet documented.</span></span> <span data-ttu-id="0e9b7-173">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0e9b7-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="0e9b7-174">securityDeviceRequired</span></span>|<span data-ttu-id="0e9b7-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e9b7-175">Boolean</span></span>|<span data-ttu-id="0e9b7-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-176">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="0e9b7-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="0e9b7-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e9b7-178">Boolean</span></span>|<span data-ttu-id="0e9b7-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-179">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="0e9b7-180">remotePassportEnabled</span></span>|<span data-ttu-id="0e9b7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e9b7-181">Boolean</span></span>|<span data-ttu-id="0e9b7-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-182">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="0e9b7-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="0e9b7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9b7-184">Int32</span></span>|<span data-ttu-id="0e9b7-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-185">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="0e9b7-186">pinExpirationInDays</span></span>|<span data-ttu-id="0e9b7-187">Int32</span><span class="sxs-lookup"><span data-stu-id="0e9b7-187">Int32</span></span>|<span data-ttu-id="0e9b7-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9b7-188">Not yet documented</span></span>|
|<span data-ttu-id="0e9b7-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="0e9b7-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="0e9b7-190">启用</span><span class="sxs-lookup"><span data-stu-id="0e9b7-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="0e9b7-191">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-191">Not yet documented.</span></span> <span data-ttu-id="0e9b7-192">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="0e9b7-193">响应</span><span class="sxs-lookup"><span data-stu-id="0e9b7-193">Response</span></span>
<span data-ttu-id="0e9b7-194">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e9b7-195">示例</span><span class="sxs-lookup"><span data-stu-id="0e9b7-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e9b7-196">请求</span><span class="sxs-lookup"><span data-stu-id="0e9b7-196">Request</span></span>
<span data-ttu-id="0e9b7-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="0e9b7-198">响应</span><span class="sxs-lookup"><span data-stu-id="0e9b7-198">Response</span></span>
<span data-ttu-id="0e9b7-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e9b7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```



