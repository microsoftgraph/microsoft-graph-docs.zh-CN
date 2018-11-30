---
title: 列表 intuneBrandingProfiles
description: 列出属性和 intuneBrandingProfile 对象之间的关系。
ms.openlocfilehash: 0c7fa1a191de73ea5042e319489633388b1f95df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047476"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="33683-103">列表 intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="33683-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="33683-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="33683-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33683-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="33683-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33683-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="33683-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33683-107">列出属性和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="33683-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33683-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="33683-108">Prerequisites</span></span>
<span data-ttu-id="33683-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="33683-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33683-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="33683-111">Permission type</span></span>|<span data-ttu-id="33683-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="33683-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33683-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33683-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33683-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="33683-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="33683-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33683-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33683-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="33683-116">Not supported.</span></span>|
|<span data-ttu-id="33683-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="33683-117">Application</span></span>|<span data-ttu-id="33683-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="33683-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33683-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33683-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="33683-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="33683-120">Request headers</span></span>
|<span data-ttu-id="33683-121">标头</span><span class="sxs-lookup"><span data-stu-id="33683-121">Header</span></span>|<span data-ttu-id="33683-122">值</span><span class="sxs-lookup"><span data-stu-id="33683-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33683-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33683-123">Authorization</span></span>|<span data-ttu-id="33683-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="33683-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33683-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33683-125">Accept</span></span>|<span data-ttu-id="33683-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33683-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33683-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="33683-127">Request body</span></span>
<span data-ttu-id="33683-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33683-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33683-129">响应</span><span class="sxs-lookup"><span data-stu-id="33683-129">Response</span></span>
<span data-ttu-id="33683-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="33683-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33683-131">示例</span><span class="sxs-lookup"><span data-stu-id="33683-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="33683-132">请求</span><span class="sxs-lookup"><span data-stu-id="33683-132">Request</span></span>
<span data-ttu-id="33683-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33683-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="33683-134">响应</span><span class="sxs-lookup"><span data-stu-id="33683-134">Response</span></span>
<span data-ttu-id="33683-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33683-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

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
      "contactITName": "Contact ITName value",
      "contactITPhoneNumber": "Contact ITPhone Number value",
      "contactITEmailAddress": "Contact ITEmail Address value",
      "contactITNotes": "Contact ITNotes value",
      "privacyUrl": "https://example.com/privacyUrl/",
      "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
      "onlineSupportSiteName": "Online Support Site Name value",
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
      }
    }
  ]
}
```





