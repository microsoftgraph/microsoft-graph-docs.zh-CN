---
title: 获取 depMacOSEnrollmentProfile
description: 读取属性和 depMacOSEnrollmentProfile 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 864c5680ee48e06ec7c32b66ee5a456a77dbecde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416004"
---
# <a name="get-depmacosenrollmentprofile"></a><span data-ttu-id="12238-103">获取 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="12238-103">Get depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="12238-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="12238-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12238-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12238-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12238-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12238-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12238-107">读取属性和[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="12238-107">Read properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12238-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12238-108">Prerequisites</span></span>
<span data-ttu-id="12238-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="12238-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="12238-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12238-111">Permission type</span></span>|<span data-ttu-id="12238-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12238-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12238-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12238-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12238-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="12238-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="12238-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12238-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12238-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12238-116">Not supported.</span></span>|
|<span data-ttu-id="12238-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12238-117">Application</span></span>|<span data-ttu-id="12238-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="12238-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12238-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12238-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12238-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="12238-120">Optional query parameters</span></span>
<span data-ttu-id="12238-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="12238-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12238-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="12238-122">Request headers</span></span>
|<span data-ttu-id="12238-123">标头</span><span class="sxs-lookup"><span data-stu-id="12238-123">Header</span></span>|<span data-ttu-id="12238-124">值</span><span class="sxs-lookup"><span data-stu-id="12238-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12238-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="12238-125">Authorization</span></span>|<span data-ttu-id="12238-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12238-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12238-127">Accept</span><span class="sxs-lookup"><span data-stu-id="12238-127">Accept</span></span>|<span data-ttu-id="12238-128">application/json</span><span class="sxs-lookup"><span data-stu-id="12238-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12238-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="12238-129">Request body</span></span>
<span data-ttu-id="12238-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12238-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12238-131">响应</span><span class="sxs-lookup"><span data-stu-id="12238-131">Response</span></span>
<span data-ttu-id="12238-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12238-132">If successful, this method returns a `200 OK` response code and [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12238-133">示例</span><span class="sxs-lookup"><span data-stu-id="12238-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="12238-134">请求</span><span class="sxs-lookup"><span data-stu-id="12238-134">Request</span></span>
<span data-ttu-id="12238-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12238-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="12238-136">响应</span><span class="sxs-lookup"><span data-stu-id="12238-136">Response</span></span>
<span data-ttu-id="12238-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12238-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1187

{
  "value": {
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
    "registrationDisabled": true,
    "fileVaultDisabled": true,
    "iCloudDiagnosticsDisabled": true
  }
}
```




