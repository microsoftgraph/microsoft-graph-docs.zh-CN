---
title: 更新 activeDirectoryWindowsAutopilotDeploymentProfile
description: 更新 activeDirectoryWindowsAutopilotDeploymentProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 929ab9b026052422187eb4e94446011f3abb6f26
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404363"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="aa34b-103">更新 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="aa34b-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="aa34b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="aa34b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa34b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa34b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa34b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa34b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa34b-107">更新[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa34b-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa34b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa34b-108">Prerequisites</span></span>
<span data-ttu-id="aa34b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aa34b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aa34b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa34b-111">Permission type</span></span>|<span data-ttu-id="aa34b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa34b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa34b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa34b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa34b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa34b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa34b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa34b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa34b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa34b-116">Not supported.</span></span>|
|<span data-ttu-id="aa34b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa34b-117">Application</span></span>|<span data-ttu-id="aa34b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa34b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa34b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa34b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="aa34b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa34b-120">Request headers</span></span>
|<span data-ttu-id="aa34b-121">标头</span><span class="sxs-lookup"><span data-stu-id="aa34b-121">Header</span></span>|<span data-ttu-id="aa34b-122">值</span><span class="sxs-lookup"><span data-stu-id="aa34b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa34b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa34b-123">Authorization</span></span>|<span data-ttu-id="aa34b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa34b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa34b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa34b-125">Accept</span></span>|<span data-ttu-id="aa34b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa34b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa34b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa34b-127">Request body</span></span>
<span data-ttu-id="aa34b-128">在请求正文中，提供[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa34b-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="aa34b-129">下表显示时创建[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa34b-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="aa34b-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa34b-130">Property</span></span>|<span data-ttu-id="aa34b-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa34b-131">Type</span></span>|<span data-ttu-id="aa34b-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa34b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa34b-133">id</span><span class="sxs-lookup"><span data-stu-id="aa34b-133">id</span></span>|<span data-ttu-id="aa34b-134">String</span><span class="sxs-lookup"><span data-stu-id="aa34b-134">String</span></span>|<span data-ttu-id="aa34b-135">配置文件从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的键</span><span class="sxs-lookup"><span data-stu-id="aa34b-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="aa34b-136">displayName</span></span>|<span data-ttu-id="aa34b-137">String</span><span class="sxs-lookup"><span data-stu-id="aa34b-137">String</span></span>|<span data-ttu-id="aa34b-138">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="aa34b-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-139">说明</span><span class="sxs-lookup"><span data-stu-id="aa34b-139">description</span></span>|<span data-ttu-id="aa34b-140">String</span><span class="sxs-lookup"><span data-stu-id="aa34b-140">String</span></span>|<span data-ttu-id="aa34b-141">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="aa34b-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-142">language</span><span class="sxs-lookup"><span data-stu-id="aa34b-142">language</span></span>|<span data-ttu-id="aa34b-143">String</span><span class="sxs-lookup"><span data-stu-id="aa34b-143">String</span></span>|<span data-ttu-id="aa34b-144">在从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="aa34b-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa34b-145">createdDateTime</span></span>|<span data-ttu-id="aa34b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa34b-146">DateTimeOffset</span></span>|<span data-ttu-id="aa34b-147">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件创建时间继承</span><span class="sxs-lookup"><span data-stu-id="aa34b-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa34b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="aa34b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa34b-149">DateTimeOffset</span></span>|<span data-ttu-id="aa34b-150">上次修改配置文件从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)时间继承</span><span class="sxs-lookup"><span data-stu-id="aa34b-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="aa34b-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="aa34b-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="aa34b-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="aa34b-153">即开体验从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)设置继承</span><span class="sxs-lookup"><span data-stu-id="aa34b-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="aa34b-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="aa34b-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="aa34b-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="aa34b-156">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)设置继承注册状态屏幕</span><span class="sxs-lookup"><span data-stu-id="aa34b-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="aa34b-157">extractHardwareHash</span></span>|<span data-ttu-id="aa34b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa34b-158">Boolean</span></span>|<span data-ttu-id="aa34b-159">配置文件继承从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="aa34b-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="aa34b-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="aa34b-160">deviceNameTemplate</span></span>|<span data-ttu-id="aa34b-161">String</span><span class="sxs-lookup"><span data-stu-id="aa34b-161">String</span></span>|<span data-ttu-id="aa34b-162">用于自动执行某些操作设备命名的模板。</span><span class="sxs-lookup"><span data-stu-id="aa34b-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="aa34b-163">这可以是自定义文本，并且还可以包含该设备，序列号或随机生成的编号。</span><span class="sxs-lookup"><span data-stu-id="aa34b-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="aa34b-164">由模板生成的文本的总长度可不超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="aa34b-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="aa34b-165">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="aa34b-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="aa34b-166">响应</span><span class="sxs-lookup"><span data-stu-id="aa34b-166">Response</span></span>
<span data-ttu-id="aa34b-167">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa34b-167">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa34b-168">示例</span><span class="sxs-lookup"><span data-stu-id="aa34b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa34b-169">请求</span><span class="sxs-lookup"><span data-stu-id="aa34b-169">Request</span></span>
<span data-ttu-id="aa34b-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa34b-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1044

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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="aa34b-171">响应</span><span class="sxs-lookup"><span data-stu-id="aa34b-171">Response</span></span>
<span data-ttu-id="aa34b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa34b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




