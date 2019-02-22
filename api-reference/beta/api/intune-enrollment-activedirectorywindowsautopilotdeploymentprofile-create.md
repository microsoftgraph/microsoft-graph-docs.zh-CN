---
title: 创建 activeDirectoryWindowsAutopilotDeploymentProfile
description: 创建新的 activeDirectoryWindowsAutopilotDeploymentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8eb470994fc0227cfce3ad497bfe933df646b049
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162970"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="5fd3e-103">创建 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="5fd3e-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="5fd3e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fd3e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fd3e-106">创建新的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fd3e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5fd3e-107">Prerequisites</span></span>
<span data-ttu-id="5fd3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5fd3e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fd3e-110">Permission type</span></span>|<span data-ttu-id="5fd3e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5fd3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fd3e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fd3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fd3e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fd3e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5fd3e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fd3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fd3e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-115">Not supported.</span></span>|
|<span data-ttu-id="5fd3e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fd3e-116">Application</span></span>|<span data-ttu-id="5fd3e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fd3e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fd3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5fd3e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fd3e-119">Request headers</span></span>
|<span data-ttu-id="5fd3e-120">标头</span><span class="sxs-lookup"><span data-stu-id="5fd3e-120">Header</span></span>|<span data-ttu-id="5fd3e-121">值</span><span class="sxs-lookup"><span data-stu-id="5fd3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fd3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fd3e-122">Authorization</span></span>|<span data-ttu-id="5fd3e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fd3e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5fd3e-124">Accept</span></span>|<span data-ttu-id="5fd3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5fd3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fd3e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fd3e-126">Request body</span></span>
<span data-ttu-id="5fd3e-127">在请求正文中, 提供 activeDirectoryWindowsAutopilotDeploymentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="5fd3e-128">下表显示创建 activeDirectoryWindowsAutopilotDeploymentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="5fd3e-129">属性</span><span class="sxs-lookup"><span data-stu-id="5fd3e-129">Property</span></span>|<span data-ttu-id="5fd3e-130">类型</span><span class="sxs-lookup"><span data-stu-id="5fd3e-130">Type</span></span>|<span data-ttu-id="5fd3e-131">说明</span><span class="sxs-lookup"><span data-stu-id="5fd3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fd3e-132">id</span><span class="sxs-lookup"><span data-stu-id="5fd3e-132">id</span></span>|<span data-ttu-id="5fd3e-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="5fd3e-133">String</span></span>|<span data-ttu-id="5fd3e-134">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="5fd3e-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5fd3e-135">displayName</span></span>|<span data-ttu-id="5fd3e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="5fd3e-136">String</span></span>|<span data-ttu-id="5fd3e-137">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="5fd3e-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-138">说明</span><span class="sxs-lookup"><span data-stu-id="5fd3e-138">description</span></span>|<span data-ttu-id="5fd3e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="5fd3e-139">String</span></span>|<span data-ttu-id="5fd3e-140">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="5fd3e-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-141">language</span><span class="sxs-lookup"><span data-stu-id="5fd3e-141">language</span></span>|<span data-ttu-id="5fd3e-142">String</span><span class="sxs-lookup"><span data-stu-id="5fd3e-142">String</span></span>|<span data-ttu-id="5fd3e-143">在继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="5fd3e-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fd3e-144">createdDateTime</span></span>|<span data-ttu-id="5fd3e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fd3e-145">DateTimeOffset</span></span>|<span data-ttu-id="5fd3e-146">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="5fd3e-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fd3e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="5fd3e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fd3e-148">DateTimeOffset</span></span>|<span data-ttu-id="5fd3e-149">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的个人资料的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="5fd3e-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="5fd3e-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="5fd3e-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="5fd3e-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="5fd3e-152">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的 "现成体验" 设置</span><span class="sxs-lookup"><span data-stu-id="5fd3e-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="5fd3e-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="5fd3e-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="5fd3e-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="5fd3e-155">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="5fd3e-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="5fd3e-156">extractHardwareHash</span></span>|<span data-ttu-id="5fd3e-157">布尔</span><span class="sxs-lookup"><span data-stu-id="5fd3e-157">Boolean</span></span>|<span data-ttu-id="5fd3e-158">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="5fd3e-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="5fd3e-159">deviceNameTemplate</span></span>|<span data-ttu-id="5fd3e-160">字符串</span><span class="sxs-lookup"><span data-stu-id="5fd3e-160">String</span></span>|<span data-ttu-id="5fd3e-161">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="5fd3e-162">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="5fd3e-163">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="5fd3e-164">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5fd3e-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="5fd3e-165">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="5fd3e-165">enableWhiteGlove</span></span>|<span data-ttu-id="5fd3e-166">布尔</span><span class="sxs-lookup"><span data-stu-id="5fd3e-166">Boolean</span></span>|<span data-ttu-id="5fd3e-167">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="5fd3e-168">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5fd3e-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5fd3e-169">响应</span><span class="sxs-lookup"><span data-stu-id="5fd3e-169">Response</span></span>
<span data-ttu-id="5fd3e-170">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-170">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fd3e-171">示例</span><span class="sxs-lookup"><span data-stu-id="5fd3e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fd3e-172">请求</span><span class="sxs-lookup"><span data-stu-id="5fd3e-172">Request</span></span>
<span data-ttu-id="5fd3e-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1073

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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

### <a name="response"></a><span data-ttu-id="5fd3e-174">响应</span><span class="sxs-lookup"><span data-stu-id="5fd3e-174">Response</span></span>
<span data-ttu-id="5fd3e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fd3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1245

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
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




