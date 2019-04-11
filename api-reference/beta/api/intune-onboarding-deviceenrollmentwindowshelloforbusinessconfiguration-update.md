---
title: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44a938e652ba71c6d18846a6a4e85a87b7653ca8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796498"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="27e37-103">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="27e37-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="27e37-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27e37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27e37-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27e37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27e37-106">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27e37-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27e37-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="27e37-107">Prerequisites</span></span>
<span data-ttu-id="27e37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27e37-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27e37-110">Permission type</span></span>|<span data-ttu-id="27e37-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27e37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27e37-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27e37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27e37-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e37-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27e37-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27e37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27e37-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27e37-115">Not supported.</span></span>|
|<span data-ttu-id="27e37-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="27e37-116">Application</span></span>|<span data-ttu-id="27e37-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="27e37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27e37-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27e37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="27e37-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="27e37-119">Request headers</span></span>
|<span data-ttu-id="27e37-120">标头</span><span class="sxs-lookup"><span data-stu-id="27e37-120">Header</span></span>|<span data-ttu-id="27e37-121">值</span><span class="sxs-lookup"><span data-stu-id="27e37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27e37-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27e37-122">Authorization</span></span>|<span data-ttu-id="27e37-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27e37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27e37-124">接受</span><span class="sxs-lookup"><span data-stu-id="27e37-124">Accept</span></span>|<span data-ttu-id="27e37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27e37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e37-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="27e37-126">Request body</span></span>
<span data-ttu-id="27e37-127">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27e37-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="27e37-128">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27e37-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="27e37-129">属性</span><span class="sxs-lookup"><span data-stu-id="27e37-129">Property</span></span>|<span data-ttu-id="27e37-130">类型</span><span class="sxs-lookup"><span data-stu-id="27e37-130">Type</span></span>|<span data-ttu-id="27e37-131">说明</span><span class="sxs-lookup"><span data-stu-id="27e37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27e37-132">id</span><span class="sxs-lookup"><span data-stu-id="27e37-132">id</span></span>|<span data-ttu-id="27e37-133">String</span><span class="sxs-lookup"><span data-stu-id="27e37-133">String</span></span>|<span data-ttu-id="27e37-134">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的注册状态页面配置的 Id</span><span class="sxs-lookup"><span data-stu-id="27e37-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-135">displayName</span><span class="sxs-lookup"><span data-stu-id="27e37-135">displayName</span></span>|<span data-ttu-id="27e37-136">String</span><span class="sxs-lookup"><span data-stu-id="27e37-136">String</span></span>|<span data-ttu-id="27e37-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27e37-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-138">description</span><span class="sxs-lookup"><span data-stu-id="27e37-138">description</span></span>|<span data-ttu-id="27e37-139">String</span><span class="sxs-lookup"><span data-stu-id="27e37-139">String</span></span>|<span data-ttu-id="27e37-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27e37-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-141">priority</span><span class="sxs-lookup"><span data-stu-id="27e37-141">priority</span></span>|<span data-ttu-id="27e37-142">Int32</span><span class="sxs-lookup"><span data-stu-id="27e37-142">Int32</span></span>|<span data-ttu-id="27e37-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27e37-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27e37-144">createdDateTime</span></span>|<span data-ttu-id="27e37-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27e37-145">DateTimeOffset</span></span>|<span data-ttu-id="27e37-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27e37-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27e37-147">lastModifiedDateTime</span></span>|<span data-ttu-id="27e37-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27e37-148">DateTimeOffset</span></span>|<span data-ttu-id="27e37-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27e37-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-150">version</span><span class="sxs-lookup"><span data-stu-id="27e37-150">version</span></span>|<span data-ttu-id="27e37-151">Int32</span><span class="sxs-lookup"><span data-stu-id="27e37-151">Int32</span></span>|<span data-ttu-id="27e37-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27e37-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27e37-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="27e37-153">pinMinimumLength</span></span>|<span data-ttu-id="27e37-154">Int32</span><span class="sxs-lookup"><span data-stu-id="27e37-154">Int32</span></span>|<span data-ttu-id="27e37-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-155">Not yet documented</span></span>|
|<span data-ttu-id="27e37-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="27e37-156">pinMaximumLength</span></span>|<span data-ttu-id="27e37-157">Int32</span><span class="sxs-lookup"><span data-stu-id="27e37-157">Int32</span></span>|<span data-ttu-id="27e37-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-158">Not yet documented</span></span>|
|<span data-ttu-id="27e37-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="27e37-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="27e37-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="27e37-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="27e37-161">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="27e37-161">Not yet documented.</span></span> <span data-ttu-id="27e37-162">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="27e37-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="27e37-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="27e37-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="27e37-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="27e37-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="27e37-165">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="27e37-165">Not yet documented.</span></span> <span data-ttu-id="27e37-166">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="27e37-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="27e37-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="27e37-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="27e37-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="27e37-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="27e37-169">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="27e37-169">Not yet documented.</span></span> <span data-ttu-id="27e37-170">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="27e37-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="27e37-171">state</span><span class="sxs-lookup"><span data-stu-id="27e37-171">state</span></span>|[<span data-ttu-id="27e37-172">启用</span><span class="sxs-lookup"><span data-stu-id="27e37-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27e37-173">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="27e37-173">Not yet documented.</span></span> <span data-ttu-id="27e37-174">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27e37-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="27e37-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="27e37-175">securityDeviceRequired</span></span>|<span data-ttu-id="27e37-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="27e37-176">Boolean</span></span>|<span data-ttu-id="27e37-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-177">Not yet documented</span></span>|
|<span data-ttu-id="27e37-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="27e37-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="27e37-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="27e37-179">Boolean</span></span>|<span data-ttu-id="27e37-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-180">Not yet documented</span></span>|
|<span data-ttu-id="27e37-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="27e37-181">remotePassportEnabled</span></span>|<span data-ttu-id="27e37-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="27e37-182">Boolean</span></span>|<span data-ttu-id="27e37-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-183">Not yet documented</span></span>|
|<span data-ttu-id="27e37-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="27e37-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="27e37-185">Int32</span><span class="sxs-lookup"><span data-stu-id="27e37-185">Int32</span></span>|<span data-ttu-id="27e37-186">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-186">Not yet documented</span></span>|
|<span data-ttu-id="27e37-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="27e37-187">pinExpirationInDays</span></span>|<span data-ttu-id="27e37-188">Int32</span><span class="sxs-lookup"><span data-stu-id="27e37-188">Int32</span></span>|<span data-ttu-id="27e37-189">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27e37-189">Not yet documented</span></span>|
|<span data-ttu-id="27e37-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="27e37-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="27e37-191">启用</span><span class="sxs-lookup"><span data-stu-id="27e37-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="27e37-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="27e37-192">Not yet documented.</span></span> <span data-ttu-id="27e37-193">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="27e37-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="27e37-194">响应</span><span class="sxs-lookup"><span data-stu-id="27e37-194">Response</span></span>
<span data-ttu-id="27e37-195">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27e37-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27e37-196">示例</span><span class="sxs-lookup"><span data-stu-id="27e37-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="27e37-197">请求</span><span class="sxs-lookup"><span data-stu-id="27e37-197">Request</span></span>
<span data-ttu-id="27e37-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27e37-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="27e37-199">响应</span><span class="sxs-lookup"><span data-stu-id="27e37-199">Response</span></span>
<span data-ttu-id="27e37-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27e37-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





