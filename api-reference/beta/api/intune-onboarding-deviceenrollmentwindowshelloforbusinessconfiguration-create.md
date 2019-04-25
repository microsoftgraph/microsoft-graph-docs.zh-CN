---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6198de8729f38517ac2110e6c20e19b620b206bf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528888"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="e7711-103">创建 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7711-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="e7711-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7711-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7711-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7711-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7711-106">创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7711-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7711-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7711-107">Prerequisites</span></span>
<span data-ttu-id="e7711-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7711-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7711-110">Permission type</span></span>|<span data-ttu-id="e7711-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7711-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7711-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7711-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7711-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7711-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7711-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7711-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7711-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7711-115">Not supported.</span></span>|
|<span data-ttu-id="e7711-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7711-116">Application</span></span>|<span data-ttu-id="e7711-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7711-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7711-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7711-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7711-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7711-119">Request headers</span></span>
|<span data-ttu-id="e7711-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7711-120">Header</span></span>|<span data-ttu-id="e7711-121">值</span><span class="sxs-lookup"><span data-stu-id="e7711-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7711-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7711-122">Authorization</span></span>|<span data-ttu-id="e7711-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7711-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7711-124">接受</span><span class="sxs-lookup"><span data-stu-id="e7711-124">Accept</span></span>|<span data-ttu-id="e7711-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7711-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7711-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7711-126">Request body</span></span>
<span data-ttu-id="e7711-127">在请求正文中，提供 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7711-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="e7711-128">下表显示创建 deviceEnrollmentWindowsHelloForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7711-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="e7711-129">属性</span><span class="sxs-lookup"><span data-stu-id="e7711-129">Property</span></span>|<span data-ttu-id="e7711-130">类型</span><span class="sxs-lookup"><span data-stu-id="e7711-130">Type</span></span>|<span data-ttu-id="e7711-131">说明</span><span class="sxs-lookup"><span data-stu-id="e7711-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7711-132">id</span><span class="sxs-lookup"><span data-stu-id="e7711-132">id</span></span>|<span data-ttu-id="e7711-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e7711-133">String</span></span>|<span data-ttu-id="e7711-134">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的注册状态页面配置的 Id</span><span class="sxs-lookup"><span data-stu-id="e7711-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e7711-135">displayName</span></span>|<span data-ttu-id="e7711-136">String</span><span class="sxs-lookup"><span data-stu-id="e7711-136">String</span></span>|<span data-ttu-id="e7711-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7711-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-138">description</span><span class="sxs-lookup"><span data-stu-id="e7711-138">description</span></span>|<span data-ttu-id="e7711-139">String</span><span class="sxs-lookup"><span data-stu-id="e7711-139">String</span></span>|<span data-ttu-id="e7711-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7711-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-141">priority</span><span class="sxs-lookup"><span data-stu-id="e7711-141">priority</span></span>|<span data-ttu-id="e7711-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e7711-142">Int32</span></span>|<span data-ttu-id="e7711-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7711-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7711-144">createdDateTime</span></span>|<span data-ttu-id="e7711-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7711-145">DateTimeOffset</span></span>|<span data-ttu-id="e7711-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7711-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7711-147">lastModifiedDateTime</span></span>|<span data-ttu-id="e7711-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7711-148">DateTimeOffset</span></span>|<span data-ttu-id="e7711-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7711-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-150">version</span><span class="sxs-lookup"><span data-stu-id="e7711-150">version</span></span>|<span data-ttu-id="e7711-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e7711-151">Int32</span></span>|<span data-ttu-id="e7711-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7711-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e7711-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e7711-153">pinMinimumLength</span></span>|<span data-ttu-id="e7711-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e7711-154">Int32</span></span>|<span data-ttu-id="e7711-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-155">Not yet documented</span></span>|
|<span data-ttu-id="e7711-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="e7711-156">pinMaximumLength</span></span>|<span data-ttu-id="e7711-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e7711-157">Int32</span></span>|<span data-ttu-id="e7711-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-158">Not yet documented</span></span>|
|<span data-ttu-id="e7711-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e7711-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="e7711-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="e7711-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="e7711-161">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="e7711-161">Not yet documented.</span></span> <span data-ttu-id="e7711-162">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="e7711-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="e7711-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e7711-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="e7711-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="e7711-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="e7711-165">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="e7711-165">Not yet documented.</span></span> <span data-ttu-id="e7711-166">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="e7711-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="e7711-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e7711-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="e7711-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="e7711-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="e7711-169">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="e7711-169">Not yet documented.</span></span> <span data-ttu-id="e7711-170">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="e7711-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="e7711-171">state</span><span class="sxs-lookup"><span data-stu-id="e7711-171">state</span></span>|[<span data-ttu-id="e7711-172">启用</span><span class="sxs-lookup"><span data-stu-id="e7711-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e7711-173">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="e7711-173">Not yet documented.</span></span> <span data-ttu-id="e7711-174">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="e7711-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e7711-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="e7711-175">securityDeviceRequired</span></span>|<span data-ttu-id="e7711-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7711-176">Boolean</span></span>|<span data-ttu-id="e7711-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-177">Not yet documented</span></span>|
|<span data-ttu-id="e7711-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="e7711-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="e7711-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7711-179">Boolean</span></span>|<span data-ttu-id="e7711-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-180">Not yet documented</span></span>|
|<span data-ttu-id="e7711-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="e7711-181">remotePassportEnabled</span></span>|<span data-ttu-id="e7711-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7711-182">Boolean</span></span>|<span data-ttu-id="e7711-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-183">Not yet documented</span></span>|
|<span data-ttu-id="e7711-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="e7711-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="e7711-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e7711-185">Int32</span></span>|<span data-ttu-id="e7711-186">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-186">Not yet documented</span></span>|
|<span data-ttu-id="e7711-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="e7711-187">pinExpirationInDays</span></span>|<span data-ttu-id="e7711-188">Int32</span><span class="sxs-lookup"><span data-stu-id="e7711-188">Int32</span></span>|<span data-ttu-id="e7711-189">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7711-189">Not yet documented</span></span>|
|<span data-ttu-id="e7711-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="e7711-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="e7711-191">启用</span><span class="sxs-lookup"><span data-stu-id="e7711-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e7711-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="e7711-192">Not yet documented.</span></span> <span data-ttu-id="e7711-193">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="e7711-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="e7711-194">响应</span><span class="sxs-lookup"><span data-stu-id="e7711-194">Response</span></span>
<span data-ttu-id="e7711-195">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7711-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7711-196">示例</span><span class="sxs-lookup"><span data-stu-id="e7711-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7711-197">请求</span><span class="sxs-lookup"><span data-stu-id="e7711-197">Request</span></span>
<span data-ttu-id="e7711-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7711-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="e7711-199">响应</span><span class="sxs-lookup"><span data-stu-id="e7711-199">Response</span></span>
<span data-ttu-id="e7711-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7711-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





