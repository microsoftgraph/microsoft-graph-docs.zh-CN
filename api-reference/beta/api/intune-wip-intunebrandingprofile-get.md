---
title: 获取 intuneBrandingProfile
description: 读取 intuneBrandingProfile 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b8fc2a999f1dbf0b112d6b74e970b8e3491fe3b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970371"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="a1c13-103">获取 intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="a1c13-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="a1c13-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1c13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1c13-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1c13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1c13-106">读取[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1c13-106">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1c13-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1c13-107">Prerequisites</span></span>
<span data-ttu-id="a1c13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1c13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1c13-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1c13-110">Permission type</span></span>|<span data-ttu-id="a1c13-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1c13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1c13-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1c13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1c13-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1c13-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1c13-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1c13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1c13-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1c13-115">Not supported.</span></span>|
|<span data-ttu-id="a1c13-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1c13-116">Application</span></span>|<span data-ttu-id="a1c13-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1c13-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1c13-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1c13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1c13-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1c13-119">Optional query parameters</span></span>
<span data-ttu-id="a1c13-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1c13-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1c13-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1c13-121">Request headers</span></span>
|<span data-ttu-id="a1c13-122">标头</span><span class="sxs-lookup"><span data-stu-id="a1c13-122">Header</span></span>|<span data-ttu-id="a1c13-123">值</span><span class="sxs-lookup"><span data-stu-id="a1c13-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1c13-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1c13-124">Authorization</span></span>|<span data-ttu-id="a1c13-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1c13-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1c13-126">接受</span><span class="sxs-lookup"><span data-stu-id="a1c13-126">Accept</span></span>|<span data-ttu-id="a1c13-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1c13-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1c13-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1c13-128">Request body</span></span>
<span data-ttu-id="a1c13-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1c13-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1c13-130">响应</span><span class="sxs-lookup"><span data-stu-id="a1c13-130">Response</span></span>
<span data-ttu-id="a1c13-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a1c13-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1c13-132">示例</span><span class="sxs-lookup"><span data-stu-id="a1c13-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1c13-133">请求</span><span class="sxs-lookup"><span data-stu-id="a1c13-133">Request</span></span>
<span data-ttu-id="a1c13-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1c13-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="a1c13-135">响应</span><span class="sxs-lookup"><span data-stu-id="a1c13-135">Response</span></span>
<span data-ttu-id="a1c13-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1c13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




