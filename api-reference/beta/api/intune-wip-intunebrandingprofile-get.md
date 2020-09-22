---
title: 获取 intuneBrandingProfile
description: 读取 intuneBrandingProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a094e95e4502edf4de758a05c010fec69466fd0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062475"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="a79fa-103">获取 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="a79fa-103">Get intuneBrandingProfile</span></span>

<span data-ttu-id="a79fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a79fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a79fa-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a79fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a79fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a79fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a79fa-107">读取 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a79fa-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a79fa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a79fa-108">Prerequisites</span></span>
<span data-ttu-id="a79fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a79fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a79fa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a79fa-111">Permission type</span></span>|<span data-ttu-id="a79fa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a79fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a79fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a79fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a79fa-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a79fa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a79fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a79fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a79fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a79fa-116">Not supported.</span></span>|
|<span data-ttu-id="a79fa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a79fa-117">Application</span></span>|<span data-ttu-id="a79fa-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a79fa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a79fa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a79fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a79fa-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a79fa-120">Optional query parameters</span></span>
<span data-ttu-id="a79fa-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a79fa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a79fa-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a79fa-122">Request headers</span></span>
|<span data-ttu-id="a79fa-123">标头</span><span class="sxs-lookup"><span data-stu-id="a79fa-123">Header</span></span>|<span data-ttu-id="a79fa-124">值</span><span class="sxs-lookup"><span data-stu-id="a79fa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a79fa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a79fa-125">Authorization</span></span>|<span data-ttu-id="a79fa-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a79fa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a79fa-127">接受</span><span class="sxs-lookup"><span data-stu-id="a79fa-127">Accept</span></span>|<span data-ttu-id="a79fa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a79fa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a79fa-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a79fa-129">Request body</span></span>
<span data-ttu-id="a79fa-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a79fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a79fa-131">响应</span><span class="sxs-lookup"><span data-stu-id="a79fa-131">Response</span></span>
<span data-ttu-id="a79fa-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a79fa-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a79fa-133">示例</span><span class="sxs-lookup"><span data-stu-id="a79fa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a79fa-134">请求</span><span class="sxs-lookup"><span data-stu-id="a79fa-134">Request</span></span>
<span data-ttu-id="a79fa-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a79fa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="a79fa-136">响应</span><span class="sxs-lookup"><span data-stu-id="a79fa-136">Response</span></span>
<span data-ttu-id="a79fa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a79fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2284

{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfile",
    "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
    "profileName": "Profile Name value",
    "profileDescription": "Profile Description value",
    "isDefaultProfile": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "showDisplayNameNextToLogo": true,
    "themeColorLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "landingPageCustomizedImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "customPrivacyMessage": "Custom Privacy Message value",
    "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
    "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
    "isRemoveDeviceDisabled": true,
    "isFactoryResetDisabled": true,
    "companyPortalBlockedActions": [
      {
        "@odata.type": "microsoft.graph.companyPortalBlockedAction",
        "platform": "androidForWork",
        "ownerType": "company",
        "action": "remove"
      }
    ],
    "showAzureADEnterpriseApps": true,
    "showOfficeWebApps": true,
    "sendDeviceOwnershipChangePushNotification": true,
    "enrollmentAvailability": "availableWithoutPrompts",
    "disableClientTelemetry": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






