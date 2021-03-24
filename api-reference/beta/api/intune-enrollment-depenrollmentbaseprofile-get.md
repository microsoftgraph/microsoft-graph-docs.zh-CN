---
title: 获取 depEnrollmentBaseProfile
description: 读取 depEnrollmentBaseProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee7a2c421c0e94bb336669829505567a5a242cfd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149924"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="8eb59-103">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="8eb59-103">Get depEnrollmentBaseProfile</span></span>

<span data-ttu-id="8eb59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eb59-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8eb59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eb59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8eb59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb59-107">读取 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8eb59-107">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eb59-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8eb59-108">Prerequisites</span></span>
<span data-ttu-id="8eb59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb59-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8eb59-111">Permission type</span></span>|<span data-ttu-id="8eb59-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8eb59-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eb59-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8eb59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8eb59-114">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb59-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8eb59-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8eb59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eb59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eb59-116">Not supported.</span></span>|
|<span data-ttu-id="8eb59-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8eb59-117">Application</span></span>|<span data-ttu-id="8eb59-118">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb59-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eb59-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eb59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8eb59-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8eb59-120">Optional query parameters</span></span>
<span data-ttu-id="8eb59-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8eb59-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8eb59-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eb59-122">Request headers</span></span>
|<span data-ttu-id="8eb59-123">标头</span><span class="sxs-lookup"><span data-stu-id="8eb59-123">Header</span></span>|<span data-ttu-id="8eb59-124">值</span><span class="sxs-lookup"><span data-stu-id="8eb59-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eb59-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eb59-125">Authorization</span></span>|<span data-ttu-id="8eb59-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8eb59-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eb59-127">接受</span><span class="sxs-lookup"><span data-stu-id="8eb59-127">Accept</span></span>|<span data-ttu-id="8eb59-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8eb59-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eb59-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8eb59-129">Request body</span></span>
<span data-ttu-id="8eb59-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8eb59-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eb59-131">响应</span><span class="sxs-lookup"><span data-stu-id="8eb59-131">Response</span></span>
<span data-ttu-id="8eb59-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8eb59-132">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb59-133">示例</span><span class="sxs-lookup"><span data-stu-id="8eb59-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eb59-134">请求</span><span class="sxs-lookup"><span data-stu-id="8eb59-134">Request</span></span>
<span data-ttu-id="8eb59-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8eb59-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="8eb59-136">响应</span><span class="sxs-lookup"><span data-stu-id="8eb59-136">Response</span></span>
<span data-ttu-id="8eb59-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8eb59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1151

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
    "isMandatory": true,
    "locationDisabled": true,
    "supportPhoneNumber": "Support Phone Number value",
    "profileRemovalDisabled": true,
    "restoreBlocked": true,
    "appleIdDisabled": true,
    "termsAndConditionsDisabled": true,
    "touchIdDisabled": true,
    "applePayDisabled": true,
    "siriDisabled": true,
    "diagnosticsDisabled": true,
    "displayToneSetupDisabled": true,
    "privacyPaneDisabled": true,
    "screenTimeScreenDisabled": true,
    "deviceNameTemplate": "Device Name Template value",
    "configurationWebUrl": true
  }
}
```




