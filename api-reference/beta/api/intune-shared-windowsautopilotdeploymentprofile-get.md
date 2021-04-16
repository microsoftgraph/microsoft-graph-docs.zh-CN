---
title: 获取 windowsAutopilotDeploymentProfile
description: 读取 windowsAutopilotDeploymentProfile 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ab309a198887601778724f473f31e622a6ec9c0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866396"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="ce2ac-103">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="ce2ac-103">Get windowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="ce2ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce2ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce2ac-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce2ac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2ac-107">读取 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce2ac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce2ac-108">Prerequisites</span></span>
<span data-ttu-id="ce2ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce2ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce2ac-111">Permission type</span></span>|<span data-ttu-id="ce2ac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ce2ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce2ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce2ac-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ce2ac-114">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="ce2ac-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ce2ac-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2ac-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="ce2ac-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="ce2ac-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ce2ac-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2ac-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ce2ac-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce2ac-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce2ac-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-119">Not supported.</span></span>|
|<span data-ttu-id="ce2ac-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce2ac-120">Application</span></span>||
| <span data-ttu-id="ce2ac-121">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="ce2ac-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ce2ac-122">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2ac-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="ce2ac-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="ce2ac-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ce2ac-124">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2ac-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce2ac-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce2ac-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce2ac-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce2ac-126">Optional query parameters</span></span>
<span data-ttu-id="ce2ac-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce2ac-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce2ac-128">Request headers</span></span>
|<span data-ttu-id="ce2ac-129">标头</span><span class="sxs-lookup"><span data-stu-id="ce2ac-129">Header</span></span>|<span data-ttu-id="ce2ac-130">值</span><span class="sxs-lookup"><span data-stu-id="ce2ac-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce2ac-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2ac-131">Authorization</span></span>|<span data-ttu-id="ce2ac-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce2ac-133">接受</span><span class="sxs-lookup"><span data-stu-id="ce2ac-133">Accept</span></span>|<span data-ttu-id="ce2ac-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ce2ac-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce2ac-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce2ac-135">Request body</span></span>
<span data-ttu-id="ce2ac-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce2ac-137">响应</span><span class="sxs-lookup"><span data-stu-id="ce2ac-137">Response</span></span>
<span data-ttu-id="ce2ac-138">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-138">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce2ac-139">示例</span><span class="sxs-lookup"><span data-stu-id="ce2ac-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce2ac-140">请求</span><span class="sxs-lookup"><span data-stu-id="ce2ac-140">Request</span></span>
<span data-ttu-id="ce2ac-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="ce2ac-142">响应</span><span class="sxs-lookup"><span data-stu-id="ce2ac-142">Response</span></span>
<span data-ttu-id="ce2ac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce2ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







