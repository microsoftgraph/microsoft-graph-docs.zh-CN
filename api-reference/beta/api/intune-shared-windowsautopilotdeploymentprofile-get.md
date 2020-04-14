---
title: 获取 windowsAutopilotDeploymentProfile
description: 读取 windowsAutopilotDeploymentProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b650260d1332cc8decc7cc2c21c05e31165f36e0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447369"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="8c369-103">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="8c369-103">Get windowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="8c369-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c369-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c369-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c369-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c369-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c369-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c369-107">读取[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8c369-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c369-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c369-108">Prerequisites</span></span>
<span data-ttu-id="8c369-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c369-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c369-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c369-111">Permission type</span></span>|<span data-ttu-id="8c369-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c369-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c369-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c369-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c369-114">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="8c369-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="8c369-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c369-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="8c369-116">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="8c369-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8c369-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c369-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8c369-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c369-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c369-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c369-119">Not supported.</span></span>|
|<span data-ttu-id="8c369-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c369-120">Application</span></span>||
| <span data-ttu-id="8c369-121">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="8c369-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="8c369-122">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c369-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="8c369-123">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="8c369-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8c369-124">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c369-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c369-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c369-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c369-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c369-126">Optional query parameters</span></span>
<span data-ttu-id="8c369-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c369-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c369-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c369-128">Request headers</span></span>
|<span data-ttu-id="8c369-129">标头</span><span class="sxs-lookup"><span data-stu-id="8c369-129">Header</span></span>|<span data-ttu-id="8c369-130">值</span><span class="sxs-lookup"><span data-stu-id="8c369-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c369-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c369-131">Authorization</span></span>|<span data-ttu-id="8c369-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c369-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c369-133">接受</span><span class="sxs-lookup"><span data-stu-id="8c369-133">Accept</span></span>|<span data-ttu-id="8c369-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8c369-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c369-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c369-135">Request body</span></span>
<span data-ttu-id="8c369-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c369-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c369-137">响应</span><span class="sxs-lookup"><span data-stu-id="8c369-137">Response</span></span>
<span data-ttu-id="8c369-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c369-138">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c369-139">示例</span><span class="sxs-lookup"><span data-stu-id="8c369-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c369-140">请求</span><span class="sxs-lookup"><span data-stu-id="8c369-140">Request</span></span>
<span data-ttu-id="8c369-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c369-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="8c369-142">响应</span><span class="sxs-lookup"><span data-stu-id="8c369-142">Response</span></span>
<span data-ttu-id="8c369-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c369-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
    "id": "9d6394a9-94a9-9d63-a994-639da994639d",
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
}
```






