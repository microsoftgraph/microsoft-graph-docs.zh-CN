---
title: 获取 androidManagedStoreApp
description: 读取 androidManagedStoreApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcc04d92a817aceeb18c0d1125a6bd39e63b7e3b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952245"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="92e3b-103">获取 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="92e3b-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="92e3b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92e3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e3b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92e3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e3b-106">读取[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92e3b-106">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e3b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="92e3b-107">Prerequisites</span></span>
<span data-ttu-id="92e3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92e3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="92e3b-110">Permission type</span></span>|<span data-ttu-id="92e3b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92e3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92e3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92e3b-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92e3b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="92e3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92e3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e3b-115">Not supported.</span></span>|
|<span data-ttu-id="92e3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92e3b-116">Application</span></span>|<span data-ttu-id="92e3b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92e3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92e3b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92e3b-119">Optional query parameters</span></span>
<span data-ttu-id="92e3b-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92e3b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92e3b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="92e3b-121">Request headers</span></span>
|<span data-ttu-id="92e3b-122">标头</span><span class="sxs-lookup"><span data-stu-id="92e3b-122">Header</span></span>|<span data-ttu-id="92e3b-123">值</span><span class="sxs-lookup"><span data-stu-id="92e3b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e3b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="92e3b-124">Authorization</span></span>|<span data-ttu-id="92e3b-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92e3b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e3b-126">接受</span><span class="sxs-lookup"><span data-stu-id="92e3b-126">Accept</span></span>|<span data-ttu-id="92e3b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="92e3b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e3b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="92e3b-128">Request body</span></span>
<span data-ttu-id="92e3b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92e3b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92e3b-130">响应</span><span class="sxs-lookup"><span data-stu-id="92e3b-130">Response</span></span>
<span data-ttu-id="92e3b-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="92e3b-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e3b-132">示例</span><span class="sxs-lookup"><span data-stu-id="92e3b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e3b-133">请求</span><span class="sxs-lookup"><span data-stu-id="92e3b-133">Request</span></span>
<span data-ttu-id="92e3b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92e3b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="92e3b-135">响应</span><span class="sxs-lookup"><span data-stu-id="92e3b-135">Response</span></span>
<span data-ttu-id="92e3b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92e3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1191

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreApp",
    "id": "87247525-7525-8724-2575-248725752487",
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
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "supportsOemConfig": true
  }
}
```





