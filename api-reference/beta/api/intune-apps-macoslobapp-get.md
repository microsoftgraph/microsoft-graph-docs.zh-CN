---
title: 获取 macOSLobApp
description: 读取属性和 macOSLobApp 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06b66861f475d20c1bf10ac4ebacee5781fb2b2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414716"
---
# <a name="get-macoslobapp"></a><span data-ttu-id="1bdd7-103">获取 macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="1bdd7-103">Get macOSLobApp</span></span>

> <span data-ttu-id="1bdd7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1bdd7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bdd7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bdd7-107">读取属性和[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-107">Read properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bdd7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bdd7-108">Prerequisites</span></span>
<span data-ttu-id="1bdd7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1bdd7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bdd7-111">Permission type</span></span>|<span data-ttu-id="1bdd7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bdd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdd7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bdd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdd7-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdd7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1bdd7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bdd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-116">Not supported.</span></span>|
|<span data-ttu-id="1bdd7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bdd7-117">Application</span></span>|<span data-ttu-id="1bdd7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdd7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bdd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bdd7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1bdd7-120">Optional query parameters</span></span>
<span data-ttu-id="1bdd7-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bdd7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bdd7-122">Request headers</span></span>
|<span data-ttu-id="1bdd7-123">标头</span><span class="sxs-lookup"><span data-stu-id="1bdd7-123">Header</span></span>|<span data-ttu-id="1bdd7-124">值</span><span class="sxs-lookup"><span data-stu-id="1bdd7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdd7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdd7-125">Authorization</span></span>|<span data-ttu-id="1bdd7-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdd7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1bdd7-127">Accept</span></span>|<span data-ttu-id="1bdd7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdd7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdd7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bdd7-129">Request body</span></span>
<span data-ttu-id="1bdd7-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bdd7-131">响应</span><span class="sxs-lookup"><span data-stu-id="1bdd7-131">Response</span></span>
<span data-ttu-id="1bdd7-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-132">If successful, this method returns a `200 OK` response code and [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdd7-133">示例</span><span class="sxs-lookup"><span data-stu-id="1bdd7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bdd7-134">请求</span><span class="sxs-lookup"><span data-stu-id="1bdd7-134">Request</span></span>
<span data-ttu-id="1bdd7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="1bdd7-136">响应</span><span class="sxs-lookup"><span data-stu-id="1bdd7-136">Response</span></span>
<span data-ttu-id="1bdd7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bdd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1846

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSLobApp",
    "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
      "v10_7": true,
      "v10_8": true,
      "v10_9": true,
      "v10_10": true,
      "v10_11": true,
      "v10_12": true,
      "v10_13": true
    },
    "buildNumber": "Build Number value",
    "versionNumber": "Version Number value",
    "childApps": [
      {
        "@odata.type": "microsoft.graph.macOSLobChildApp",
        "bundleId": "Bundle Id value",
        "buildNumber": "Build Number value",
        "versionNumber": "Version Number value"
      }
    ],
    "identityVersion": "Identity Version value",
    "md5HashChunkSize": 0,
    "md5Hash": [
      "Md5Hash value"
    ],
    "ignoreVersionDetection": true
  }
}
```




