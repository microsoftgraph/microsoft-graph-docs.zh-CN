---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbd45a72db4b226ec23cdd8221cbb16cb27ba771
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362552"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="6d010-103">创建 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d010-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="6d010-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d010-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d010-105">创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d010-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d010-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d010-106">Prerequisites</span></span>
<span data-ttu-id="6d010-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d010-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d010-109">Permission type</span></span>|<span data-ttu-id="6d010-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6d010-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d010-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d010-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d010-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d010-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6d010-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d010-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d010-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d010-114">Not supported.</span></span>|
|<span data-ttu-id="6d010-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d010-115">Application</span></span>|<span data-ttu-id="6d010-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d010-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d010-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d010-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6d010-118">请求头</span><span class="sxs-lookup"><span data-stu-id="6d010-118">Request headers</span></span>
|<span data-ttu-id="6d010-119">标头</span><span class="sxs-lookup"><span data-stu-id="6d010-119">Header</span></span>|<span data-ttu-id="6d010-120">值</span><span class="sxs-lookup"><span data-stu-id="6d010-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d010-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d010-121">Authorization</span></span>|<span data-ttu-id="6d010-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d010-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d010-123">接受</span><span class="sxs-lookup"><span data-stu-id="6d010-123">Accept</span></span>|<span data-ttu-id="6d010-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d010-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d010-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d010-125">Request body</span></span>
<span data-ttu-id="6d010-126">在请求正文中，提供 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d010-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="6d010-127">下表显示创建 deviceEnrollmentWindowsHelloForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6d010-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="6d010-128">属性</span><span class="sxs-lookup"><span data-stu-id="6d010-128">Property</span></span>|<span data-ttu-id="6d010-129">类型</span><span class="sxs-lookup"><span data-stu-id="6d010-129">Type</span></span>|<span data-ttu-id="6d010-130">说明</span><span class="sxs-lookup"><span data-stu-id="6d010-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d010-131">id</span><span class="sxs-lookup"><span data-stu-id="6d010-131">id</span></span>|<span data-ttu-id="6d010-132">字符串</span><span class="sxs-lookup"><span data-stu-id="6d010-132">String</span></span>|<span data-ttu-id="6d010-133">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6d010-134">displayName</span></span>|<span data-ttu-id="6d010-135">String</span><span class="sxs-lookup"><span data-stu-id="6d010-135">String</span></span>|<span data-ttu-id="6d010-136">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-137">说明</span><span class="sxs-lookup"><span data-stu-id="6d010-137">description</span></span>|<span data-ttu-id="6d010-138">String</span><span class="sxs-lookup"><span data-stu-id="6d010-138">String</span></span>|<span data-ttu-id="6d010-139">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-140">priority</span><span class="sxs-lookup"><span data-stu-id="6d010-140">priority</span></span>|<span data-ttu-id="6d010-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6d010-141">Int32</span></span>|<span data-ttu-id="6d010-142">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d010-143">createdDateTime</span></span>|<span data-ttu-id="6d010-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d010-144">DateTimeOffset</span></span>|<span data-ttu-id="6d010-145">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d010-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6d010-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d010-147">DateTimeOffset</span></span>|<span data-ttu-id="6d010-148">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-149">version</span><span class="sxs-lookup"><span data-stu-id="6d010-149">version</span></span>|<span data-ttu-id="6d010-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6d010-150">Int32</span></span>|<span data-ttu-id="6d010-151">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d010-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d010-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6d010-152">pinMinimumLength</span></span>|<span data-ttu-id="6d010-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6d010-153">Int32</span></span>|<span data-ttu-id="6d010-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-154">Not yet documented</span></span>|
|<span data-ttu-id="6d010-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="6d010-155">pinMaximumLength</span></span>|<span data-ttu-id="6d010-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6d010-156">Int32</span></span>|<span data-ttu-id="6d010-157">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-157">Not yet documented</span></span>|
|<span data-ttu-id="6d010-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6d010-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="6d010-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6d010-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6d010-160">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6d010-160">Not yet documented.</span></span> <span data-ttu-id="6d010-161">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6d010-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6d010-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6d010-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="6d010-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6d010-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6d010-164">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6d010-164">Not yet documented.</span></span> <span data-ttu-id="6d010-165">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6d010-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6d010-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6d010-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="6d010-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6d010-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6d010-168">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6d010-168">Not yet documented.</span></span> <span data-ttu-id="6d010-169">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="6d010-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6d010-170">state</span><span class="sxs-lookup"><span data-stu-id="6d010-170">state</span></span>|[<span data-ttu-id="6d010-171">启用</span><span class="sxs-lookup"><span data-stu-id="6d010-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="6d010-172">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6d010-172">Not yet documented.</span></span> <span data-ttu-id="6d010-173">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6d010-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="6d010-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="6d010-174">securityDeviceRequired</span></span>|<span data-ttu-id="6d010-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d010-175">Boolean</span></span>|<span data-ttu-id="6d010-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-176">Not yet documented</span></span>|
|<span data-ttu-id="6d010-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="6d010-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="6d010-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d010-178">Boolean</span></span>|<span data-ttu-id="6d010-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-179">Not yet documented</span></span>|
|<span data-ttu-id="6d010-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="6d010-180">remotePassportEnabled</span></span>|<span data-ttu-id="6d010-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d010-181">Boolean</span></span>|<span data-ttu-id="6d010-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-182">Not yet documented</span></span>|
|<span data-ttu-id="6d010-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="6d010-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="6d010-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6d010-184">Int32</span></span>|<span data-ttu-id="6d010-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-185">Not yet documented</span></span>|
|<span data-ttu-id="6d010-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="6d010-186">pinExpirationInDays</span></span>|<span data-ttu-id="6d010-187">Int32</span><span class="sxs-lookup"><span data-stu-id="6d010-187">Int32</span></span>|<span data-ttu-id="6d010-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d010-188">Not yet documented</span></span>|
|<span data-ttu-id="6d010-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="6d010-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="6d010-190">启用</span><span class="sxs-lookup"><span data-stu-id="6d010-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="6d010-191">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6d010-191">Not yet documented.</span></span> <span data-ttu-id="6d010-192">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6d010-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="6d010-193">响应</span><span class="sxs-lookup"><span data-stu-id="6d010-193">Response</span></span>
<span data-ttu-id="6d010-194">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d010-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d010-195">示例</span><span class="sxs-lookup"><span data-stu-id="6d010-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d010-196">请求</span><span class="sxs-lookup"><span data-stu-id="6d010-196">Request</span></span>
<span data-ttu-id="6d010-197">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d010-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="6d010-198">响应</span><span class="sxs-lookup"><span data-stu-id="6d010-198">Response</span></span>
<span data-ttu-id="6d010-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d010-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




