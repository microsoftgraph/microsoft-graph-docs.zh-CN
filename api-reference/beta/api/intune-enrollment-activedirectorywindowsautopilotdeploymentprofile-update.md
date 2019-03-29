---
title: 更新 activeDirectoryWindowsAutopilotDeploymentProfile
description: 更新 activeDirectoryWindowsAutopilotDeploymentProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27edb3659d220a56a97d955ab9c296c640e922f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973332"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="9f9ce-103">更新 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="9f9ce-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="9f9ce-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f9ce-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f9ce-106">更新[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f9ce-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f9ce-107">Prerequisites</span></span>
<span data-ttu-id="9f9ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f9ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f9ce-110">Permission type</span></span>|<span data-ttu-id="9f9ce-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f9ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f9ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f9ce-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f9ce-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f9ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f9ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-115">Not supported.</span></span>|
|<span data-ttu-id="9f9ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f9ce-116">Application</span></span>|<span data-ttu-id="9f9ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f9ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f9ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="9f9ce-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f9ce-119">Request headers</span></span>
|<span data-ttu-id="9f9ce-120">标头</span><span class="sxs-lookup"><span data-stu-id="9f9ce-120">Header</span></span>|<span data-ttu-id="9f9ce-121">值</span><span class="sxs-lookup"><span data-stu-id="9f9ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f9ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f9ce-122">Authorization</span></span>|<span data-ttu-id="9f9ce-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f9ce-124">接受</span><span class="sxs-lookup"><span data-stu-id="9f9ce-124">Accept</span></span>|<span data-ttu-id="9f9ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f9ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f9ce-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f9ce-126">Request body</span></span>
<span data-ttu-id="9f9ce-127">在请求正文中, 提供[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="9f9ce-128">下表显示创建[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="9f9ce-129">属性</span><span class="sxs-lookup"><span data-stu-id="9f9ce-129">Property</span></span>|<span data-ttu-id="9f9ce-130">类型</span><span class="sxs-lookup"><span data-stu-id="9f9ce-130">Type</span></span>|<span data-ttu-id="9f9ce-131">说明</span><span class="sxs-lookup"><span data-stu-id="9f9ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f9ce-132">id</span><span class="sxs-lookup"><span data-stu-id="9f9ce-132">id</span></span>|<span data-ttu-id="9f9ce-133">String</span><span class="sxs-lookup"><span data-stu-id="9f9ce-133">String</span></span>|<span data-ttu-id="9f9ce-134">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="9f9ce-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9f9ce-135">displayName</span></span>|<span data-ttu-id="9f9ce-136">String</span><span class="sxs-lookup"><span data-stu-id="9f9ce-136">String</span></span>|<span data-ttu-id="9f9ce-137">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="9f9ce-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-138">description</span><span class="sxs-lookup"><span data-stu-id="9f9ce-138">description</span></span>|<span data-ttu-id="9f9ce-139">String</span><span class="sxs-lookup"><span data-stu-id="9f9ce-139">String</span></span>|<span data-ttu-id="9f9ce-140">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="9f9ce-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-141">language</span><span class="sxs-lookup"><span data-stu-id="9f9ce-141">language</span></span>|<span data-ttu-id="9f9ce-142">String</span><span class="sxs-lookup"><span data-stu-id="9f9ce-142">String</span></span>|<span data-ttu-id="9f9ce-143">在继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="9f9ce-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9ce-144">createdDateTime</span></span>|<span data-ttu-id="9f9ce-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9ce-145">DateTimeOffset</span></span>|<span data-ttu-id="9f9ce-146">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="9f9ce-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9ce-147">lastModifiedDateTime</span></span>|<span data-ttu-id="9f9ce-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9ce-148">DateTimeOffset</span></span>|<span data-ttu-id="9f9ce-149">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的个人资料的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="9f9ce-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="9f9ce-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="9f9ce-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="9f9ce-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="9f9ce-152">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的 "现成体验" 设置</span><span class="sxs-lookup"><span data-stu-id="9f9ce-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="9f9ce-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="9f9ce-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="9f9ce-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="9f9ce-155">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="9f9ce-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="9f9ce-156">extractHardwareHash</span></span>|<span data-ttu-id="9f9ce-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9ce-157">Boolean</span></span>|<span data-ttu-id="9f9ce-158">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="9f9ce-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="9f9ce-159">deviceNameTemplate</span></span>|<span data-ttu-id="9f9ce-160">String</span><span class="sxs-lookup"><span data-stu-id="9f9ce-160">String</span></span>|<span data-ttu-id="9f9ce-161">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="9f9ce-162">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="9f9ce-163">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="9f9ce-164">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9f9ce-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9f9ce-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="9f9ce-165">deviceType</span></span>|[<span data-ttu-id="9f9ce-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="9f9ce-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="9f9ce-167">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="9f9ce-168">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="9f9ce-169">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="9f9ce-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="9f9ce-170">enableWhiteGlove</span></span>|<span data-ttu-id="9f9ce-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9ce-171">Boolean</span></span>|<span data-ttu-id="9f9ce-172">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="9f9ce-173">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9f9ce-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9f9ce-174">响应</span><span class="sxs-lookup"><span data-stu-id="9f9ce-174">Response</span></span>
<span data-ttu-id="9f9ce-175">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-175">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f9ce-176">示例</span><span class="sxs-lookup"><span data-stu-id="9f9ce-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f9ce-177">请求</span><span class="sxs-lookup"><span data-stu-id="9f9ce-177">Request</span></span>
<span data-ttu-id="9f9ce-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
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

### <a name="response"></a><span data-ttu-id="9f9ce-179">响应</span><span class="sxs-lookup"><span data-stu-id="9f9ce-179">Response</span></span>
<span data-ttu-id="9f9ce-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f9ce-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




