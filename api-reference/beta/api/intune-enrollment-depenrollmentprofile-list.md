---
title: 列出 depEnrollmentProfiles
description: 列出 depEnrollmentProfile 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 762cbf6790c09010e27a8f7f95c3ba748e4d93f6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187931"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="c70ce-103">列出 depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="c70ce-103">List depEnrollmentProfiles</span></span>

> <span data-ttu-id="c70ce-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c70ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c70ce-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c70ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c70ce-106">列出[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c70ce-106">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c70ce-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c70ce-107">Prerequisites</span></span>
<span data-ttu-id="c70ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c70ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c70ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c70ce-110">Permission type</span></span>|<span data-ttu-id="c70ce-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c70ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c70ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c70ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c70ce-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c70ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c70ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c70ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c70ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c70ce-115">Not supported.</span></span>|
|<span data-ttu-id="c70ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c70ce-116">Application</span></span>|<span data-ttu-id="c70ce-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c70ce-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c70ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c70ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c70ce-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c70ce-119">Request headers</span></span>
|<span data-ttu-id="c70ce-120">标头</span><span class="sxs-lookup"><span data-stu-id="c70ce-120">Header</span></span>|<span data-ttu-id="c70ce-121">值</span><span class="sxs-lookup"><span data-stu-id="c70ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c70ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c70ce-122">Authorization</span></span>|<span data-ttu-id="c70ce-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c70ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c70ce-124">接受</span><span class="sxs-lookup"><span data-stu-id="c70ce-124">Accept</span></span>|<span data-ttu-id="c70ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c70ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c70ce-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c70ce-126">Request body</span></span>
<span data-ttu-id="c70ce-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c70ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c70ce-128">响应</span><span class="sxs-lookup"><span data-stu-id="c70ce-128">Response</span></span>
<span data-ttu-id="c70ce-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c70ce-129">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c70ce-130">示例</span><span class="sxs-lookup"><span data-stu-id="c70ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c70ce-131">请求</span><span class="sxs-lookup"><span data-stu-id="c70ce-131">Request</span></span>
<span data-ttu-id="c70ce-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c70ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="c70ce-133">响应</span><span class="sxs-lookup"><span data-stu-id="c70ce-133">Response</span></span>
<span data-ttu-id="c70ce-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c70ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1588

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depEnrollmentProfile",
      "id": "3d4534f7-34f7-3d45-f734-453df734453d",
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
      "iTunesPairingMode": "allow",
      "profileRemovalDisabled": true,
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreBlocked": true,
      "restoreFromAndroidDisabled": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "macOSRegistrationDisabled": true,
      "macOSFileVaultDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true
    }
  ]
}
```




