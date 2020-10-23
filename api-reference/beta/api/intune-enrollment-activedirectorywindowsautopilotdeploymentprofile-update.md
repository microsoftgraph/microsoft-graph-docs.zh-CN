---
title: 更新 activeDirectoryWindowsAutopilotDeploymentProfile
description: 更新 activeDirectoryWindowsAutopilotDeploymentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9b7e5537bec9169dcaa44e89b424e7f521f8a9b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734390"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="29539-103">更新 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="29539-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="29539-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29539-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29539-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29539-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29539-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29539-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29539-107">更新 [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="29539-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29539-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29539-108">Prerequisites</span></span>
<span data-ttu-id="29539-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29539-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29539-111">Permission type</span></span>|<span data-ttu-id="29539-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29539-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29539-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29539-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29539-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29539-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29539-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29539-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29539-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29539-116">Not supported.</span></span>|
|<span data-ttu-id="29539-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29539-117">Application</span></span>|<span data-ttu-id="29539-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29539-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29539-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29539-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="29539-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29539-120">Request headers</span></span>
|<span data-ttu-id="29539-121">标头</span><span class="sxs-lookup"><span data-stu-id="29539-121">Header</span></span>|<span data-ttu-id="29539-122">值</span><span class="sxs-lookup"><span data-stu-id="29539-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29539-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29539-123">Authorization</span></span>|<span data-ttu-id="29539-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29539-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29539-125">接受</span><span class="sxs-lookup"><span data-stu-id="29539-125">Accept</span></span>|<span data-ttu-id="29539-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29539-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29539-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29539-127">Request body</span></span>
<span data-ttu-id="29539-128">在请求正文中，提供 [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29539-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="29539-129">下表显示创建 [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29539-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="29539-130">属性</span><span class="sxs-lookup"><span data-stu-id="29539-130">Property</span></span>|<span data-ttu-id="29539-131">类型</span><span class="sxs-lookup"><span data-stu-id="29539-131">Type</span></span>|<span data-ttu-id="29539-132">说明</span><span class="sxs-lookup"><span data-stu-id="29539-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29539-133">id</span><span class="sxs-lookup"><span data-stu-id="29539-133">id</span></span>|<span data-ttu-id="29539-134">String</span><span class="sxs-lookup"><span data-stu-id="29539-134">String</span></span>|<span data-ttu-id="29539-135">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="29539-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-136">displayName</span><span class="sxs-lookup"><span data-stu-id="29539-136">displayName</span></span>|<span data-ttu-id="29539-137">String</span><span class="sxs-lookup"><span data-stu-id="29539-137">String</span></span>|<span data-ttu-id="29539-138">继承自[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="29539-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-139">说明</span><span class="sxs-lookup"><span data-stu-id="29539-139">description</span></span>|<span data-ttu-id="29539-140">String</span><span class="sxs-lookup"><span data-stu-id="29539-140">String</span></span>|<span data-ttu-id="29539-141">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="29539-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-142">language</span><span class="sxs-lookup"><span data-stu-id="29539-142">language</span></span>|<span data-ttu-id="29539-143">String</span><span class="sxs-lookup"><span data-stu-id="29539-143">String</span></span>|<span data-ttu-id="29539-144">在继承自[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)的设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="29539-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29539-145">createdDateTime</span></span>|<span data-ttu-id="29539-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29539-146">DateTimeOffset</span></span>|<span data-ttu-id="29539-147">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="29539-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29539-148">lastModifiedDateTime</span></span>|<span data-ttu-id="29539-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29539-149">DateTimeOffset</span></span>|<span data-ttu-id="29539-150">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的个人资料的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="29539-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="29539-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="29539-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="29539-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="29539-153">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的 "现成体验" 设置</span><span class="sxs-lookup"><span data-stu-id="29539-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="29539-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="29539-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="29539-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="29539-156">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="29539-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="29539-157">extractHardwareHash</span></span>|<span data-ttu-id="29539-158">布尔</span><span class="sxs-lookup"><span data-stu-id="29539-158">Boolean</span></span>|<span data-ttu-id="29539-159">从[WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)继承的配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="29539-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="29539-160">deviceNameTemplate</span></span>|<span data-ttu-id="29539-161">String</span><span class="sxs-lookup"><span data-stu-id="29539-161">String</span></span>|<span data-ttu-id="29539-162">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="29539-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="29539-163">它可以是自定义文本，也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="29539-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="29539-164">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="29539-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="29539-165">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="29539-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="29539-166">deviceType</span></span>|[<span data-ttu-id="29539-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="29539-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="29539-168">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="29539-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="29539-169">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="29539-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="29539-170">可取值为：`windowsPc`、`surfaceHub2`、`holoLens`。</span><span class="sxs-lookup"><span data-stu-id="29539-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="29539-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="29539-171">enableWhiteGlove</span></span>|<span data-ttu-id="29539-172">布尔</span><span class="sxs-lookup"><span data-stu-id="29539-172">Boolean</span></span>|<span data-ttu-id="29539-173">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="29539-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="29539-174">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="29539-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29539-175">roleScopeTagIds</span></span>|<span data-ttu-id="29539-176">String collection</span><span class="sxs-lookup"><span data-stu-id="29539-176">String collection</span></span>|<span data-ttu-id="29539-177">配置文件的范围标记。</span><span class="sxs-lookup"><span data-stu-id="29539-177">Scope tags for the profile.</span></span> <span data-ttu-id="29539-178">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="29539-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="29539-179">hybridAzureADJoinSkipConnectivityCheck</span><span class="sxs-lookup"><span data-stu-id="29539-179">hybridAzureADJoinSkipConnectivityCheck</span></span>|<span data-ttu-id="29539-180">布尔</span><span class="sxs-lookup"><span data-stu-id="29539-180">Boolean</span></span>|<span data-ttu-id="29539-181">即使不在 OOBE 期间建立域控制器连接，Autopilot 混合 Azure AD join 流也将继续进行。</span><span class="sxs-lookup"><span data-stu-id="29539-181">The Autopilot Hybrid Azure AD join flow will continue even if it does not establish domain controller connectivity during OOBE.</span></span>|



## <a name="response"></a><span data-ttu-id="29539-182">响应</span><span class="sxs-lookup"><span data-stu-id="29539-182">Response</span></span>
<span data-ttu-id="29539-183">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29539-183">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29539-184">示例</span><span class="sxs-lookup"><span data-stu-id="29539-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="29539-185">请求</span><span class="sxs-lookup"><span data-stu-id="29539-185">Request</span></span>
<span data-ttu-id="29539-186">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29539-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1218

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```

### <a name="response"></a><span data-ttu-id="29539-187">响应</span><span class="sxs-lookup"><span data-stu-id="29539-187">Response</span></span>
<span data-ttu-id="29539-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29539-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1390

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```





