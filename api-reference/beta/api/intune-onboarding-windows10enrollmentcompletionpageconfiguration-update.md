---
title: 更新 windows10EnrollmentCompletionPageConfiguration
description: 更新 windows10EnrollmentCompletionPageConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b5eec2b016fc6a61e5e241997bbb9a722ef5b27
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152584"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="2bcf9-103">更新 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="2bcf9-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="2bcf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bcf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bcf9-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bcf9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bcf9-107">更新 [windows10EnrollmentCompletionPageConfiguration 对象](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bcf9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2bcf9-108">Prerequisites</span></span>
<span data-ttu-id="2bcf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bcf9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bcf9-111">Permission type</span></span>|<span data-ttu-id="2bcf9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bcf9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bcf9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bcf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bcf9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bcf9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2bcf9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bcf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bcf9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-116">Not supported.</span></span>|
|<span data-ttu-id="2bcf9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bcf9-117">Application</span></span>|<span data-ttu-id="2bcf9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bcf9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bcf9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bcf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2bcf9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bcf9-120">Request headers</span></span>
|<span data-ttu-id="2bcf9-121">标头</span><span class="sxs-lookup"><span data-stu-id="2bcf9-121">Header</span></span>|<span data-ttu-id="2bcf9-122">值</span><span class="sxs-lookup"><span data-stu-id="2bcf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bcf9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bcf9-123">Authorization</span></span>|<span data-ttu-id="2bcf9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bcf9-125">接受</span><span class="sxs-lookup"><span data-stu-id="2bcf9-125">Accept</span></span>|<span data-ttu-id="2bcf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bcf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bcf9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bcf9-127">Request body</span></span>
<span data-ttu-id="2bcf9-128">在请求正文中，提供 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="2bcf9-129">下表显示创建 [windows10EnrollmentCompletionPageConfiguration 时所需的属性](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="2bcf9-130">属性</span><span class="sxs-lookup"><span data-stu-id="2bcf9-130">Property</span></span>|<span data-ttu-id="2bcf9-131">类型</span><span class="sxs-lookup"><span data-stu-id="2bcf9-131">Type</span></span>|<span data-ttu-id="2bcf9-132">说明</span><span class="sxs-lookup"><span data-stu-id="2bcf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bcf9-133">id</span><span class="sxs-lookup"><span data-stu-id="2bcf9-133">id</span></span>|<span data-ttu-id="2bcf9-134">String</span><span class="sxs-lookup"><span data-stu-id="2bcf9-134">String</span></span>|<span data-ttu-id="2bcf9-135">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2bcf9-136">displayName</span></span>|<span data-ttu-id="2bcf9-137">String</span><span class="sxs-lookup"><span data-stu-id="2bcf9-137">String</span></span>|<span data-ttu-id="2bcf9-138">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-139">说明</span><span class="sxs-lookup"><span data-stu-id="2bcf9-139">description</span></span>|<span data-ttu-id="2bcf9-140">String</span><span class="sxs-lookup"><span data-stu-id="2bcf9-140">String</span></span>|<span data-ttu-id="2bcf9-141">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-142">priority</span><span class="sxs-lookup"><span data-stu-id="2bcf9-142">priority</span></span>|<span data-ttu-id="2bcf9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2bcf9-143">Int32</span></span>|<span data-ttu-id="2bcf9-144">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="2bcf9-145">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="2bcf9-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bcf9-147">createdDateTime</span></span>|<span data-ttu-id="2bcf9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bcf9-148">DateTimeOffset</span></span>|<span data-ttu-id="2bcf9-149">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bcf9-150">lastModifiedDateTime</span></span>|<span data-ttu-id="2bcf9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bcf9-151">DateTimeOffset</span></span>|<span data-ttu-id="2bcf9-152">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-153">version</span><span class="sxs-lookup"><span data-stu-id="2bcf9-153">version</span></span>|<span data-ttu-id="2bcf9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2bcf9-154">Int32</span></span>|<span data-ttu-id="2bcf9-155">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2bcf9-156">roleScopeTagIds</span></span>|<span data-ttu-id="2bcf9-157">String collection</span><span class="sxs-lookup"><span data-stu-id="2bcf9-157">String collection</span></span>|<span data-ttu-id="2bcf9-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="2bcf9-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bcf9-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2bcf9-160">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="2bcf9-160">showInstallationProgress</span></span>|<span data-ttu-id="2bcf9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-161">Boolean</span></span>|<span data-ttu-id="2bcf9-162">向用户显示或隐藏安装进度</span><span class="sxs-lookup"><span data-stu-id="2bcf9-162">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="2bcf9-163">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="2bcf9-163">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="2bcf9-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-164">Boolean</span></span>|<span data-ttu-id="2bcf9-165">允许用户在安装失败时重试安装</span><span class="sxs-lookup"><span data-stu-id="2bcf9-165">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="2bcf9-166">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="2bcf9-166">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="2bcf9-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-167">Boolean</span></span>|<span data-ttu-id="2bcf9-168">安装失败时允许或阻止设备重置</span><span class="sxs-lookup"><span data-stu-id="2bcf9-168">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="2bcf9-169">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="2bcf9-169">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="2bcf9-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-170">Boolean</span></span>|<span data-ttu-id="2bcf9-171">安装失败时允许或阻止日志收集</span><span class="sxs-lookup"><span data-stu-id="2bcf9-171">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="2bcf9-172">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="2bcf9-172">customErrorMessage</span></span>|<span data-ttu-id="2bcf9-173">String</span><span class="sxs-lookup"><span data-stu-id="2bcf9-173">String</span></span>|<span data-ttu-id="2bcf9-174">将自定义错误消息设置为在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="2bcf9-174">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="2bcf9-175">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="2bcf9-175">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="2bcf9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2bcf9-176">Int32</span></span>|<span data-ttu-id="2bcf9-177">设置安装进度超时（分钟）</span><span class="sxs-lookup"><span data-stu-id="2bcf9-177">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="2bcf9-178">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="2bcf9-178">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="2bcf9-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-179">Boolean</span></span>|<span data-ttu-id="2bcf9-180">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="2bcf9-180">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="2bcf9-181">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="2bcf9-181">selectedMobileAppIds</span></span>|<span data-ttu-id="2bcf9-182">String collection</span><span class="sxs-lookup"><span data-stu-id="2bcf9-182">String collection</span></span>|<span data-ttu-id="2bcf9-183">用于跟踪安装状态的选定应用程序</span><span class="sxs-lookup"><span data-stu-id="2bcf9-183">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="2bcf9-184">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="2bcf9-184">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="2bcf9-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-185">Boolean</span></span>|<span data-ttu-id="2bcf9-186">仅显示 Autopilot 注册方案的安装进度</span><span class="sxs-lookup"><span data-stu-id="2bcf9-186">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="2bcf9-187">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="2bcf9-187">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="2bcf9-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcf9-188">Boolean</span></span>|<span data-ttu-id="2bcf9-189">仅显示第一个用户注册后的安装进度</span><span class="sxs-lookup"><span data-stu-id="2bcf9-189">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="2bcf9-190">响应</span><span class="sxs-lookup"><span data-stu-id="2bcf9-190">Response</span></span>
<span data-ttu-id="2bcf9-191">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-191">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bcf9-192">示例</span><span class="sxs-lookup"><span data-stu-id="2bcf9-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bcf9-193">请求</span><span class="sxs-lookup"><span data-stu-id="2bcf9-193">Request</span></span>
<span data-ttu-id="2bcf9-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2bcf9-195">响应</span><span class="sxs-lookup"><span data-stu-id="2bcf9-195">Response</span></span>
<span data-ttu-id="2bcf9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2bcf9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




