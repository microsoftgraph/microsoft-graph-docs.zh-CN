---
title: 列出 intuneBrandingProfiles
description: 列出 intuneBrandingProfile 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bc7add6e2c5add524419961636300e903a64d6d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938479"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="a6ef7-103">列出 intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="a6ef7-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="a6ef7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6ef7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ef7-106">列出[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-106">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6ef7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6ef7-107">Prerequisites</span></span>
<span data-ttu-id="a6ef7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6ef7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6ef7-110">Permission type</span></span>|<span data-ttu-id="a6ef7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6ef7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6ef7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6ef7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6ef7-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ef7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6ef7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6ef7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6ef7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-115">Not supported.</span></span>|
|<span data-ttu-id="a6ef7-116">Application</span><span class="sxs-lookup"><span data-stu-id="a6ef7-116">Application</span></span>|<span data-ttu-id="a6ef7-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ef7-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6ef7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6ef7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a6ef7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6ef7-119">Request headers</span></span>
|<span data-ttu-id="a6ef7-120">标头</span><span class="sxs-lookup"><span data-stu-id="a6ef7-120">Header</span></span>|<span data-ttu-id="a6ef7-121">值</span><span class="sxs-lookup"><span data-stu-id="a6ef7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6ef7-122">授权</span><span class="sxs-lookup"><span data-stu-id="a6ef7-122">Authorization</span></span>|<span data-ttu-id="a6ef7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6ef7-124">接受</span><span class="sxs-lookup"><span data-stu-id="a6ef7-124">Accept</span></span>|<span data-ttu-id="a6ef7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6ef7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6ef7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6ef7-126">Request body</span></span>
<span data-ttu-id="a6ef7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6ef7-128">响应</span><span class="sxs-lookup"><span data-stu-id="a6ef7-128">Response</span></span>
<span data-ttu-id="a6ef7-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6ef7-130">示例</span><span class="sxs-lookup"><span data-stu-id="a6ef7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6ef7-131">请求</span><span class="sxs-lookup"><span data-stu-id="a6ef7-131">Request</span></span>
<span data-ttu-id="a6ef7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="a6ef7-133">响应</span><span class="sxs-lookup"><span data-stu-id="a6ef7-133">Response</span></span>
<span data-ttu-id="a6ef7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6ef7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "value": [
    {
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
      "showOfficeWebApps": true
    }
  ]
}
```





