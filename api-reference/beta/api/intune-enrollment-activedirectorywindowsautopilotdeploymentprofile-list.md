---
title: 列出 activeDirectoryWindowsAutopilotDeploymentProfiles
description: 列出 activeDirectoryWindowsAutopilotDeploymentProfile 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 192a1b3dbcad17415f260670075f5970632687fb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790037"
---
# <a name="list-activedirectorywindowsautopilotdeploymentprofiles"></a><span data-ttu-id="d49de-103">列出 activeDirectoryWindowsAutopilotDeploymentProfiles</span><span class="sxs-lookup"><span data-stu-id="d49de-103">List activeDirectoryWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="d49de-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d49de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d49de-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d49de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d49de-106">列出[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d49de-106">List properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d49de-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d49de-107">Prerequisites</span></span>
<span data-ttu-id="d49de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d49de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d49de-110">Permission type</span></span>|<span data-ttu-id="d49de-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d49de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d49de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d49de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d49de-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d49de-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d49de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d49de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d49de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d49de-115">Not supported.</span></span>|
|<span data-ttu-id="d49de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d49de-116">Application</span></span>|<span data-ttu-id="d49de-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d49de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d49de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d49de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d49de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d49de-119">Request headers</span></span>
|<span data-ttu-id="d49de-120">标头</span><span class="sxs-lookup"><span data-stu-id="d49de-120">Header</span></span>|<span data-ttu-id="d49de-121">值</span><span class="sxs-lookup"><span data-stu-id="d49de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d49de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d49de-122">Authorization</span></span>|<span data-ttu-id="d49de-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d49de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d49de-124">接受</span><span class="sxs-lookup"><span data-stu-id="d49de-124">Accept</span></span>|<span data-ttu-id="d49de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d49de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d49de-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d49de-126">Request body</span></span>
<span data-ttu-id="d49de-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d49de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d49de-128">响应</span><span class="sxs-lookup"><span data-stu-id="d49de-128">Response</span></span>
<span data-ttu-id="d49de-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d49de-129">If successful, this method returns a `200 OK` response code and a collection of [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d49de-130">示例</span><span class="sxs-lookup"><span data-stu-id="d49de-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d49de-131">请求</span><span class="sxs-lookup"><span data-stu-id="d49de-131">Request</span></span>
<span data-ttu-id="d49de-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d49de-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="d49de-133">响应</span><span class="sxs-lookup"><span data-stu-id="d49de-133">Response</span></span>
<span data-ttu-id="d49de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d49de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1430

{
  "value": [
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
  ]
}
```





