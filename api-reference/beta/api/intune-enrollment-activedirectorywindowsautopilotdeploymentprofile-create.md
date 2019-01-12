---
title: 创建 activeDirectoryWindowsAutopilotDeploymentProfile
description: 创建新的 activeDirectoryWindowsAutopilotDeploymentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d0c0a2bd47af195fc39371ef81b5e571b4cd44cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980025"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="584a3-103">创建 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="584a3-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="584a3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="584a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="584a3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="584a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="584a3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="584a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="584a3-107">创建新的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="584a3-107">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="584a3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="584a3-108">Prerequisites</span></span>
<span data-ttu-id="584a3-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="584a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="584a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="584a3-111">Permission type</span></span>|<span data-ttu-id="584a3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="584a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="584a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="584a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="584a3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584a3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="584a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="584a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="584a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="584a3-116">Not supported.</span></span>|
|<span data-ttu-id="584a3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="584a3-117">Application</span></span>|<span data-ttu-id="584a3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="584a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="584a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="584a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="584a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="584a3-120">Request headers</span></span>
|<span data-ttu-id="584a3-121">标头</span><span class="sxs-lookup"><span data-stu-id="584a3-121">Header</span></span>|<span data-ttu-id="584a3-122">值</span><span class="sxs-lookup"><span data-stu-id="584a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="584a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="584a3-123">Authorization</span></span>|<span data-ttu-id="584a3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="584a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="584a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="584a3-125">Accept</span></span>|<span data-ttu-id="584a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="584a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="584a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="584a3-127">Request body</span></span>
<span data-ttu-id="584a3-128">在请求正文中，提供 activeDirectoryWindowsAutopilotDeploymentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="584a3-128">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="584a3-129">下表显示时创建 activeDirectoryWindowsAutopilotDeploymentProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="584a3-129">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="584a3-130">属性</span><span class="sxs-lookup"><span data-stu-id="584a3-130">Property</span></span>|<span data-ttu-id="584a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="584a3-131">Type</span></span>|<span data-ttu-id="584a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="584a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="584a3-133">id</span><span class="sxs-lookup"><span data-stu-id="584a3-133">id</span></span>|<span data-ttu-id="584a3-134">字符串</span><span class="sxs-lookup"><span data-stu-id="584a3-134">String</span></span>|<span data-ttu-id="584a3-135">配置文件从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)继承的键</span><span class="sxs-lookup"><span data-stu-id="584a3-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="584a3-136">displayName</span></span>|<span data-ttu-id="584a3-137">字符串</span><span class="sxs-lookup"><span data-stu-id="584a3-137">String</span></span>|<span data-ttu-id="584a3-138">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="584a3-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-139">说明</span><span class="sxs-lookup"><span data-stu-id="584a3-139">description</span></span>|<span data-ttu-id="584a3-140">字符串</span><span class="sxs-lookup"><span data-stu-id="584a3-140">String</span></span>|<span data-ttu-id="584a3-141">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="584a3-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-142">language</span><span class="sxs-lookup"><span data-stu-id="584a3-142">language</span></span>|<span data-ttu-id="584a3-143">String</span><span class="sxs-lookup"><span data-stu-id="584a3-143">String</span></span>|<span data-ttu-id="584a3-144">在从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的继承设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="584a3-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="584a3-145">createdDateTime</span></span>|<span data-ttu-id="584a3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="584a3-146">DateTimeOffset</span></span>|<span data-ttu-id="584a3-147">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)的配置文件创建时间继承</span><span class="sxs-lookup"><span data-stu-id="584a3-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="584a3-148">lastModifiedDateTime</span></span>|<span data-ttu-id="584a3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="584a3-149">DateTimeOffset</span></span>|<span data-ttu-id="584a3-150">上次修改配置文件从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)时间继承</span><span class="sxs-lookup"><span data-stu-id="584a3-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="584a3-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="584a3-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="584a3-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="584a3-153">即开体验从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)设置继承</span><span class="sxs-lookup"><span data-stu-id="584a3-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="584a3-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="584a3-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="584a3-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="584a3-156">从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)设置继承注册状态屏幕</span><span class="sxs-lookup"><span data-stu-id="584a3-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="584a3-157">extractHardwareHash</span></span>|<span data-ttu-id="584a3-158">布尔</span><span class="sxs-lookup"><span data-stu-id="584a3-158">Boolean</span></span>|<span data-ttu-id="584a3-159">配置文件继承从[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="584a3-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="584a3-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="584a3-160">deviceNameTemplate</span></span>|<span data-ttu-id="584a3-161">字符串</span><span class="sxs-lookup"><span data-stu-id="584a3-161">String</span></span>|<span data-ttu-id="584a3-162">用于自动执行某些操作设备命名的模板。</span><span class="sxs-lookup"><span data-stu-id="584a3-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="584a3-163">这可以是自定义文本，并且还可以包含该设备，序列号或随机生成的编号。</span><span class="sxs-lookup"><span data-stu-id="584a3-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="584a3-164">由模板生成的文本的总长度可不超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="584a3-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="584a3-165">继承自[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="584a3-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="584a3-166">响应</span><span class="sxs-lookup"><span data-stu-id="584a3-166">Response</span></span>
<span data-ttu-id="584a3-167">如果成功，此方法返回`201 Created`响应代码和响应正文中的[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="584a3-167">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="584a3-168">示例</span><span class="sxs-lookup"><span data-stu-id="584a3-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="584a3-169">请求</span><span class="sxs-lookup"><span data-stu-id="584a3-169">Request</span></span>
<span data-ttu-id="584a3-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="584a3-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1108

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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

### <a name="response"></a><span data-ttu-id="584a3-171">响应</span><span class="sxs-lookup"><span data-stu-id="584a3-171">Response</span></span>
<span data-ttu-id="584a3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="584a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





