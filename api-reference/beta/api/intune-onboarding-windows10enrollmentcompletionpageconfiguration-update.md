---
title: 更新 windows10EnrollmentCompletionPageConfiguration
description: 更新 windows10EnrollmentCompletionPageConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e6accf7b452a94a54a1006e3b11b9d9c6cbdec6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899723"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="dfdac-103">更新 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfdac-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="dfdac-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfdac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfdac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfdac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfdac-106">更新[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dfdac-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfdac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfdac-107">Prerequisites</span></span>
<span data-ttu-id="dfdac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfdac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfdac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfdac-110">Permission type</span></span>|<span data-ttu-id="dfdac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfdac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfdac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfdac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfdac-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfdac-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dfdac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfdac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfdac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfdac-115">Not supported.</span></span>|
|<span data-ttu-id="dfdac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfdac-116">Application</span></span>|<span data-ttu-id="dfdac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfdac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfdac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfdac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dfdac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfdac-119">Request headers</span></span>
|<span data-ttu-id="dfdac-120">标头</span><span class="sxs-lookup"><span data-stu-id="dfdac-120">Header</span></span>|<span data-ttu-id="dfdac-121">值</span><span class="sxs-lookup"><span data-stu-id="dfdac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfdac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfdac-122">Authorization</span></span>|<span data-ttu-id="dfdac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfdac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfdac-124">接受</span><span class="sxs-lookup"><span data-stu-id="dfdac-124">Accept</span></span>|<span data-ttu-id="dfdac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfdac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfdac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfdac-126">Request body</span></span>
<span data-ttu-id="dfdac-127">在请求正文中, 提供[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfdac-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="dfdac-128">下表显示创建[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dfdac-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="dfdac-129">属性</span><span class="sxs-lookup"><span data-stu-id="dfdac-129">Property</span></span>|<span data-ttu-id="dfdac-130">类型</span><span class="sxs-lookup"><span data-stu-id="dfdac-130">Type</span></span>|<span data-ttu-id="dfdac-131">说明</span><span class="sxs-lookup"><span data-stu-id="dfdac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfdac-132">id</span><span class="sxs-lookup"><span data-stu-id="dfdac-132">id</span></span>|<span data-ttu-id="dfdac-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dfdac-133">String</span></span>|<span data-ttu-id="dfdac-134">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="dfdac-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dfdac-135">displayName</span></span>|<span data-ttu-id="dfdac-136">String</span><span class="sxs-lookup"><span data-stu-id="dfdac-136">String</span></span>|<span data-ttu-id="dfdac-137">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="dfdac-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-138">说明</span><span class="sxs-lookup"><span data-stu-id="dfdac-138">description</span></span>|<span data-ttu-id="dfdac-139">String</span><span class="sxs-lookup"><span data-stu-id="dfdac-139">String</span></span>|<span data-ttu-id="dfdac-140">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="dfdac-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-141">priority</span><span class="sxs-lookup"><span data-stu-id="dfdac-141">priority</span></span>|<span data-ttu-id="dfdac-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dfdac-142">Int32</span></span>|<span data-ttu-id="dfdac-143">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="dfdac-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="dfdac-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="dfdac-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="dfdac-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfdac-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfdac-146">createdDateTime</span></span>|<span data-ttu-id="dfdac-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfdac-147">DateTimeOffset</span></span>|<span data-ttu-id="dfdac-148">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="dfdac-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfdac-149">lastModifiedDateTime</span></span>|<span data-ttu-id="dfdac-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfdac-150">DateTimeOffset</span></span>|<span data-ttu-id="dfdac-151">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="dfdac-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-152">version</span><span class="sxs-lookup"><span data-stu-id="dfdac-152">version</span></span>|<span data-ttu-id="dfdac-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dfdac-153">Int32</span></span>|<span data-ttu-id="dfdac-154">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="dfdac-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfdac-155">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="dfdac-155">showInstallationProgress</span></span>|<span data-ttu-id="dfdac-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfdac-156">Boolean</span></span>|<span data-ttu-id="dfdac-157">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="dfdac-157">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="dfdac-158">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="dfdac-158">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="dfdac-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfdac-159">Boolean</span></span>|<span data-ttu-id="dfdac-160">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="dfdac-160">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="dfdac-161">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="dfdac-161">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="dfdac-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfdac-162">Boolean</span></span>|<span data-ttu-id="dfdac-163">允许或阻止在安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="dfdac-163">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="dfdac-164">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="dfdac-164">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="dfdac-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfdac-165">Boolean</span></span>|<span data-ttu-id="dfdac-166">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="dfdac-166">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="dfdac-167">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="dfdac-167">customErrorMessage</span></span>|<span data-ttu-id="dfdac-168">String</span><span class="sxs-lookup"><span data-stu-id="dfdac-168">String</span></span>|<span data-ttu-id="dfdac-169">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="dfdac-169">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="dfdac-170">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="dfdac-170">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="dfdac-171">Int32</span><span class="sxs-lookup"><span data-stu-id="dfdac-171">Int32</span></span>|<span data-ttu-id="dfdac-172">设置安装进度超时 (分钟)</span><span class="sxs-lookup"><span data-stu-id="dfdac-172">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="dfdac-173">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="dfdac-173">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="dfdac-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfdac-174">Boolean</span></span>|<span data-ttu-id="dfdac-175">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="dfdac-175">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="dfdac-176">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="dfdac-176">selectedMobileAppIds</span></span>|<span data-ttu-id="dfdac-177">String collection</span><span class="sxs-lookup"><span data-stu-id="dfdac-177">String collection</span></span>|<span data-ttu-id="dfdac-178">选定的应用程序跟踪安装状态</span><span class="sxs-lookup"><span data-stu-id="dfdac-178">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="dfdac-179">响应</span><span class="sxs-lookup"><span data-stu-id="dfdac-179">Response</span></span>
<span data-ttu-id="dfdac-180">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfdac-180">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfdac-181">示例</span><span class="sxs-lookup"><span data-stu-id="dfdac-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfdac-182">请求</span><span class="sxs-lookup"><span data-stu-id="dfdac-182">Request</span></span>
<span data-ttu-id="dfdac-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfdac-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 583

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="dfdac-184">响应</span><span class="sxs-lookup"><span data-stu-id="dfdac-184">Response</span></span>
<span data-ttu-id="dfdac-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfdac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 755

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
  ]
}
```




