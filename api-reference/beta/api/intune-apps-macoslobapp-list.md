---
title: 列出 macOSLobApps
description: 列出 macOSLobApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 174a93763e30aab4f22aed3161a4695628eaace7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330228"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="525b7-103">列出 macOSLobApps</span><span class="sxs-lookup"><span data-stu-id="525b7-103">List macOSLobApps</span></span>

> <span data-ttu-id="525b7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="525b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="525b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="525b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="525b7-106">列出[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="525b7-106">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="525b7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="525b7-107">Prerequisites</span></span>
<span data-ttu-id="525b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="525b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="525b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="525b7-110">Permission type</span></span>|<span data-ttu-id="525b7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="525b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="525b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="525b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="525b7-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="525b7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="525b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="525b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="525b7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="525b7-115">Not supported.</span></span>|
|<span data-ttu-id="525b7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="525b7-116">Application</span></span>|<span data-ttu-id="525b7-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="525b7-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="525b7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="525b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="525b7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="525b7-119">Request headers</span></span>
|<span data-ttu-id="525b7-120">标头</span><span class="sxs-lookup"><span data-stu-id="525b7-120">Header</span></span>|<span data-ttu-id="525b7-121">值</span><span class="sxs-lookup"><span data-stu-id="525b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="525b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="525b7-122">Authorization</span></span>|<span data-ttu-id="525b7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="525b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="525b7-124">接受</span><span class="sxs-lookup"><span data-stu-id="525b7-124">Accept</span></span>|<span data-ttu-id="525b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="525b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="525b7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="525b7-126">Request body</span></span>
<span data-ttu-id="525b7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="525b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="525b7-128">响应</span><span class="sxs-lookup"><span data-stu-id="525b7-128">Response</span></span>
<span data-ttu-id="525b7-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="525b7-129">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="525b7-130">示例</span><span class="sxs-lookup"><span data-stu-id="525b7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="525b7-131">请求</span><span class="sxs-lookup"><span data-stu-id="525b7-131">Request</span></span>
<span data-ttu-id="525b7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="525b7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="525b7-133">响应</span><span class="sxs-lookup"><span data-stu-id="525b7-133">Response</span></span>
<span data-ttu-id="525b7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="525b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1999

{
  "value": [
    {
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
      "dependentAppCount": 1,
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
  ]
}
```






