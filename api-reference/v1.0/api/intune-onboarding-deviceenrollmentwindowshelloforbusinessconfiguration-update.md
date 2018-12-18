---
title: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: dc443dc6804c994b8dc94ce71ca1e693e0afc43c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349075"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="6844a-103">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="6844a-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="6844a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6844a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6844a-105">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6844a-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6844a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6844a-106">Prerequisites</span></span>
<span data-ttu-id="6844a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6844a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6844a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6844a-109">Permission type</span></span>|<span data-ttu-id="6844a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6844a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6844a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6844a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6844a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6844a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6844a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6844a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6844a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6844a-114">Not supported.</span></span>|
|<span data-ttu-id="6844a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6844a-115">Application</span></span>|<span data-ttu-id="6844a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6844a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6844a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6844a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6844a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6844a-118">Request headers</span></span>
|<span data-ttu-id="6844a-119">标头</span><span class="sxs-lookup"><span data-stu-id="6844a-119">Header</span></span>|<span data-ttu-id="6844a-120">值</span><span class="sxs-lookup"><span data-stu-id="6844a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6844a-121">授权</span><span class="sxs-lookup"><span data-stu-id="6844a-121">Authorization</span></span>|<span data-ttu-id="6844a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6844a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6844a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6844a-123">Accept</span></span>|<span data-ttu-id="6844a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6844a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6844a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6844a-125">Request body</span></span>
<span data-ttu-id="6844a-126">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6844a-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="6844a-127">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6844a-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="6844a-128">属性</span><span class="sxs-lookup"><span data-stu-id="6844a-128">Property</span></span>|<span data-ttu-id="6844a-129">类型</span><span class="sxs-lookup"><span data-stu-id="6844a-129">Type</span></span>|<span data-ttu-id="6844a-130">说明</span><span class="sxs-lookup"><span data-stu-id="6844a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6844a-131">id</span><span class="sxs-lookup"><span data-stu-id="6844a-131">id</span></span>|<span data-ttu-id="6844a-132">String</span><span class="sxs-lookup"><span data-stu-id="6844a-132">String</span></span>|<span data-ttu-id="6844a-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6844a-134">displayName</span></span>|<span data-ttu-id="6844a-135">String</span><span class="sxs-lookup"><span data-stu-id="6844a-135">String</span></span>|<span data-ttu-id="6844a-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-137">description</span><span class="sxs-lookup"><span data-stu-id="6844a-137">description</span></span>|<span data-ttu-id="6844a-138">String</span><span class="sxs-lookup"><span data-stu-id="6844a-138">String</span></span>|<span data-ttu-id="6844a-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-140">priority</span><span class="sxs-lookup"><span data-stu-id="6844a-140">priority</span></span>|<span data-ttu-id="6844a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6844a-141">Int32</span></span>|<span data-ttu-id="6844a-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6844a-143">createdDateTime</span></span>|<span data-ttu-id="6844a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6844a-144">DateTimeOffset</span></span>|<span data-ttu-id="6844a-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6844a-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6844a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6844a-147">DateTimeOffset</span></span>|<span data-ttu-id="6844a-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-149">version</span><span class="sxs-lookup"><span data-stu-id="6844a-149">version</span></span>|<span data-ttu-id="6844a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6844a-150">Int32</span></span>|<span data-ttu-id="6844a-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6844a-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6844a-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6844a-152">pinMinimumLength</span></span>|<span data-ttu-id="6844a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6844a-153">Int32</span></span>|<span data-ttu-id="6844a-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-154">Not yet documented</span></span>|
|<span data-ttu-id="6844a-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="6844a-155">pinMaximumLength</span></span>|<span data-ttu-id="6844a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6844a-156">Int32</span></span>|<span data-ttu-id="6844a-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-157">Not yet documented</span></span>|
|<span data-ttu-id="6844a-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6844a-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="6844a-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6844a-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6844a-160">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="6844a-160">Not yet documented.</span></span> <span data-ttu-id="6844a-161">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6844a-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6844a-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6844a-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="6844a-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6844a-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6844a-164">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="6844a-164">Not yet documented.</span></span> <span data-ttu-id="6844a-165">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6844a-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6844a-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6844a-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="6844a-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6844a-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6844a-168">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="6844a-168">Not yet documented.</span></span> <span data-ttu-id="6844a-169">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6844a-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6844a-170">状态</span><span class="sxs-lookup"><span data-stu-id="6844a-170">state</span></span>|[<span data-ttu-id="6844a-171">启用</span><span class="sxs-lookup"><span data-stu-id="6844a-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="6844a-172">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="6844a-172">Not yet documented.</span></span> <span data-ttu-id="6844a-173">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6844a-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="6844a-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="6844a-174">securityDeviceRequired</span></span>|<span data-ttu-id="6844a-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6844a-175">Boolean</span></span>|<span data-ttu-id="6844a-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-176">Not yet documented</span></span>|
|<span data-ttu-id="6844a-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="6844a-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="6844a-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="6844a-178">Boolean</span></span>|<span data-ttu-id="6844a-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-179">Not yet documented</span></span>|
|<span data-ttu-id="6844a-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="6844a-180">remotePassportEnabled</span></span>|<span data-ttu-id="6844a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6844a-181">Boolean</span></span>|<span data-ttu-id="6844a-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-182">Not yet documented</span></span>|
|<span data-ttu-id="6844a-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="6844a-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="6844a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6844a-184">Int32</span></span>|<span data-ttu-id="6844a-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-185">Not yet documented</span></span>|
|<span data-ttu-id="6844a-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="6844a-186">pinExpirationInDays</span></span>|<span data-ttu-id="6844a-187">Int32</span><span class="sxs-lookup"><span data-stu-id="6844a-187">Int32</span></span>|<span data-ttu-id="6844a-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6844a-188">Not yet documented</span></span>|
|<span data-ttu-id="6844a-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="6844a-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="6844a-190">启用</span><span class="sxs-lookup"><span data-stu-id="6844a-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="6844a-191">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="6844a-191">Not yet documented.</span></span> <span data-ttu-id="6844a-192">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6844a-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="6844a-193">响应</span><span class="sxs-lookup"><span data-stu-id="6844a-193">Response</span></span>
<span data-ttu-id="6844a-194">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6844a-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6844a-195">示例</span><span class="sxs-lookup"><span data-stu-id="6844a-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="6844a-196">请求</span><span class="sxs-lookup"><span data-stu-id="6844a-196">Request</span></span>
<span data-ttu-id="6844a-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6844a-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6844a-198">响应</span><span class="sxs-lookup"><span data-stu-id="6844a-198">Response</span></span>
<span data-ttu-id="6844a-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6844a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



