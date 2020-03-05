---
title: 列出 depEnrollmentBaseProfiles
description: 列出 depEnrollmentBaseProfile 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05541f36bb289139aa52a5af1c5182e484db7dc1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467310"
---
# <a name="list-depenrollmentbaseprofiles"></a><span data-ttu-id="6f843-103">列出 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="6f843-103">List depEnrollmentBaseProfiles</span></span>

<span data-ttu-id="6f843-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6f843-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f843-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f843-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f843-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f843-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f843-107">列出[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f843-107">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f843-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f843-108">Prerequisites</span></span>
<span data-ttu-id="6f843-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f843-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f843-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f843-111">Permission type</span></span>|<span data-ttu-id="6f843-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f843-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f843-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f843-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f843-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f843-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6f843-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f843-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f843-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f843-116">Not supported.</span></span>|
|<span data-ttu-id="6f843-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f843-117">Application</span></span>|<span data-ttu-id="6f843-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f843-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f843-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f843-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6f843-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f843-120">Request headers</span></span>
|<span data-ttu-id="6f843-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f843-121">Header</span></span>|<span data-ttu-id="6f843-122">值</span><span class="sxs-lookup"><span data-stu-id="6f843-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f843-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f843-123">Authorization</span></span>|<span data-ttu-id="6f843-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f843-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f843-125">接受</span><span class="sxs-lookup"><span data-stu-id="6f843-125">Accept</span></span>|<span data-ttu-id="6f843-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f843-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f843-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f843-127">Request body</span></span>
<span data-ttu-id="6f843-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f843-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f843-129">响应</span><span class="sxs-lookup"><span data-stu-id="6f843-129">Response</span></span>
<span data-ttu-id="6f843-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6f843-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f843-131">示例</span><span class="sxs-lookup"><span data-stu-id="6f843-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f843-132">请求</span><span class="sxs-lookup"><span data-stu-id="6f843-132">Request</span></span>
<span data-ttu-id="6f843-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f843-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="6f843-134">响应</span><span class="sxs-lookup"><span data-stu-id="6f843-134">Response</span></span>
<span data-ttu-id="6f843-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f843-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1281

{
  "value": [
    {
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
      "privacyPaneDisabled": true,
      "screenTimeScreenDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "configurationWebUrl": true
    }
  ]
}
```





