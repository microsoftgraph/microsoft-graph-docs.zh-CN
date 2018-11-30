---
title: 更新 activeDirectoryWindowsAutopilotDeploymentProfile
description: 更新 activeDirectoryWindowsAutopilotDeploymentProfile 对象的属性。
ms.openlocfilehash: 11b6122167ad29bfa29d9d86931436cc02aac690
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043143"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="cff2f-103">更新 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="cff2f-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="cff2f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cff2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cff2f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cff2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cff2f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cff2f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cff2f-107">更新[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cff2f-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cff2f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cff2f-108">Prerequisites</span></span>
<span data-ttu-id="cff2f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cff2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cff2f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cff2f-111">Permission type</span></span>|<span data-ttu-id="cff2f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cff2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff2f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cff2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cff2f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cff2f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cff2f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cff2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff2f-116">Not supported.</span></span>|
|<span data-ttu-id="cff2f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cff2f-117">Application</span></span>|<span data-ttu-id="cff2f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff2f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cff2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="cff2f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cff2f-120">Request headers</span></span>
|<span data-ttu-id="cff2f-121">标头</span><span class="sxs-lookup"><span data-stu-id="cff2f-121">Header</span></span>|<span data-ttu-id="cff2f-122">值</span><span class="sxs-lookup"><span data-stu-id="cff2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cff2f-123">Authorization</span></span>|<span data-ttu-id="cff2f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cff2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cff2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cff2f-125">Accept</span></span>|<span data-ttu-id="cff2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cff2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff2f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cff2f-127">Request body</span></span>
<span data-ttu-id="cff2f-128">在请求正文中，提供[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cff2f-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="cff2f-129">下表显示时创建[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cff2f-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="cff2f-130">属性</span><span class="sxs-lookup"><span data-stu-id="cff2f-130">Property</span></span>|<span data-ttu-id="cff2f-131">类型</span><span class="sxs-lookup"><span data-stu-id="cff2f-131">Type</span></span>|<span data-ttu-id="cff2f-132">说明</span><span class="sxs-lookup"><span data-stu-id="cff2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cff2f-133">id</span><span class="sxs-lookup"><span data-stu-id="cff2f-133">id</span></span>|<span data-ttu-id="cff2f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cff2f-134">String</span></span>|<span data-ttu-id="cff2f-135">配置文件从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的键</span><span class="sxs-lookup"><span data-stu-id="cff2f-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cff2f-136">displayName</span></span>|<span data-ttu-id="cff2f-137">字符串</span><span class="sxs-lookup"><span data-stu-id="cff2f-137">String</span></span>|<span data-ttu-id="cff2f-138">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cff2f-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-139">说明</span><span class="sxs-lookup"><span data-stu-id="cff2f-139">description</span></span>|<span data-ttu-id="cff2f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="cff2f-140">String</span></span>|<span data-ttu-id="cff2f-141">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cff2f-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-142">language</span><span class="sxs-lookup"><span data-stu-id="cff2f-142">language</span></span>|<span data-ttu-id="cff2f-143">String</span><span class="sxs-lookup"><span data-stu-id="cff2f-143">String</span></span>|<span data-ttu-id="cff2f-144">在从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="cff2f-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cff2f-145">createdDateTime</span></span>|<span data-ttu-id="cff2f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cff2f-146">DateTimeOffset</span></span>|<span data-ttu-id="cff2f-147">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件创建时间继承</span><span class="sxs-lookup"><span data-stu-id="cff2f-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cff2f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cff2f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cff2f-149">DateTimeOffset</span></span>|<span data-ttu-id="cff2f-150">上次修改配置文件从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)时间继承</span><span class="sxs-lookup"><span data-stu-id="cff2f-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="cff2f-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="cff2f-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="cff2f-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="cff2f-153">即开体验从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)设置继承</span><span class="sxs-lookup"><span data-stu-id="cff2f-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="cff2f-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="cff2f-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="cff2f-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="cff2f-156">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)设置继承注册状态屏幕</span><span class="sxs-lookup"><span data-stu-id="cff2f-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="cff2f-157">extractHardwareHash</span></span>|<span data-ttu-id="cff2f-158">布尔</span><span class="sxs-lookup"><span data-stu-id="cff2f-158">Boolean</span></span>|<span data-ttu-id="cff2f-159">配置文件继承从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="cff2f-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="cff2f-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="cff2f-160">deviceNameTemplate</span></span>|<span data-ttu-id="cff2f-161">字符串</span><span class="sxs-lookup"><span data-stu-id="cff2f-161">String</span></span>|<span data-ttu-id="cff2f-162">用于自动执行某些操作设备命名的模板。</span><span class="sxs-lookup"><span data-stu-id="cff2f-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="cff2f-163">这可以是自定义文本，并且还可以包含该设备，序列号或随机生成的编号。</span><span class="sxs-lookup"><span data-stu-id="cff2f-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="cff2f-164">由模板生成的文本的总长度可不超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="cff2f-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="cff2f-165">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cff2f-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cff2f-166">响应</span><span class="sxs-lookup"><span data-stu-id="cff2f-166">Response</span></span>
<span data-ttu-id="cff2f-167">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cff2f-167">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff2f-168">示例</span><span class="sxs-lookup"><span data-stu-id="cff2f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="cff2f-169">请求</span><span class="sxs-lookup"><span data-stu-id="cff2f-169">Request</span></span>
<span data-ttu-id="cff2f-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cff2f-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1021

{
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="cff2f-171">响应</span><span class="sxs-lookup"><span data-stu-id="cff2f-171">Response</span></span>
<span data-ttu-id="cff2f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cff2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

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
  "deviceNameTemplate": "Device Name Template value"
}
```





