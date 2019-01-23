---
title: 创建 windows10EnrollmentCompletionPageConfiguration
description: 创建新的 windows10EnrollmentCompletionPageConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4e7797ac1cd3ca46724c046e43bfa1fa1649ebb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411356"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="7ab50-103">创建 windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ab50-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="7ab50-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7ab50-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ab50-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ab50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ab50-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ab50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ab50-107">创建新的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ab50-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ab50-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ab50-108">Prerequisites</span></span>
<span data-ttu-id="7ab50-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7ab50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ab50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ab50-111">Permission type</span></span>|<span data-ttu-id="7ab50-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ab50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ab50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ab50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ab50-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ab50-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ab50-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ab50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ab50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ab50-116">Not supported.</span></span>|
|<span data-ttu-id="7ab50-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ab50-117">Application</span></span>|<span data-ttu-id="7ab50-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ab50-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ab50-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ab50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ab50-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ab50-120">Request headers</span></span>
|<span data-ttu-id="7ab50-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ab50-121">Header</span></span>|<span data-ttu-id="7ab50-122">值</span><span class="sxs-lookup"><span data-stu-id="7ab50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ab50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ab50-123">Authorization</span></span>|<span data-ttu-id="7ab50-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ab50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ab50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ab50-125">Accept</span></span>|<span data-ttu-id="7ab50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ab50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ab50-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ab50-127">Request body</span></span>
<span data-ttu-id="7ab50-128">在请求正文中，提供 windows10EnrollmentCompletionPageConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ab50-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="7ab50-129">下表显示时创建 windows10EnrollmentCompletionPageConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ab50-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="7ab50-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ab50-130">Property</span></span>|<span data-ttu-id="7ab50-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ab50-131">Type</span></span>|<span data-ttu-id="7ab50-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ab50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ab50-133">id</span><span class="sxs-lookup"><span data-stu-id="7ab50-133">id</span></span>|<span data-ttu-id="7ab50-134">String</span><span class="sxs-lookup"><span data-stu-id="7ab50-134">String</span></span>|<span data-ttu-id="7ab50-135">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ab50-136">displayName</span></span>|<span data-ttu-id="7ab50-137">String</span><span class="sxs-lookup"><span data-stu-id="7ab50-137">String</span></span>|<span data-ttu-id="7ab50-138">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-139">description</span><span class="sxs-lookup"><span data-stu-id="7ab50-139">description</span></span>|<span data-ttu-id="7ab50-140">String</span><span class="sxs-lookup"><span data-stu-id="7ab50-140">String</span></span>|<span data-ttu-id="7ab50-141">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-142">priority</span><span class="sxs-lookup"><span data-stu-id="7ab50-142">priority</span></span>|<span data-ttu-id="7ab50-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7ab50-143">Int32</span></span>|<span data-ttu-id="7ab50-144">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ab50-145">createdDateTime</span></span>|<span data-ttu-id="7ab50-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ab50-146">DateTimeOffset</span></span>|<span data-ttu-id="7ab50-147">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ab50-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7ab50-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ab50-149">DateTimeOffset</span></span>|<span data-ttu-id="7ab50-150">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-151">version</span><span class="sxs-lookup"><span data-stu-id="7ab50-151">version</span></span>|<span data-ttu-id="7ab50-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7ab50-152">Int32</span></span>|<span data-ttu-id="7ab50-153">尚未记录。继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ab50-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ab50-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="7ab50-154">showInstallationProgress</span></span>|<span data-ttu-id="7ab50-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab50-155">Boolean</span></span>|<span data-ttu-id="7ab50-156">显示或隐藏用户安装进度</span><span class="sxs-lookup"><span data-stu-id="7ab50-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="7ab50-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="7ab50-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="7ab50-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab50-158">Boolean</span></span>|<span data-ttu-id="7ab50-159">允许用户重试上安装失败的设置</span><span class="sxs-lookup"><span data-stu-id="7ab50-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="7ab50-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7ab50-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="7ab50-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab50-161">Boolean</span></span>|<span data-ttu-id="7ab50-162">允许或阻止安装失败时重置设备</span><span class="sxs-lookup"><span data-stu-id="7ab50-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="7ab50-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7ab50-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="7ab50-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab50-164">Boolean</span></span>|<span data-ttu-id="7ab50-165">允许或阻止上安装失败日志集合</span><span class="sxs-lookup"><span data-stu-id="7ab50-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="7ab50-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="7ab50-166">customErrorMessage</span></span>|<span data-ttu-id="7ab50-167">String</span><span class="sxs-lookup"><span data-stu-id="7ab50-167">String</span></span>|<span data-ttu-id="7ab50-168">设置要在安装失败时显示自定义错误消息</span><span class="sxs-lookup"><span data-stu-id="7ab50-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="7ab50-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7ab50-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="7ab50-170">Int32</span><span class="sxs-lookup"><span data-stu-id="7ab50-170">Int32</span></span>|<span data-ttu-id="7ab50-171">以分钟为单位的设置安装进度超时</span><span class="sxs-lookup"><span data-stu-id="7ab50-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="7ab50-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7ab50-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="7ab50-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab50-173">Boolean</span></span>|<span data-ttu-id="7ab50-174">允许用户继续使用设备上安装失败</span><span class="sxs-lookup"><span data-stu-id="7ab50-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="7ab50-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="7ab50-175">selectedMobileAppIds</span></span>|<span data-ttu-id="7ab50-176">String 集合</span><span class="sxs-lookup"><span data-stu-id="7ab50-176">String collection</span></span>|<span data-ttu-id="7ab50-177">所选应用程序来跟踪的安装状态</span><span class="sxs-lookup"><span data-stu-id="7ab50-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="7ab50-178">响应</span><span class="sxs-lookup"><span data-stu-id="7ab50-178">Response</span></span>
<span data-ttu-id="7ab50-179">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ab50-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ab50-180">示例</span><span class="sxs-lookup"><span data-stu-id="7ab50-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ab50-181">请求</span><span class="sxs-lookup"><span data-stu-id="7ab50-181">Request</span></span>
<span data-ttu-id="7ab50-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ab50-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ab50-183">响应</span><span class="sxs-lookup"><span data-stu-id="7ab50-183">Response</span></span>
<span data-ttu-id="7ab50-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ab50-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




