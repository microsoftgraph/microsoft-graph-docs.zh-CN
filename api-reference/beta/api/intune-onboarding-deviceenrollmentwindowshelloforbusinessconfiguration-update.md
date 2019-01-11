---
title: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3a087b38a4bd1a156645b45936fa6e5c966adea5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862774"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="94a22-103">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="94a22-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="94a22-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94a22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94a22-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94a22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94a22-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="94a22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94a22-107">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94a22-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94a22-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="94a22-108">Prerequisites</span></span>
<span data-ttu-id="94a22-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="94a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a22-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94a22-111">Permission type</span></span>|<span data-ttu-id="94a22-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="94a22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94a22-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94a22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94a22-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a22-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94a22-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94a22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94a22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94a22-116">Not supported.</span></span>|
|<span data-ttu-id="94a22-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94a22-117">Application</span></span>|<span data-ttu-id="94a22-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="94a22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94a22-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94a22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="94a22-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94a22-120">Request headers</span></span>
|<span data-ttu-id="94a22-121">标头</span><span class="sxs-lookup"><span data-stu-id="94a22-121">Header</span></span>|<span data-ttu-id="94a22-122">值</span><span class="sxs-lookup"><span data-stu-id="94a22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94a22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94a22-123">Authorization</span></span>|<span data-ttu-id="94a22-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94a22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94a22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94a22-125">Accept</span></span>|<span data-ttu-id="94a22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94a22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94a22-127">Request body</span></span>
<span data-ttu-id="94a22-128">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a22-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="94a22-129">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="94a22-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="94a22-130">属性</span><span class="sxs-lookup"><span data-stu-id="94a22-130">Property</span></span>|<span data-ttu-id="94a22-131">类型</span><span class="sxs-lookup"><span data-stu-id="94a22-131">Type</span></span>|<span data-ttu-id="94a22-132">说明</span><span class="sxs-lookup"><span data-stu-id="94a22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a22-133">id</span><span class="sxs-lookup"><span data-stu-id="94a22-133">id</span></span>|<span data-ttu-id="94a22-134">String</span><span class="sxs-lookup"><span data-stu-id="94a22-134">String</span></span>|<span data-ttu-id="94a22-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-136">displayName</span><span class="sxs-lookup"><span data-stu-id="94a22-136">displayName</span></span>|<span data-ttu-id="94a22-137">String</span><span class="sxs-lookup"><span data-stu-id="94a22-137">String</span></span>|<span data-ttu-id="94a22-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-139">description</span><span class="sxs-lookup"><span data-stu-id="94a22-139">description</span></span>|<span data-ttu-id="94a22-140">String</span><span class="sxs-lookup"><span data-stu-id="94a22-140">String</span></span>|<span data-ttu-id="94a22-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-142">priority</span><span class="sxs-lookup"><span data-stu-id="94a22-142">priority</span></span>|<span data-ttu-id="94a22-143">Int32</span><span class="sxs-lookup"><span data-stu-id="94a22-143">Int32</span></span>|<span data-ttu-id="94a22-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94a22-145">createdDateTime</span></span>|<span data-ttu-id="94a22-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a22-146">DateTimeOffset</span></span>|<span data-ttu-id="94a22-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94a22-148">lastModifiedDateTime</span></span>|<span data-ttu-id="94a22-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a22-149">DateTimeOffset</span></span>|<span data-ttu-id="94a22-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-151">version</span><span class="sxs-lookup"><span data-stu-id="94a22-151">version</span></span>|<span data-ttu-id="94a22-152">Int32</span><span class="sxs-lookup"><span data-stu-id="94a22-152">Int32</span></span>|<span data-ttu-id="94a22-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94a22-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="94a22-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="94a22-154">pinMinimumLength</span></span>|<span data-ttu-id="94a22-155">Int32</span><span class="sxs-lookup"><span data-stu-id="94a22-155">Int32</span></span>|<span data-ttu-id="94a22-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-156">Not yet documented</span></span>|
|<span data-ttu-id="94a22-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="94a22-157">pinMaximumLength</span></span>|<span data-ttu-id="94a22-158">Int32</span><span class="sxs-lookup"><span data-stu-id="94a22-158">Int32</span></span>|<span data-ttu-id="94a22-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-159">Not yet documented</span></span>|
|<span data-ttu-id="94a22-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="94a22-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="94a22-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="94a22-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="94a22-162">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="94a22-162">Not yet documented.</span></span> <span data-ttu-id="94a22-163">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="94a22-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="94a22-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="94a22-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="94a22-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="94a22-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="94a22-166">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="94a22-166">Not yet documented.</span></span> <span data-ttu-id="94a22-167">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="94a22-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="94a22-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="94a22-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="94a22-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="94a22-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="94a22-170">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="94a22-170">Not yet documented.</span></span> <span data-ttu-id="94a22-171">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="94a22-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="94a22-172">state</span><span class="sxs-lookup"><span data-stu-id="94a22-172">state</span></span>|[<span data-ttu-id="94a22-173">启用</span><span class="sxs-lookup"><span data-stu-id="94a22-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a22-174">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="94a22-174">Not yet documented.</span></span> <span data-ttu-id="94a22-175">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="94a22-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="94a22-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="94a22-176">securityDeviceRequired</span></span>|<span data-ttu-id="94a22-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a22-177">Boolean</span></span>|<span data-ttu-id="94a22-178">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-178">Not yet documented</span></span>|
|<span data-ttu-id="94a22-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="94a22-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="94a22-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a22-180">Boolean</span></span>|<span data-ttu-id="94a22-181">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-181">Not yet documented</span></span>|
|<span data-ttu-id="94a22-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="94a22-182">remotePassportEnabled</span></span>|<span data-ttu-id="94a22-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a22-183">Boolean</span></span>|<span data-ttu-id="94a22-184">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-184">Not yet documented</span></span>|
|<span data-ttu-id="94a22-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="94a22-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="94a22-186">Int32</span><span class="sxs-lookup"><span data-stu-id="94a22-186">Int32</span></span>|<span data-ttu-id="94a22-187">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-187">Not yet documented</span></span>|
|<span data-ttu-id="94a22-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="94a22-188">pinExpirationInDays</span></span>|<span data-ttu-id="94a22-189">Int32</span><span class="sxs-lookup"><span data-stu-id="94a22-189">Int32</span></span>|<span data-ttu-id="94a22-190">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94a22-190">Not yet documented</span></span>|
|<span data-ttu-id="94a22-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="94a22-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="94a22-192">启用</span><span class="sxs-lookup"><span data-stu-id="94a22-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="94a22-193">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="94a22-193">Not yet documented.</span></span> <span data-ttu-id="94a22-194">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="94a22-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="94a22-195">响应</span><span class="sxs-lookup"><span data-stu-id="94a22-195">Response</span></span>
<span data-ttu-id="94a22-196">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94a22-196">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a22-197">示例</span><span class="sxs-lookup"><span data-stu-id="94a22-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="94a22-198">请求</span><span class="sxs-lookup"><span data-stu-id="94a22-198">Request</span></span>
<span data-ttu-id="94a22-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94a22-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="94a22-200">响应</span><span class="sxs-lookup"><span data-stu-id="94a22-200">Response</span></span>
<span data-ttu-id="94a22-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94a22-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





