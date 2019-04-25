---
title: 列出 depIOSEnrollmentProfiles
description: 列出 depIOSEnrollmentProfile 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9176cfeaebc5e219ea64d68ecf82767877d2f8d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534050"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="83e62-103">列出 depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="83e62-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="83e62-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83e62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83e62-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83e62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83e62-106">列出[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83e62-106">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83e62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="83e62-107">Prerequisites</span></span>
<span data-ttu-id="83e62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="83e62-110">Permission type</span></span>|<span data-ttu-id="83e62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83e62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83e62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83e62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83e62-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83e62-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="83e62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83e62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83e62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="83e62-115">Not supported.</span></span>|
|<span data-ttu-id="83e62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="83e62-116">Application</span></span>|<span data-ttu-id="83e62-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="83e62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83e62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83e62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="83e62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="83e62-119">Request headers</span></span>
|<span data-ttu-id="83e62-120">标头</span><span class="sxs-lookup"><span data-stu-id="83e62-120">Header</span></span>|<span data-ttu-id="83e62-121">值</span><span class="sxs-lookup"><span data-stu-id="83e62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83e62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e62-122">Authorization</span></span>|<span data-ttu-id="83e62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83e62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83e62-124">接受</span><span class="sxs-lookup"><span data-stu-id="83e62-124">Accept</span></span>|<span data-ttu-id="83e62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83e62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83e62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="83e62-126">Request body</span></span>
<span data-ttu-id="83e62-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83e62-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e62-128">响应</span><span class="sxs-lookup"><span data-stu-id="83e62-128">Response</span></span>
<span data-ttu-id="83e62-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="83e62-129">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83e62-130">示例</span><span class="sxs-lookup"><span data-stu-id="83e62-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="83e62-131">请求</span><span class="sxs-lookup"><span data-stu-id="83e62-131">Request</span></span>
<span data-ttu-id="83e62-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83e62-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="83e62-133">响应</span><span class="sxs-lookup"><span data-stu-id="83e62-133">Response</span></span>
<span data-ttu-id="83e62-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83e62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
      "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
      "deviceNameTemplate": "Device Name Template value",
      "iTunesPairingMode": "allow",
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreFromAndroidDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true,
      "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
      "enableSingleAppEnrollmentMode": true,
      "homeButtonScreenDisabled": true,
      "iMessageAndFaceTimeScreenDisabled": true,
      "onBoardingScreenDisabled": true,
      "screenTimeScreenDisabled": true,
      "simSetupScreenDisabled": true,
      "softwareUpdateScreenDisabled": true,
      "watchMigrationScreenDisabled": true
    }
  ]
}
```





