---
title: 创建 windows10EnrollmentCompletionPageConfiguration
description: 创建新的 windows10EnrollmentCompletionPageConfiguration 对象。
ms.openlocfilehash: db276cefec8a764b2ad2ddcade93bae7a518f264
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042040"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="7ac28-103">创建 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ac28-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="7ac28-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ac28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ac28-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ac28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ac28-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ac28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ac28-107">创建新的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ac28-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ac28-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ac28-108">Prerequisites</span></span>
<span data-ttu-id="7ac28-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7ac28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac28-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ac28-111">Permission type</span></span>|<span data-ttu-id="7ac28-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ac28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac28-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac28-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac28-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac28-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac28-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac28-116">Not supported.</span></span>|
|<span data-ttu-id="7ac28-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ac28-117">Application</span></span>|<span data-ttu-id="7ac28-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac28-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac28-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ac28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ac28-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ac28-120">Request headers</span></span>
|<span data-ttu-id="7ac28-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ac28-121">Header</span></span>|<span data-ttu-id="7ac28-122">值</span><span class="sxs-lookup"><span data-stu-id="7ac28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac28-123">Authorization</span></span>|<span data-ttu-id="7ac28-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ac28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac28-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ac28-125">Accept</span></span>|<span data-ttu-id="7ac28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac28-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ac28-127">Request body</span></span>
<span data-ttu-id="7ac28-128">在请求正文中，提供 windows10EnrollmentCompletionPageConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ac28-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="7ac28-129">下表显示时创建 windows10EnrollmentCompletionPageConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ac28-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="7ac28-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ac28-130">Property</span></span>|<span data-ttu-id="7ac28-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ac28-131">Type</span></span>|<span data-ttu-id="7ac28-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ac28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac28-133">id</span><span class="sxs-lookup"><span data-stu-id="7ac28-133">id</span></span>|<span data-ttu-id="7ac28-134">String</span><span class="sxs-lookup"><span data-stu-id="7ac28-134">String</span></span>|<span data-ttu-id="7ac28-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ac28-136">displayName</span></span>|<span data-ttu-id="7ac28-137">String</span><span class="sxs-lookup"><span data-stu-id="7ac28-137">String</span></span>|<span data-ttu-id="7ac28-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-139">description</span><span class="sxs-lookup"><span data-stu-id="7ac28-139">description</span></span>|<span data-ttu-id="7ac28-140">String</span><span class="sxs-lookup"><span data-stu-id="7ac28-140">String</span></span>|<span data-ttu-id="7ac28-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-142">priority</span><span class="sxs-lookup"><span data-stu-id="7ac28-142">priority</span></span>|<span data-ttu-id="7ac28-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac28-143">Int32</span></span>|<span data-ttu-id="7ac28-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac28-145">createdDateTime</span></span>|<span data-ttu-id="7ac28-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac28-146">DateTimeOffset</span></span>|<span data-ttu-id="7ac28-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac28-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7ac28-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac28-149">DateTimeOffset</span></span>|<span data-ttu-id="7ac28-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-151">version</span><span class="sxs-lookup"><span data-stu-id="7ac28-151">version</span></span>|<span data-ttu-id="7ac28-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac28-152">Int32</span></span>|<span data-ttu-id="7ac28-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ac28-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ac28-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="7ac28-154">showInstallationProgress</span></span>|<span data-ttu-id="7ac28-155">布尔</span><span class="sxs-lookup"><span data-stu-id="7ac28-155">Boolean</span></span>|<span data-ttu-id="7ac28-156">显示或隐藏用户安装进度</span><span class="sxs-lookup"><span data-stu-id="7ac28-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="7ac28-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="7ac28-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="7ac28-158">布尔</span><span class="sxs-lookup"><span data-stu-id="7ac28-158">Boolean</span></span>|<span data-ttu-id="7ac28-159">允许用户重试上安装失败的设置</span><span class="sxs-lookup"><span data-stu-id="7ac28-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="7ac28-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7ac28-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="7ac28-161">布尔</span><span class="sxs-lookup"><span data-stu-id="7ac28-161">Boolean</span></span>|<span data-ttu-id="7ac28-162">允许或阻止安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="7ac28-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="7ac28-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7ac28-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="7ac28-164">布尔</span><span class="sxs-lookup"><span data-stu-id="7ac28-164">Boolean</span></span>|<span data-ttu-id="7ac28-165">允许或阻止上安装失败日志集合</span><span class="sxs-lookup"><span data-stu-id="7ac28-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="7ac28-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="7ac28-166">customErrorMessage</span></span>|<span data-ttu-id="7ac28-167">字符串</span><span class="sxs-lookup"><span data-stu-id="7ac28-167">String</span></span>|<span data-ttu-id="7ac28-168">设置要在安装失败时显示自定义错误消息</span><span class="sxs-lookup"><span data-stu-id="7ac28-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="7ac28-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7ac28-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="7ac28-170">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac28-170">Int32</span></span>|<span data-ttu-id="7ac28-171">以分钟为单位的设置安装进度超时</span><span class="sxs-lookup"><span data-stu-id="7ac28-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="7ac28-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7ac28-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="7ac28-173">布尔</span><span class="sxs-lookup"><span data-stu-id="7ac28-173">Boolean</span></span>|<span data-ttu-id="7ac28-174">允许用户继续使用设备上安装失败</span><span class="sxs-lookup"><span data-stu-id="7ac28-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="7ac28-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="7ac28-175">selectedMobileAppIds</span></span>|<span data-ttu-id="7ac28-176">String 集合</span><span class="sxs-lookup"><span data-stu-id="7ac28-176">String collection</span></span>|<span data-ttu-id="7ac28-177">所选应用程序来跟踪的安装状态</span><span class="sxs-lookup"><span data-stu-id="7ac28-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="7ac28-178">响应</span><span class="sxs-lookup"><span data-stu-id="7ac28-178">Response</span></span>
<span data-ttu-id="7ac28-179">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ac28-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac28-180">示例</span><span class="sxs-lookup"><span data-stu-id="7ac28-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ac28-181">请求</span><span class="sxs-lookup"><span data-stu-id="7ac28-181">Request</span></span>
<span data-ttu-id="7ac28-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ac28-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="7ac28-183">响应</span><span class="sxs-lookup"><span data-stu-id="7ac28-183">Response</span></span>
<span data-ttu-id="7ac28-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ac28-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





