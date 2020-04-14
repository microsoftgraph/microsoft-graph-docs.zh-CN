---
title: 列出 depMacOSEnrollmentProfiles
description: 列出 depMacOSEnrollmentProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c347220d6290405681c41519a14e35e58e05e4ba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443490"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="3e71d-103">列出 depMacOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="3e71d-103">List depMacOSEnrollmentProfiles</span></span>

<span data-ttu-id="3e71d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e71d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e71d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e71d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e71d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e71d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e71d-107">列出[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e71d-107">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e71d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3e71d-108">Prerequisites</span></span>
<span data-ttu-id="3e71d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e71d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e71d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e71d-111">Permission type</span></span>|<span data-ttu-id="3e71d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3e71d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e71d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e71d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e71d-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e71d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3e71d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e71d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e71d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e71d-116">Not supported.</span></span>|
|<span data-ttu-id="3e71d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e71d-117">Application</span></span>|<span data-ttu-id="3e71d-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e71d-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e71d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e71d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3e71d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e71d-120">Request headers</span></span>
|<span data-ttu-id="3e71d-121">标头</span><span class="sxs-lookup"><span data-stu-id="3e71d-121">Header</span></span>|<span data-ttu-id="3e71d-122">值</span><span class="sxs-lookup"><span data-stu-id="3e71d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e71d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e71d-123">Authorization</span></span>|<span data-ttu-id="3e71d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3e71d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e71d-125">接受</span><span class="sxs-lookup"><span data-stu-id="3e71d-125">Accept</span></span>|<span data-ttu-id="3e71d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e71d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e71d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e71d-127">Request body</span></span>
<span data-ttu-id="3e71d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e71d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e71d-129">响应</span><span class="sxs-lookup"><span data-stu-id="3e71d-129">Response</span></span>
<span data-ttu-id="3e71d-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3e71d-130">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e71d-131">示例</span><span class="sxs-lookup"><span data-stu-id="3e71d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e71d-132">请求</span><span class="sxs-lookup"><span data-stu-id="3e71d-132">Request</span></span>
<span data-ttu-id="3e71d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e71d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="3e71d-134">响应</span><span class="sxs-lookup"><span data-stu-id="3e71d-134">Response</span></span>
<span data-ttu-id="3e71d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e71d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1478

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "displayToneSetupDisabled": true,
      "privacyPaneDisabled": true,
      "screenTimeScreenDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "configurationWebUrl": true,
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true,
      "iCloudStorageDisabled": true,
      "chooseYourLockScreenDisabled": true
    }
  ]
}
```



