---
title: 创建 azureADWindowsAutopilotDeploymentProfile
description: 创建新的 azureADWindowsAutopilotDeploymentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c31f0d32530ba5a080b70631b67f11a76145b9d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143363"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="c7c40-103">创建 azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c7c40-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="c7c40-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7c40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c40-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7c40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c40-106">创建新的[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7c40-106">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c40-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7c40-107">Prerequisites</span></span>
<span data-ttu-id="c7c40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c7c40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7c40-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7c40-110">Permission type</span></span>|<span data-ttu-id="c7c40-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7c40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c40-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c40-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c40-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c7c40-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c40-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c40-115">Not supported.</span></span>|
|<span data-ttu-id="c7c40-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7c40-116">Application</span></span>|<span data-ttu-id="c7c40-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c40-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7c40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c7c40-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7c40-119">Request headers</span></span>
|<span data-ttu-id="c7c40-120">标头</span><span class="sxs-lookup"><span data-stu-id="c7c40-120">Header</span></span>|<span data-ttu-id="c7c40-121">值</span><span class="sxs-lookup"><span data-stu-id="c7c40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c40-122">Authorization</span></span>|<span data-ttu-id="c7c40-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7c40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c40-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c7c40-124">Accept</span></span>|<span data-ttu-id="c7c40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7c40-126">Request body</span></span>
<span data-ttu-id="c7c40-127">在请求正文中, 提供 azureADWindowsAutopilotDeploymentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7c40-127">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="c7c40-128">下表显示创建 azureADWindowsAutopilotDeploymentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c7c40-128">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="c7c40-129">属性</span><span class="sxs-lookup"><span data-stu-id="c7c40-129">Property</span></span>|<span data-ttu-id="c7c40-130">类型</span><span class="sxs-lookup"><span data-stu-id="c7c40-130">Type</span></span>|<span data-ttu-id="c7c40-131">说明</span><span class="sxs-lookup"><span data-stu-id="c7c40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c40-132">id</span><span class="sxs-lookup"><span data-stu-id="c7c40-132">id</span></span>|<span data-ttu-id="c7c40-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="c7c40-133">String</span></span>|<span data-ttu-id="c7c40-134">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="c7c40-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c7c40-135">displayName</span></span>|<span data-ttu-id="c7c40-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c7c40-136">String</span></span>|<span data-ttu-id="c7c40-137">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="c7c40-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-138">说明</span><span class="sxs-lookup"><span data-stu-id="c7c40-138">description</span></span>|<span data-ttu-id="c7c40-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c7c40-139">String</span></span>|<span data-ttu-id="c7c40-140">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="c7c40-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-141">language</span><span class="sxs-lookup"><span data-stu-id="c7c40-141">language</span></span>|<span data-ttu-id="c7c40-142">String</span><span class="sxs-lookup"><span data-stu-id="c7c40-142">String</span></span>|<span data-ttu-id="c7c40-143">在继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="c7c40-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c40-144">createdDateTime</span></span>|<span data-ttu-id="c7c40-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c40-145">DateTimeOffset</span></span>|<span data-ttu-id="c7c40-146">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="c7c40-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c40-147">lastModifiedDateTime</span></span>|<span data-ttu-id="c7c40-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c40-148">DateTimeOffset</span></span>|<span data-ttu-id="c7c40-149">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的个人资料的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="c7c40-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c7c40-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="c7c40-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c7c40-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="c7c40-152">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的 "现成体验" 设置</span><span class="sxs-lookup"><span data-stu-id="c7c40-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c7c40-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="c7c40-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c7c40-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="c7c40-155">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="c7c40-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="c7c40-156">extractHardwareHash</span></span>|<span data-ttu-id="c7c40-157">布尔</span><span class="sxs-lookup"><span data-stu-id="c7c40-157">Boolean</span></span>|<span data-ttu-id="c7c40-158">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="c7c40-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="c7c40-159">deviceNameTemplate</span></span>|<span data-ttu-id="c7c40-160">字符串</span><span class="sxs-lookup"><span data-stu-id="c7c40-160">String</span></span>|<span data-ttu-id="c7c40-161">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="c7c40-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="c7c40-162">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="c7c40-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="c7c40-163">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="c7c40-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="c7c40-164">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c7c40-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c7c40-165">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="c7c40-165">enableWhiteGlove</span></span>|<span data-ttu-id="c7c40-166">布尔</span><span class="sxs-lookup"><span data-stu-id="c7c40-166">Boolean</span></span>|<span data-ttu-id="c7c40-167">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="c7c40-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="c7c40-168">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c7c40-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c7c40-169">响应</span><span class="sxs-lookup"><span data-stu-id="c7c40-169">Response</span></span>
<span data-ttu-id="c7c40-170">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7c40-170">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c40-171">示例</span><span class="sxs-lookup"><span data-stu-id="c7c40-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c40-172">请求</span><span class="sxs-lookup"><span data-stu-id="c7c40-172">Request</span></span>
<span data-ttu-id="c7c40-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7c40-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1065

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="c7c40-174">响应</span><span class="sxs-lookup"><span data-stu-id="c7c40-174">Response</span></span>
<span data-ttu-id="c7c40-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7c40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1237

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "enableWhiteGlove": true
}
```




