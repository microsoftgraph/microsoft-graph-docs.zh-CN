---
title: 创建 azureADWindowsAutopilotDeploymentProfile
description: 创建新的 azureADWindowsAutopilotDeploymentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c8816c71808a2ee7175cf89c90d78d0ba6cbd7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146046"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="3676b-103">创建 azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="3676b-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="3676b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3676b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3676b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3676b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3676b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3676b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3676b-107">创建新的 [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3676b-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3676b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3676b-108">Prerequisites</span></span>
<span data-ttu-id="3676b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3676b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3676b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3676b-111">Permission type</span></span>|<span data-ttu-id="3676b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3676b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3676b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3676b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3676b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3676b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3676b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3676b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3676b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3676b-116">Not supported.</span></span>|
|<span data-ttu-id="3676b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3676b-117">Application</span></span>|<span data-ttu-id="3676b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3676b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3676b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3676b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3676b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3676b-120">Request headers</span></span>
|<span data-ttu-id="3676b-121">标头</span><span class="sxs-lookup"><span data-stu-id="3676b-121">Header</span></span>|<span data-ttu-id="3676b-122">值</span><span class="sxs-lookup"><span data-stu-id="3676b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3676b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3676b-123">Authorization</span></span>|<span data-ttu-id="3676b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3676b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3676b-125">接受</span><span class="sxs-lookup"><span data-stu-id="3676b-125">Accept</span></span>|<span data-ttu-id="3676b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3676b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3676b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3676b-127">Request body</span></span>
<span data-ttu-id="3676b-128">在请求正文中，提供 azureADWindowsAutopilotDeploymentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3676b-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="3676b-129">下表显示创建 azureADWindowsAutopilotDeploymentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3676b-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="3676b-130">属性</span><span class="sxs-lookup"><span data-stu-id="3676b-130">Property</span></span>|<span data-ttu-id="3676b-131">类型</span><span class="sxs-lookup"><span data-stu-id="3676b-131">Type</span></span>|<span data-ttu-id="3676b-132">说明</span><span class="sxs-lookup"><span data-stu-id="3676b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3676b-133">id</span><span class="sxs-lookup"><span data-stu-id="3676b-133">id</span></span>|<span data-ttu-id="3676b-134">String</span><span class="sxs-lookup"><span data-stu-id="3676b-134">String</span></span>|<span data-ttu-id="3676b-135">配置文件密钥 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3676b-136">displayName</span></span>|<span data-ttu-id="3676b-137">String</span><span class="sxs-lookup"><span data-stu-id="3676b-137">String</span></span>|<span data-ttu-id="3676b-138">配置文件的名称 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-139">说明</span><span class="sxs-lookup"><span data-stu-id="3676b-139">description</span></span>|<span data-ttu-id="3676b-140">String</span><span class="sxs-lookup"><span data-stu-id="3676b-140">String</span></span>|<span data-ttu-id="3676b-141">配置文件的说明 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-142">language</span><span class="sxs-lookup"><span data-stu-id="3676b-142">language</span></span>|<span data-ttu-id="3676b-143">String</span><span class="sxs-lookup"><span data-stu-id="3676b-143">String</span></span>|<span data-ttu-id="3676b-144">在设备上配置的语言 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3676b-145">createdDateTime</span></span>|<span data-ttu-id="3676b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3676b-146">DateTimeOffset</span></span>|<span data-ttu-id="3676b-147">配置文件创建时间 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3676b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3676b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3676b-149">DateTimeOffset</span></span>|<span data-ttu-id="3676b-150">配置文件上次修改时间 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3676b-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="3676b-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3676b-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="3676b-153">开箱体验设置 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="3676b-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="3676b-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="3676b-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="3676b-156">注册状态屏幕设置 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="3676b-157">extractHardwareHash</span></span>|<span data-ttu-id="3676b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="3676b-158">Boolean</span></span>|<span data-ttu-id="3676b-159">配置文件的 HardwareHash 提取 继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="3676b-160">deviceNameTemplate</span></span>|<span data-ttu-id="3676b-161">String</span><span class="sxs-lookup"><span data-stu-id="3676b-161">String</span></span>|<span data-ttu-id="3676b-162">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="3676b-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="3676b-163">这可以是自定义文本，还可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="3676b-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="3676b-164">模板生成的文本的总长度不能超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="3676b-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="3676b-165">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="3676b-166">deviceType</span></span>|[<span data-ttu-id="3676b-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="3676b-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="3676b-168">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="3676b-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="3676b-169">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="3676b-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="3676b-170">可取值为：`windowsPc`、`surfaceHub2`、`holoLens`。</span><span class="sxs-lookup"><span data-stu-id="3676b-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="3676b-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="3676b-171">enableWhiteGlove</span></span>|<span data-ttu-id="3676b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="3676b-172">Boolean</span></span>|<span data-ttu-id="3676b-173">为配置文件启用 Autopilot White Glove。</span><span class="sxs-lookup"><span data-stu-id="3676b-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="3676b-174">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3676b-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3676b-175">roleScopeTagIds</span></span>|<span data-ttu-id="3676b-176">String collection</span><span class="sxs-lookup"><span data-stu-id="3676b-176">String collection</span></span>|<span data-ttu-id="3676b-177">配置文件的范围标记。</span><span class="sxs-lookup"><span data-stu-id="3676b-177">Scope tags for the profile.</span></span> <span data-ttu-id="3676b-178">继承自 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3676b-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3676b-179">响应</span><span class="sxs-lookup"><span data-stu-id="3676b-179">Response</span></span>
<span data-ttu-id="3676b-180">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3676b-180">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3676b-181">示例</span><span class="sxs-lookup"><span data-stu-id="3676b-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="3676b-182">请求</span><span class="sxs-lookup"><span data-stu-id="3676b-182">Request</span></span>
<span data-ttu-id="3676b-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3676b-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1159

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
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3676b-184">响应</span><span class="sxs-lookup"><span data-stu-id="3676b-184">Response</span></span>
<span data-ttu-id="3676b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3676b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

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
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




