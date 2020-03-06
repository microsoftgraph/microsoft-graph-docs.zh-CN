---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfdc22edcd04638c5b5f7a332ede550feae98352
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512613"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="ef1d0-103">创建 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef1d0-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="ef1d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef1d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef1d0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef1d0-106">创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef1d0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef1d0-107">Prerequisites</span></span>
<span data-ttu-id="ef1d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef1d0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef1d0-110">Permission type</span></span>|<span data-ttu-id="ef1d0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef1d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef1d0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef1d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef1d0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1d0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ef1d0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef1d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef1d0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-115">Not supported.</span></span>|
|<span data-ttu-id="ef1d0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef1d0-116">Application</span></span>|<span data-ttu-id="ef1d0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef1d0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef1d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef1d0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef1d0-119">Request headers</span></span>
|<span data-ttu-id="ef1d0-120">标头</span><span class="sxs-lookup"><span data-stu-id="ef1d0-120">Header</span></span>|<span data-ttu-id="ef1d0-121">值</span><span class="sxs-lookup"><span data-stu-id="ef1d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef1d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef1d0-122">Authorization</span></span>|<span data-ttu-id="ef1d0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef1d0-124">接受</span><span class="sxs-lookup"><span data-stu-id="ef1d0-124">Accept</span></span>|<span data-ttu-id="ef1d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef1d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef1d0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef1d0-126">Request body</span></span>
<span data-ttu-id="ef1d0-127">在请求正文中，提供 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="ef1d0-128">下表显示创建 deviceEnrollmentWindowsHelloForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="ef1d0-129">属性</span><span class="sxs-lookup"><span data-stu-id="ef1d0-129">Property</span></span>|<span data-ttu-id="ef1d0-130">类型</span><span class="sxs-lookup"><span data-stu-id="ef1d0-130">Type</span></span>|<span data-ttu-id="ef1d0-131">说明</span><span class="sxs-lookup"><span data-stu-id="ef1d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef1d0-132">id</span><span class="sxs-lookup"><span data-stu-id="ef1d0-132">id</span></span>|<span data-ttu-id="ef1d0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ef1d0-133">String</span></span>|<span data-ttu-id="ef1d0-134">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ef1d0-135">displayName</span></span>|<span data-ttu-id="ef1d0-136">String</span><span class="sxs-lookup"><span data-stu-id="ef1d0-136">String</span></span>|<span data-ttu-id="ef1d0-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-138">说明</span><span class="sxs-lookup"><span data-stu-id="ef1d0-138">description</span></span>|<span data-ttu-id="ef1d0-139">String</span><span class="sxs-lookup"><span data-stu-id="ef1d0-139">String</span></span>|<span data-ttu-id="ef1d0-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-141">priority</span><span class="sxs-lookup"><span data-stu-id="ef1d0-141">priority</span></span>|<span data-ttu-id="ef1d0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1d0-142">Int32</span></span>|<span data-ttu-id="ef1d0-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1d0-144">createdDateTime</span></span>|<span data-ttu-id="ef1d0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1d0-145">DateTimeOffset</span></span>|<span data-ttu-id="ef1d0-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1d0-147">lastModifiedDateTime</span></span>|<span data-ttu-id="ef1d0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1d0-148">DateTimeOffset</span></span>|<span data-ttu-id="ef1d0-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-150">version</span><span class="sxs-lookup"><span data-stu-id="ef1d0-150">version</span></span>|<span data-ttu-id="ef1d0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1d0-151">Int32</span></span>|<span data-ttu-id="ef1d0-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1d0-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef1d0-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ef1d0-153">pinMinimumLength</span></span>|<span data-ttu-id="ef1d0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1d0-154">Int32</span></span>|<span data-ttu-id="ef1d0-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-155">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="ef1d0-156">pinMaximumLength</span></span>|<span data-ttu-id="ef1d0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1d0-157">Int32</span></span>|<span data-ttu-id="ef1d0-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-158">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ef1d0-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="ef1d0-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="ef1d0-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="ef1d0-161">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-161">Not yet documented.</span></span> <span data-ttu-id="ef1d0-162">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ef1d0-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ef1d0-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="ef1d0-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="ef1d0-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="ef1d0-165">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-165">Not yet documented.</span></span> <span data-ttu-id="ef1d0-166">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ef1d0-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ef1d0-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="ef1d0-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="ef1d0-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="ef1d0-169">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-169">Not yet documented.</span></span> <span data-ttu-id="ef1d0-170">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ef1d0-171">state</span><span class="sxs-lookup"><span data-stu-id="ef1d0-171">state</span></span>|[<span data-ttu-id="ef1d0-172">启用</span><span class="sxs-lookup"><span data-stu-id="ef1d0-172">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="ef1d0-173">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-173">Not yet documented.</span></span> <span data-ttu-id="ef1d0-174">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ef1d0-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="ef1d0-175">securityDeviceRequired</span></span>|<span data-ttu-id="ef1d0-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef1d0-176">Boolean</span></span>|<span data-ttu-id="ef1d0-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-177">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="ef1d0-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="ef1d0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef1d0-179">Boolean</span></span>|<span data-ttu-id="ef1d0-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-180">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="ef1d0-181">remotePassportEnabled</span></span>|<span data-ttu-id="ef1d0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef1d0-182">Boolean</span></span>|<span data-ttu-id="ef1d0-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-183">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="ef1d0-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="ef1d0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1d0-185">Int32</span></span>|<span data-ttu-id="ef1d0-186">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-186">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="ef1d0-187">pinExpirationInDays</span></span>|<span data-ttu-id="ef1d0-188">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1d0-188">Int32</span></span>|<span data-ttu-id="ef1d0-189">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ef1d0-189">Not yet documented</span></span>|
|<span data-ttu-id="ef1d0-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="ef1d0-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="ef1d0-191">启用</span><span class="sxs-lookup"><span data-stu-id="ef1d0-191">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="ef1d0-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-192">Not yet documented.</span></span> <span data-ttu-id="ef1d0-193">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef1d0-194">响应</span><span class="sxs-lookup"><span data-stu-id="ef1d0-194">Response</span></span>
<span data-ttu-id="ef1d0-195">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef1d0-196">示例</span><span class="sxs-lookup"><span data-stu-id="ef1d0-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef1d0-197">请求</span><span class="sxs-lookup"><span data-stu-id="ef1d0-197">Request</span></span>
<span data-ttu-id="ef1d0-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef1d0-199">响应</span><span class="sxs-lookup"><span data-stu-id="ef1d0-199">Response</span></span>
<span data-ttu-id="ef1d0-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef1d0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




