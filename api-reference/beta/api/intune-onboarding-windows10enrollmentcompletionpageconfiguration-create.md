---
title: 创建 windows10EnrollmentCompletionPageConfiguration
description: 创建新的 windows10EnrollmentCompletionPageConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d46ffcef2336a1a43e72ef07587c02a84b588bd5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537648"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="f64d8-103">创建 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="f64d8-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="f64d8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f64d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f64d8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f64d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f64d8-106">创建新的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f64d8-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f64d8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f64d8-107">Prerequisites</span></span>
<span data-ttu-id="f64d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f64d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64d8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f64d8-110">Permission type</span></span>|<span data-ttu-id="f64d8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f64d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f64d8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f64d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f64d8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64d8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f64d8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f64d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f64d8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f64d8-115">Not supported.</span></span>|
|<span data-ttu-id="f64d8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f64d8-116">Application</span></span>|<span data-ttu-id="f64d8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64d8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f64d8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f64d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f64d8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f64d8-119">Request headers</span></span>
|<span data-ttu-id="f64d8-120">标头</span><span class="sxs-lookup"><span data-stu-id="f64d8-120">Header</span></span>|<span data-ttu-id="f64d8-121">值</span><span class="sxs-lookup"><span data-stu-id="f64d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f64d8-122">授权</span><span class="sxs-lookup"><span data-stu-id="f64d8-122">Authorization</span></span>|<span data-ttu-id="f64d8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f64d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f64d8-124">接受</span><span class="sxs-lookup"><span data-stu-id="f64d8-124">Accept</span></span>|<span data-ttu-id="f64d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f64d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f64d8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f64d8-126">Request body</span></span>
<span data-ttu-id="f64d8-127">在请求正文中，提供 windows10EnrollmentCompletionPageConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f64d8-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="f64d8-128">下表显示创建 windows10EnrollmentCompletionPageConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f64d8-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="f64d8-129">属性</span><span class="sxs-lookup"><span data-stu-id="f64d8-129">Property</span></span>|<span data-ttu-id="f64d8-130">类型</span><span class="sxs-lookup"><span data-stu-id="f64d8-130">Type</span></span>|<span data-ttu-id="f64d8-131">说明</span><span class="sxs-lookup"><span data-stu-id="f64d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f64d8-132">id</span><span class="sxs-lookup"><span data-stu-id="f64d8-132">id</span></span>|<span data-ttu-id="f64d8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f64d8-133">String</span></span>|<span data-ttu-id="f64d8-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f64d8-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f64d8-135">displayName</span></span>|<span data-ttu-id="f64d8-136">String</span><span class="sxs-lookup"><span data-stu-id="f64d8-136">String</span></span>|<span data-ttu-id="f64d8-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="f64d8-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-138">说明</span><span class="sxs-lookup"><span data-stu-id="f64d8-138">description</span></span>|<span data-ttu-id="f64d8-139">String</span><span class="sxs-lookup"><span data-stu-id="f64d8-139">String</span></span>|<span data-ttu-id="f64d8-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="f64d8-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-141">priority</span><span class="sxs-lookup"><span data-stu-id="f64d8-141">priority</span></span>|<span data-ttu-id="f64d8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f64d8-142">Int32</span></span>|<span data-ttu-id="f64d8-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="f64d8-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="f64d8-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="f64d8-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="f64d8-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f64d8-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f64d8-146">createdDateTime</span></span>|<span data-ttu-id="f64d8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f64d8-147">DateTimeOffset</span></span>|<span data-ttu-id="f64d8-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="f64d8-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f64d8-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f64d8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f64d8-150">DateTimeOffset</span></span>|<span data-ttu-id="f64d8-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="f64d8-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-152">version</span><span class="sxs-lookup"><span data-stu-id="f64d8-152">version</span></span>|<span data-ttu-id="f64d8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f64d8-153">Int32</span></span>|<span data-ttu-id="f64d8-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="f64d8-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f64d8-155">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="f64d8-155">showInstallationProgress</span></span>|<span data-ttu-id="f64d8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-156">Boolean</span></span>|<span data-ttu-id="f64d8-157">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="f64d8-157">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="f64d8-158">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="f64d8-158">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="f64d8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-159">Boolean</span></span>|<span data-ttu-id="f64d8-160">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="f64d8-160">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="f64d8-161">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f64d8-161">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="f64d8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-162">Boolean</span></span>|<span data-ttu-id="f64d8-163">允许或阻止在安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="f64d8-163">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="f64d8-164">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f64d8-164">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="f64d8-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-165">Boolean</span></span>|<span data-ttu-id="f64d8-166">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="f64d8-166">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="f64d8-167">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="f64d8-167">customErrorMessage</span></span>|<span data-ttu-id="f64d8-168">字符串</span><span class="sxs-lookup"><span data-stu-id="f64d8-168">String</span></span>|<span data-ttu-id="f64d8-169">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="f64d8-169">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="f64d8-170">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="f64d8-170">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="f64d8-171">Int32</span><span class="sxs-lookup"><span data-stu-id="f64d8-171">Int32</span></span>|<span data-ttu-id="f64d8-172">设置安装进度超时（分钟）</span><span class="sxs-lookup"><span data-stu-id="f64d8-172">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="f64d8-173">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f64d8-173">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="f64d8-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-174">Boolean</span></span>|<span data-ttu-id="f64d8-175">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="f64d8-175">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="f64d8-176">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="f64d8-176">selectedMobileAppIds</span></span>|<span data-ttu-id="f64d8-177">String 集合</span><span class="sxs-lookup"><span data-stu-id="f64d8-177">String collection</span></span>|<span data-ttu-id="f64d8-178">选定的应用程序跟踪安装状态</span><span class="sxs-lookup"><span data-stu-id="f64d8-178">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="f64d8-179">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="f64d8-179">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="f64d8-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-180">Boolean</span></span>|<span data-ttu-id="f64d8-181">仅显示 Autopilot 注册方案的安装进度</span><span class="sxs-lookup"><span data-stu-id="f64d8-181">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="f64d8-182">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="f64d8-182">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="f64d8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="f64d8-183">Boolean</span></span>|<span data-ttu-id="f64d8-184">仅显示第一个用户后期注册的安装进度</span><span class="sxs-lookup"><span data-stu-id="f64d8-184">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="f64d8-185">响应</span><span class="sxs-lookup"><span data-stu-id="f64d8-185">Response</span></span>
<span data-ttu-id="f64d8-186">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f64d8-186">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f64d8-187">示例</span><span class="sxs-lookup"><span data-stu-id="f64d8-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="f64d8-188">请求</span><span class="sxs-lookup"><span data-stu-id="f64d8-188">Request</span></span>
<span data-ttu-id="f64d8-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f64d8-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 684

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```

### <a name="response"></a><span data-ttu-id="f64d8-190">响应</span><span class="sxs-lookup"><span data-stu-id="f64d8-190">Response</span></span>
<span data-ttu-id="f64d8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f64d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 856

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```






