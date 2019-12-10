---
title: 获取 androidStoreApp
description: 读取 androidStoreApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9617bf288fc353bdb06127b8e7454fa06c15984d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921863"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="13556-103">获取 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="13556-103">Get androidStoreApp</span></span>

> <span data-ttu-id="13556-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13556-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13556-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13556-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13556-106">读取 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13556-106">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13556-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="13556-107">Prerequisites</span></span>
<span data-ttu-id="13556-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13556-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="13556-110">Permission type</span></span>|<span data-ttu-id="13556-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="13556-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13556-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13556-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13556-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13556-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="13556-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13556-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13556-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13556-115">Not supported.</span></span>|
|<span data-ttu-id="13556-116">Application</span><span class="sxs-lookup"><span data-stu-id="13556-116">Application</span></span>|<span data-ttu-id="13556-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13556-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13556-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13556-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13556-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13556-119">Optional query parameters</span></span>
<span data-ttu-id="13556-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13556-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13556-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="13556-121">Request headers</span></span>
|<span data-ttu-id="13556-122">标头</span><span class="sxs-lookup"><span data-stu-id="13556-122">Header</span></span>|<span data-ttu-id="13556-123">值</span><span class="sxs-lookup"><span data-stu-id="13556-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13556-124">授权</span><span class="sxs-lookup"><span data-stu-id="13556-124">Authorization</span></span>|<span data-ttu-id="13556-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13556-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13556-126">接受</span><span class="sxs-lookup"><span data-stu-id="13556-126">Accept</span></span>|<span data-ttu-id="13556-127">application/json</span><span class="sxs-lookup"><span data-stu-id="13556-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13556-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="13556-128">Request body</span></span>
<span data-ttu-id="13556-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13556-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13556-130">响应</span><span class="sxs-lookup"><span data-stu-id="13556-130">Response</span></span>
<span data-ttu-id="13556-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13556-131">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13556-132">示例</span><span class="sxs-lookup"><span data-stu-id="13556-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="13556-133">请求</span><span class="sxs-lookup"><span data-stu-id="13556-133">Request</span></span>
<span data-ttu-id="13556-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13556-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="13556-135">响应</span><span class="sxs-lookup"><span data-stu-id="13556-135">Response</span></span>
<span data-ttu-id="13556-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13556-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1511

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    }
  }
}
```





