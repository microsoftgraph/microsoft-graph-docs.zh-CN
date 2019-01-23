---
title: 获取 intuneBrandingProfile
description: 读取属性和 intuneBrandingProfile 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5efcfcabcb84dae77e91d7d3c765b18c9d95783c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402998"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="d67f6-103">获取 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="d67f6-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="d67f6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d67f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d67f6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d67f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d67f6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d67f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d67f6-107">读取属性和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d67f6-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d67f6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d67f6-108">Prerequisites</span></span>
<span data-ttu-id="d67f6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d67f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d67f6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d67f6-111">Permission type</span></span>|<span data-ttu-id="d67f6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d67f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d67f6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d67f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d67f6-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d67f6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d67f6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d67f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d67f6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d67f6-116">Not supported.</span></span>|
|<span data-ttu-id="d67f6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d67f6-117">Application</span></span>|<span data-ttu-id="d67f6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d67f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d67f6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d67f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d67f6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d67f6-120">Optional query parameters</span></span>
<span data-ttu-id="d67f6-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d67f6-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d67f6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d67f6-122">Request headers</span></span>
|<span data-ttu-id="d67f6-123">标头</span><span class="sxs-lookup"><span data-stu-id="d67f6-123">Header</span></span>|<span data-ttu-id="d67f6-124">值</span><span class="sxs-lookup"><span data-stu-id="d67f6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d67f6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d67f6-125">Authorization</span></span>|<span data-ttu-id="d67f6-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d67f6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d67f6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d67f6-127">Accept</span></span>|<span data-ttu-id="d67f6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d67f6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d67f6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d67f6-129">Request body</span></span>
<span data-ttu-id="d67f6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d67f6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d67f6-131">响应</span><span class="sxs-lookup"><span data-stu-id="d67f6-131">Response</span></span>
<span data-ttu-id="d67f6-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d67f6-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d67f6-133">示例</span><span class="sxs-lookup"><span data-stu-id="d67f6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d67f6-134">请求</span><span class="sxs-lookup"><span data-stu-id="d67f6-134">Request</span></span>
<span data-ttu-id="d67f6-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d67f6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="d67f6-136">响应</span><span class="sxs-lookup"><span data-stu-id="d67f6-136">Response</span></span>
<span data-ttu-id="d67f6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d67f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1472

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
}
```




