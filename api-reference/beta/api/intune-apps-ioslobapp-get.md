---
title: 获取 iosLobApp
description: 读取 iosLobApp 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0de46d89b0848dcf91c9031f8d35e1954fed2cd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962083"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="36a33-103">获取 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="36a33-103">Get iosLobApp</span></span>

> <span data-ttu-id="36a33-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36a33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a33-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36a33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a33-106">读取 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36a33-106">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36a33-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="36a33-107">Prerequisites</span></span>
<span data-ttu-id="36a33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36a33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36a33-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36a33-110">Permission type</span></span>|<span data-ttu-id="36a33-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36a33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36a33-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36a33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36a33-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="36a33-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="36a33-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36a33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36a33-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36a33-115">Not supported.</span></span>|
|<span data-ttu-id="36a33-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36a33-116">Application</span></span>|<span data-ttu-id="36a33-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="36a33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36a33-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36a33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36a33-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36a33-119">Optional query parameters</span></span>
<span data-ttu-id="36a33-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36a33-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36a33-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="36a33-121">Request headers</span></span>
|<span data-ttu-id="36a33-122">标头</span><span class="sxs-lookup"><span data-stu-id="36a33-122">Header</span></span>|<span data-ttu-id="36a33-123">值</span><span class="sxs-lookup"><span data-stu-id="36a33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36a33-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36a33-124">Authorization</span></span>|<span data-ttu-id="36a33-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36a33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36a33-126">接受</span><span class="sxs-lookup"><span data-stu-id="36a33-126">Accept</span></span>|<span data-ttu-id="36a33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="36a33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36a33-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="36a33-128">Request body</span></span>
<span data-ttu-id="36a33-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36a33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36a33-130">响应</span><span class="sxs-lookup"><span data-stu-id="36a33-130">Response</span></span>
<span data-ttu-id="36a33-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36a33-131">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36a33-132">示例</span><span class="sxs-lookup"><span data-stu-id="36a33-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="36a33-133">请求</span><span class="sxs-lookup"><span data-stu-id="36a33-133">Request</span></span>
<span data-ttu-id="36a33-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36a33-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="36a33-135">响应</span><span class="sxs-lookup"><span data-stu-id="36a33-135">Response</span></span>
<span data-ttu-id="36a33-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36a33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1645

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobApp",
    "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```




