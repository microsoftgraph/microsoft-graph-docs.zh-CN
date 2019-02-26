---
title: 获取 depEnrollmentBaseProfile
description: 读取 depEnrollmentBaseProfile 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9be0c8db30e5df525d565b7ad9433611c9e6a0a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168129"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="0b8cf-103">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="0b8cf-103">Get depEnrollmentBaseProfile</span></span>

> <span data-ttu-id="0b8cf-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b8cf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b8cf-106">读取[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-106">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b8cf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b8cf-107">Prerequisites</span></span>
<span data-ttu-id="0b8cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b8cf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b8cf-110">Permission type</span></span>|<span data-ttu-id="0b8cf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b8cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b8cf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b8cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b8cf-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b8cf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0b8cf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b8cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b8cf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-115">Not supported.</span></span>|
|<span data-ttu-id="0b8cf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b8cf-116">Application</span></span>|<span data-ttu-id="0b8cf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b8cf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b8cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b8cf-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b8cf-119">Optional query parameters</span></span>
<span data-ttu-id="0b8cf-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b8cf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b8cf-121">Request headers</span></span>
|<span data-ttu-id="0b8cf-122">标头</span><span class="sxs-lookup"><span data-stu-id="0b8cf-122">Header</span></span>|<span data-ttu-id="0b8cf-123">值</span><span class="sxs-lookup"><span data-stu-id="0b8cf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b8cf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b8cf-124">Authorization</span></span>|<span data-ttu-id="0b8cf-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b8cf-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0b8cf-126">Accept</span></span>|<span data-ttu-id="0b8cf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0b8cf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b8cf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b8cf-128">Request body</span></span>
<span data-ttu-id="0b8cf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b8cf-130">响应</span><span class="sxs-lookup"><span data-stu-id="0b8cf-130">Response</span></span>
<span data-ttu-id="0b8cf-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-131">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b8cf-132">示例</span><span class="sxs-lookup"><span data-stu-id="0b8cf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b8cf-133">请求</span><span class="sxs-lookup"><span data-stu-id="0b8cf-133">Request</span></span>
<span data-ttu-id="0b8cf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="0b8cf-135">响应</span><span class="sxs-lookup"><span data-stu-id="0b8cf-135">Response</span></span>
<span data-ttu-id="0b8cf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b8cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1079

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
    "id": "db378868-8868-db37-6888-37db688837db",
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
    "privacyPaneDisabled": true
  }
}
```




