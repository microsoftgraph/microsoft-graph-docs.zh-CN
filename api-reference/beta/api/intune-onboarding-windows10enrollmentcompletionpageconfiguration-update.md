---
title: 更新 windows10EnrollmentCompletionPageConfiguration
description: 更新 windows10EnrollmentCompletionPageConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2219a2f2e2b5a0717fe6cc7bb954c8af11ebfd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959795"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="44d50-103">更新 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="44d50-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="44d50-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44d50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44d50-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44d50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44d50-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44d50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44d50-107">更新[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="44d50-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44d50-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44d50-108">Prerequisites</span></span>
<span data-ttu-id="44d50-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="44d50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44d50-111">Permission type</span></span>|<span data-ttu-id="44d50-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44d50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44d50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44d50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44d50-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d50-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44d50-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44d50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44d50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44d50-116">Not supported.</span></span>|
|<span data-ttu-id="44d50-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44d50-117">Application</span></span>|<span data-ttu-id="44d50-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="44d50-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44d50-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44d50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="44d50-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44d50-120">Request headers</span></span>
|<span data-ttu-id="44d50-121">标头</span><span class="sxs-lookup"><span data-stu-id="44d50-121">Header</span></span>|<span data-ttu-id="44d50-122">值</span><span class="sxs-lookup"><span data-stu-id="44d50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44d50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44d50-123">Authorization</span></span>|<span data-ttu-id="44d50-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44d50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44d50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44d50-125">Accept</span></span>|<span data-ttu-id="44d50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44d50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44d50-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44d50-127">Request body</span></span>
<span data-ttu-id="44d50-128">在请求正文中，提供[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44d50-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="44d50-129">下表显示时创建[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44d50-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="44d50-130">属性</span><span class="sxs-lookup"><span data-stu-id="44d50-130">Property</span></span>|<span data-ttu-id="44d50-131">类型</span><span class="sxs-lookup"><span data-stu-id="44d50-131">Type</span></span>|<span data-ttu-id="44d50-132">说明</span><span class="sxs-lookup"><span data-stu-id="44d50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d50-133">id</span><span class="sxs-lookup"><span data-stu-id="44d50-133">id</span></span>|<span data-ttu-id="44d50-134">String</span><span class="sxs-lookup"><span data-stu-id="44d50-134">String</span></span>|<span data-ttu-id="44d50-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-136">displayName</span><span class="sxs-lookup"><span data-stu-id="44d50-136">displayName</span></span>|<span data-ttu-id="44d50-137">String</span><span class="sxs-lookup"><span data-stu-id="44d50-137">String</span></span>|<span data-ttu-id="44d50-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-139">description</span><span class="sxs-lookup"><span data-stu-id="44d50-139">description</span></span>|<span data-ttu-id="44d50-140">String</span><span class="sxs-lookup"><span data-stu-id="44d50-140">String</span></span>|<span data-ttu-id="44d50-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-142">priority</span><span class="sxs-lookup"><span data-stu-id="44d50-142">priority</span></span>|<span data-ttu-id="44d50-143">Int32</span><span class="sxs-lookup"><span data-stu-id="44d50-143">Int32</span></span>|<span data-ttu-id="44d50-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44d50-145">createdDateTime</span></span>|<span data-ttu-id="44d50-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44d50-146">DateTimeOffset</span></span>|<span data-ttu-id="44d50-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44d50-148">lastModifiedDateTime</span></span>|<span data-ttu-id="44d50-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44d50-149">DateTimeOffset</span></span>|<span data-ttu-id="44d50-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-151">version</span><span class="sxs-lookup"><span data-stu-id="44d50-151">version</span></span>|<span data-ttu-id="44d50-152">Int32</span><span class="sxs-lookup"><span data-stu-id="44d50-152">Int32</span></span>|<span data-ttu-id="44d50-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44d50-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="44d50-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="44d50-154">showInstallationProgress</span></span>|<span data-ttu-id="44d50-155">布尔</span><span class="sxs-lookup"><span data-stu-id="44d50-155">Boolean</span></span>|<span data-ttu-id="44d50-156">显示或隐藏用户安装进度</span><span class="sxs-lookup"><span data-stu-id="44d50-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="44d50-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="44d50-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="44d50-158">布尔</span><span class="sxs-lookup"><span data-stu-id="44d50-158">Boolean</span></span>|<span data-ttu-id="44d50-159">允许用户重试上安装失败的设置</span><span class="sxs-lookup"><span data-stu-id="44d50-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="44d50-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="44d50-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="44d50-161">布尔</span><span class="sxs-lookup"><span data-stu-id="44d50-161">Boolean</span></span>|<span data-ttu-id="44d50-162">允许或阻止安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="44d50-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="44d50-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="44d50-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="44d50-164">布尔</span><span class="sxs-lookup"><span data-stu-id="44d50-164">Boolean</span></span>|<span data-ttu-id="44d50-165">允许或阻止上安装失败日志集合</span><span class="sxs-lookup"><span data-stu-id="44d50-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="44d50-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="44d50-166">customErrorMessage</span></span>|<span data-ttu-id="44d50-167">字符串</span><span class="sxs-lookup"><span data-stu-id="44d50-167">String</span></span>|<span data-ttu-id="44d50-168">设置要在安装失败时显示自定义错误消息</span><span class="sxs-lookup"><span data-stu-id="44d50-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="44d50-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="44d50-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="44d50-170">Int32</span><span class="sxs-lookup"><span data-stu-id="44d50-170">Int32</span></span>|<span data-ttu-id="44d50-171">以分钟为单位的设置安装进度超时</span><span class="sxs-lookup"><span data-stu-id="44d50-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="44d50-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="44d50-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="44d50-173">布尔</span><span class="sxs-lookup"><span data-stu-id="44d50-173">Boolean</span></span>|<span data-ttu-id="44d50-174">允许用户继续使用设备上安装失败</span><span class="sxs-lookup"><span data-stu-id="44d50-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="44d50-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="44d50-175">selectedMobileAppIds</span></span>|<span data-ttu-id="44d50-176">String 集合</span><span class="sxs-lookup"><span data-stu-id="44d50-176">String collection</span></span>|<span data-ttu-id="44d50-177">所选应用程序来跟踪的安装状态</span><span class="sxs-lookup"><span data-stu-id="44d50-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="44d50-178">响应</span><span class="sxs-lookup"><span data-stu-id="44d50-178">Response</span></span>
<span data-ttu-id="44d50-179">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="44d50-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44d50-180">示例</span><span class="sxs-lookup"><span data-stu-id="44d50-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="44d50-181">请求</span><span class="sxs-lookup"><span data-stu-id="44d50-181">Request</span></span>
<span data-ttu-id="44d50-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44d50-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 562

{
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

### <a name="response"></a><span data-ttu-id="44d50-183">响应</span><span class="sxs-lookup"><span data-stu-id="44d50-183">Response</span></span>
<span data-ttu-id="44d50-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44d50-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





