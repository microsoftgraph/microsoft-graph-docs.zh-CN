---
title: 创建 activeDirectoryWindowsAutopilotDeploymentProfile
description: 创建新的 activeDirectoryWindowsAutopilotDeploymentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1434d4cd171c28152ad84089ea3c4ad0b04fc5e7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571667"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="2eec5-103">创建 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="2eec5-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="2eec5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2eec5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eec5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2eec5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eec5-106">创建新的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2eec5-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eec5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2eec5-107">Prerequisites</span></span>
<span data-ttu-id="2eec5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2eec5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2eec5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2eec5-110">Permission type</span></span>|<span data-ttu-id="2eec5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2eec5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eec5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2eec5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2eec5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eec5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2eec5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2eec5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eec5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2eec5-115">Not supported.</span></span>|
|<span data-ttu-id="2eec5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2eec5-116">Application</span></span>|<span data-ttu-id="2eec5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2eec5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eec5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2eec5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2eec5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2eec5-119">Request headers</span></span>
|<span data-ttu-id="2eec5-120">标头</span><span class="sxs-lookup"><span data-stu-id="2eec5-120">Header</span></span>|<span data-ttu-id="2eec5-121">值</span><span class="sxs-lookup"><span data-stu-id="2eec5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eec5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eec5-122">Authorization</span></span>|<span data-ttu-id="2eec5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2eec5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eec5-124">接受</span><span class="sxs-lookup"><span data-stu-id="2eec5-124">Accept</span></span>|<span data-ttu-id="2eec5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2eec5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eec5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2eec5-126">Request body</span></span>
<span data-ttu-id="2eec5-127">在请求正文中, 提供 activeDirectoryWindowsAutopilotDeploymentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2eec5-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="2eec5-128">下表显示创建 activeDirectoryWindowsAutopilotDeploymentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2eec5-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="2eec5-129">属性</span><span class="sxs-lookup"><span data-stu-id="2eec5-129">Property</span></span>|<span data-ttu-id="2eec5-130">类型</span><span class="sxs-lookup"><span data-stu-id="2eec5-130">Type</span></span>|<span data-ttu-id="2eec5-131">说明</span><span class="sxs-lookup"><span data-stu-id="2eec5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eec5-132">id</span><span class="sxs-lookup"><span data-stu-id="2eec5-132">id</span></span>|<span data-ttu-id="2eec5-133">String</span><span class="sxs-lookup"><span data-stu-id="2eec5-133">String</span></span>|<span data-ttu-id="2eec5-134">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="2eec5-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2eec5-135">displayName</span></span>|<span data-ttu-id="2eec5-136">String</span><span class="sxs-lookup"><span data-stu-id="2eec5-136">String</span></span>|<span data-ttu-id="2eec5-137">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="2eec5-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-138">说明</span><span class="sxs-lookup"><span data-stu-id="2eec5-138">description</span></span>|<span data-ttu-id="2eec5-139">String</span><span class="sxs-lookup"><span data-stu-id="2eec5-139">String</span></span>|<span data-ttu-id="2eec5-140">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="2eec5-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-141">language</span><span class="sxs-lookup"><span data-stu-id="2eec5-141">language</span></span>|<span data-ttu-id="2eec5-142">String</span><span class="sxs-lookup"><span data-stu-id="2eec5-142">String</span></span>|<span data-ttu-id="2eec5-143">在继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="2eec5-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2eec5-144">createdDateTime</span></span>|<span data-ttu-id="2eec5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eec5-145">DateTimeOffset</span></span>|<span data-ttu-id="2eec5-146">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="2eec5-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2eec5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2eec5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eec5-148">DateTimeOffset</span></span>|<span data-ttu-id="2eec5-149">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的个人资料的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="2eec5-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="2eec5-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="2eec5-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="2eec5-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="2eec5-152">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的 "现成体验" 设置</span><span class="sxs-lookup"><span data-stu-id="2eec5-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="2eec5-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="2eec5-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="2eec5-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="2eec5-155">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="2eec5-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="2eec5-156">extractHardwareHash</span></span>|<span data-ttu-id="2eec5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="2eec5-157">Boolean</span></span>|<span data-ttu-id="2eec5-158">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="2eec5-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="2eec5-159">deviceNameTemplate</span></span>|<span data-ttu-id="2eec5-160">String</span><span class="sxs-lookup"><span data-stu-id="2eec5-160">String</span></span>|<span data-ttu-id="2eec5-161">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="2eec5-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="2eec5-162">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="2eec5-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="2eec5-163">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="2eec5-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="2eec5-164">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2eec5-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2eec5-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="2eec5-165">deviceType</span></span>|[<span data-ttu-id="2eec5-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="2eec5-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="2eec5-167">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="2eec5-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="2eec5-168">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="2eec5-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="2eec5-169">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="2eec5-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="2eec5-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="2eec5-170">enableWhiteGlove</span></span>|<span data-ttu-id="2eec5-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="2eec5-171">Boolean</span></span>|<span data-ttu-id="2eec5-172">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="2eec5-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="2eec5-173">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2eec5-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2eec5-174">响应</span><span class="sxs-lookup"><span data-stu-id="2eec5-174">Response</span></span>
<span data-ttu-id="2eec5-175">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2eec5-175">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eec5-176">示例</span><span class="sxs-lookup"><span data-stu-id="2eec5-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eec5-177">请求</span><span class="sxs-lookup"><span data-stu-id="2eec5-177">Request</span></span>
<span data-ttu-id="2eec5-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2eec5-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1105

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
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="2eec5-179">响应</span><span class="sxs-lookup"><span data-stu-id="2eec5-179">Response</span></span>
<span data-ttu-id="2eec5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2eec5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1277

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
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true
}
```




