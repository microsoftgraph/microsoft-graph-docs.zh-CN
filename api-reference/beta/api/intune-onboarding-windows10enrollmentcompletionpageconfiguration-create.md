---
title: 创建 windows10EnrollmentCompletionPageConfiguration
description: 创建新的 windows10EnrollmentCompletionPageConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3f67590255f8feb3da15a7f02949eac34659907
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211346"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="7a943-103">创建 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a943-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="7a943-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a943-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a943-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a943-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a943-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a943-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a943-107">创建新的 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a943-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a943-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7a943-108">Prerequisites</span></span>
<span data-ttu-id="7a943-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a943-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a943-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a943-111">Permission type</span></span>|<span data-ttu-id="7a943-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7a943-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a943-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a943-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a943-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a943-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7a943-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a943-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a943-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a943-116">Not supported.</span></span>|
|<span data-ttu-id="7a943-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a943-117">Application</span></span>|<span data-ttu-id="7a943-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a943-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a943-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a943-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7a943-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a943-120">Request headers</span></span>
|<span data-ttu-id="7a943-121">标头</span><span class="sxs-lookup"><span data-stu-id="7a943-121">Header</span></span>|<span data-ttu-id="7a943-122">值</span><span class="sxs-lookup"><span data-stu-id="7a943-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a943-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a943-123">Authorization</span></span>|<span data-ttu-id="7a943-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7a943-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a943-125">接受</span><span class="sxs-lookup"><span data-stu-id="7a943-125">Accept</span></span>|<span data-ttu-id="7a943-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a943-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a943-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a943-127">Request body</span></span>
<span data-ttu-id="7a943-128">在请求正文中，提供 windows10EnrollmentCompletionPageConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a943-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="7a943-129">下表显示创建 windows10EnrollmentCompletionPageConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7a943-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="7a943-130">属性</span><span class="sxs-lookup"><span data-stu-id="7a943-130">Property</span></span>|<span data-ttu-id="7a943-131">类型</span><span class="sxs-lookup"><span data-stu-id="7a943-131">Type</span></span>|<span data-ttu-id="7a943-132">说明</span><span class="sxs-lookup"><span data-stu-id="7a943-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a943-133">id</span><span class="sxs-lookup"><span data-stu-id="7a943-133">id</span></span>|<span data-ttu-id="7a943-134">String</span><span class="sxs-lookup"><span data-stu-id="7a943-134">String</span></span>|<span data-ttu-id="7a943-135">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7a943-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7a943-136">displayName</span></span>|<span data-ttu-id="7a943-137">String</span><span class="sxs-lookup"><span data-stu-id="7a943-137">String</span></span>|<span data-ttu-id="7a943-138">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="7a943-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-139">description</span><span class="sxs-lookup"><span data-stu-id="7a943-139">description</span></span>|<span data-ttu-id="7a943-140">String</span><span class="sxs-lookup"><span data-stu-id="7a943-140">String</span></span>|<span data-ttu-id="7a943-141">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="7a943-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-142">priority</span><span class="sxs-lookup"><span data-stu-id="7a943-142">priority</span></span>|<span data-ttu-id="7a943-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7a943-143">Int32</span></span>|<span data-ttu-id="7a943-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="7a943-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="7a943-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="7a943-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="7a943-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7a943-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-147">createdDateTime</span></span>|<span data-ttu-id="7a943-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a943-148">DateTimeOffset</span></span>|<span data-ttu-id="7a943-149">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-150">lastModifiedDateTime</span></span>|<span data-ttu-id="7a943-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a943-151">DateTimeOffset</span></span>|<span data-ttu-id="7a943-152">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-153">version</span><span class="sxs-lookup"><span data-stu-id="7a943-153">version</span></span>|<span data-ttu-id="7a943-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7a943-154">Int32</span></span>|<span data-ttu-id="7a943-155">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="7a943-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a943-156">roleScopeTagIds</span></span>|<span data-ttu-id="7a943-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="7a943-157">String collection</span></span>|<span data-ttu-id="7a943-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="7a943-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="7a943-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7a943-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7a943-160">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="7a943-160">showInstallationProgress</span></span>|<span data-ttu-id="7a943-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-161">Boolean</span></span>|<span data-ttu-id="7a943-162">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="7a943-162">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="7a943-163">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="7a943-163">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="7a943-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-164">Boolean</span></span>|<span data-ttu-id="7a943-165">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="7a943-165">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="7a943-166">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7a943-166">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="7a943-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-167">Boolean</span></span>|<span data-ttu-id="7a943-168">允许或阻止在安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="7a943-168">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="7a943-169">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7a943-169">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="7a943-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-170">Boolean</span></span>|<span data-ttu-id="7a943-171">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="7a943-171">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="7a943-172">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="7a943-172">customErrorMessage</span></span>|<span data-ttu-id="7a943-173">String</span><span class="sxs-lookup"><span data-stu-id="7a943-173">String</span></span>|<span data-ttu-id="7a943-174">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="7a943-174">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="7a943-175">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7a943-175">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="7a943-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7a943-176">Int32</span></span>|<span data-ttu-id="7a943-177">设置安装进度超时（分钟）</span><span class="sxs-lookup"><span data-stu-id="7a943-177">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="7a943-178">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7a943-178">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="7a943-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-179">Boolean</span></span>|<span data-ttu-id="7a943-180">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="7a943-180">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="7a943-181">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="7a943-181">selectedMobileAppIds</span></span>|<span data-ttu-id="7a943-182">String 集合</span><span class="sxs-lookup"><span data-stu-id="7a943-182">String collection</span></span>|<span data-ttu-id="7a943-183">选定的应用程序跟踪安装状态</span><span class="sxs-lookup"><span data-stu-id="7a943-183">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="7a943-184">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="7a943-184">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="7a943-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-185">Boolean</span></span>|<span data-ttu-id="7a943-186">仅显示 Autopilot 注册方案的安装进度</span><span class="sxs-lookup"><span data-stu-id="7a943-186">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="7a943-187">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="7a943-187">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="7a943-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-188">Boolean</span></span>|<span data-ttu-id="7a943-189">仅显示第一个用户后期注册的安装进度</span><span class="sxs-lookup"><span data-stu-id="7a943-189">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="7a943-190">响应</span><span class="sxs-lookup"><span data-stu-id="7a943-190">Response</span></span>
<span data-ttu-id="7a943-191">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a943-191">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a943-192">示例</span><span class="sxs-lookup"><span data-stu-id="7a943-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a943-193">请求</span><span class="sxs-lookup"><span data-stu-id="7a943-193">Request</span></span>
<span data-ttu-id="7a943-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a943-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="7a943-195">响应</span><span class="sxs-lookup"><span data-stu-id="7a943-195">Response</span></span>
<span data-ttu-id="7a943-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a943-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 918

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




