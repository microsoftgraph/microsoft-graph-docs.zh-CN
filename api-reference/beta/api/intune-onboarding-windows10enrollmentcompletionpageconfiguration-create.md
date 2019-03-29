---
title: 创建 windows10EnrollmentCompletionPageConfiguration
description: 创建新的 windows10EnrollmentCompletionPageConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9751c71cee378eabe3bbbf065e2e5ba3e0cdd337
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957029"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="2f1c2-103">创建 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f1c2-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="2f1c2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f1c2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f1c2-106">创建新的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f1c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f1c2-107">Prerequisites</span></span>
<span data-ttu-id="2f1c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f1c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f1c2-110">Permission type</span></span>|<span data-ttu-id="2f1c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f1c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f1c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f1c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f1c2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f1c2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f1c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f1c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f1c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-115">Not supported.</span></span>|
|<span data-ttu-id="2f1c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f1c2-116">Application</span></span>|<span data-ttu-id="2f1c2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f1c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f1c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f1c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f1c2-119">Request headers</span></span>
|<span data-ttu-id="2f1c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="2f1c2-120">Header</span></span>|<span data-ttu-id="2f1c2-121">值</span><span class="sxs-lookup"><span data-stu-id="2f1c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f1c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f1c2-122">Authorization</span></span>|<span data-ttu-id="2f1c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f1c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="2f1c2-124">Accept</span></span>|<span data-ttu-id="2f1c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f1c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f1c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f1c2-126">Request body</span></span>
<span data-ttu-id="2f1c2-127">在请求正文中, 提供 windows10EnrollmentCompletionPageConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="2f1c2-128">下表显示创建 windows10EnrollmentCompletionPageConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="2f1c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="2f1c2-129">Property</span></span>|<span data-ttu-id="2f1c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="2f1c2-130">Type</span></span>|<span data-ttu-id="2f1c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="2f1c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f1c2-132">id</span><span class="sxs-lookup"><span data-stu-id="2f1c2-132">id</span></span>|<span data-ttu-id="2f1c2-133">String</span><span class="sxs-lookup"><span data-stu-id="2f1c2-133">String</span></span>|<span data-ttu-id="2f1c2-134">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的注册状态页面配置的 Id</span><span class="sxs-lookup"><span data-stu-id="2f1c2-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2f1c2-135">displayName</span></span>|<span data-ttu-id="2f1c2-136">String</span><span class="sxs-lookup"><span data-stu-id="2f1c2-136">String</span></span>|<span data-ttu-id="2f1c2-137">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-138">description</span><span class="sxs-lookup"><span data-stu-id="2f1c2-138">description</span></span>|<span data-ttu-id="2f1c2-139">String</span><span class="sxs-lookup"><span data-stu-id="2f1c2-139">String</span></span>|<span data-ttu-id="2f1c2-140">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-141">priority</span><span class="sxs-lookup"><span data-stu-id="2f1c2-141">priority</span></span>|<span data-ttu-id="2f1c2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1c2-142">Int32</span></span>|<span data-ttu-id="2f1c2-143">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f1c2-144">createdDateTime</span></span>|<span data-ttu-id="2f1c2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f1c2-145">DateTimeOffset</span></span>|<span data-ttu-id="2f1c2-146">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f1c2-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2f1c2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f1c2-148">DateTimeOffset</span></span>|<span data-ttu-id="2f1c2-149">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-150">version</span><span class="sxs-lookup"><span data-stu-id="2f1c2-150">version</span></span>|<span data-ttu-id="2f1c2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1c2-151">Int32</span></span>|<span data-ttu-id="2f1c2-152">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2f1c2-153">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="2f1c2-153">showInstallationProgress</span></span>|<span data-ttu-id="2f1c2-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f1c2-154">Boolean</span></span>|<span data-ttu-id="2f1c2-155">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="2f1c2-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="2f1c2-156">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="2f1c2-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="2f1c2-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f1c2-157">Boolean</span></span>|<span data-ttu-id="2f1c2-158">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="2f1c2-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="2f1c2-159">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="2f1c2-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="2f1c2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f1c2-160">Boolean</span></span>|<span data-ttu-id="2f1c2-161">允许或阻止在安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="2f1c2-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="2f1c2-162">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="2f1c2-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="2f1c2-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f1c2-163">Boolean</span></span>|<span data-ttu-id="2f1c2-164">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="2f1c2-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="2f1c2-165">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="2f1c2-165">customErrorMessage</span></span>|<span data-ttu-id="2f1c2-166">String</span><span class="sxs-lookup"><span data-stu-id="2f1c2-166">String</span></span>|<span data-ttu-id="2f1c2-167">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="2f1c2-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="2f1c2-168">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="2f1c2-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="2f1c2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1c2-169">Int32</span></span>|<span data-ttu-id="2f1c2-170">设置安装进度超时 (分钟)</span><span class="sxs-lookup"><span data-stu-id="2f1c2-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="2f1c2-171">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="2f1c2-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="2f1c2-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f1c2-172">Boolean</span></span>|<span data-ttu-id="2f1c2-173">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="2f1c2-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="2f1c2-174">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="2f1c2-174">selectedMobileAppIds</span></span>|<span data-ttu-id="2f1c2-175">String 集合</span><span class="sxs-lookup"><span data-stu-id="2f1c2-175">String collection</span></span>|<span data-ttu-id="2f1c2-176">选定的应用程序跟踪安装状态</span><span class="sxs-lookup"><span data-stu-id="2f1c2-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="2f1c2-177">响应</span><span class="sxs-lookup"><span data-stu-id="2f1c2-177">Response</span></span>
<span data-ttu-id="2f1c2-178">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-178">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f1c2-179">示例</span><span class="sxs-lookup"><span data-stu-id="2f1c2-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f1c2-180">请求</span><span class="sxs-lookup"><span data-stu-id="2f1c2-180">Request</span></span>
<span data-ttu-id="2f1c2-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="2f1c2-182">响应</span><span class="sxs-lookup"><span data-stu-id="2f1c2-182">Response</span></span>
<span data-ttu-id="2f1c2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f1c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




