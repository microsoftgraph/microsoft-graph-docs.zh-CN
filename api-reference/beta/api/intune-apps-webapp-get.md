---
title: 获取 webApp
description: 读取 webApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67fb2430c053ed70c1cef7a1ef1e9b3a568f8d63
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328842"
---
# <a name="get-webapp"></a><span data-ttu-id="86aac-103">获取 webApp</span><span class="sxs-lookup"><span data-stu-id="86aac-103">Get webApp</span></span>

> <span data-ttu-id="86aac-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86aac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86aac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86aac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86aac-106">读取 [webApp](../resources/intune-apps-webapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86aac-106">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86aac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="86aac-107">Prerequisites</span></span>
<span data-ttu-id="86aac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86aac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86aac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86aac-110">Permission type</span></span>|<span data-ttu-id="86aac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86aac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86aac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86aac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86aac-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86aac-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86aac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86aac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86aac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86aac-115">Not supported.</span></span>|
|<span data-ttu-id="86aac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86aac-116">Application</span></span>|<span data-ttu-id="86aac-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86aac-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86aac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86aac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86aac-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86aac-119">Optional query parameters</span></span>
<span data-ttu-id="86aac-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86aac-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86aac-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="86aac-121">Request headers</span></span>
|<span data-ttu-id="86aac-122">标头</span><span class="sxs-lookup"><span data-stu-id="86aac-122">Header</span></span>|<span data-ttu-id="86aac-123">值</span><span class="sxs-lookup"><span data-stu-id="86aac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86aac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="86aac-124">Authorization</span></span>|<span data-ttu-id="86aac-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86aac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86aac-126">接受</span><span class="sxs-lookup"><span data-stu-id="86aac-126">Accept</span></span>|<span data-ttu-id="86aac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="86aac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86aac-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="86aac-128">Request body</span></span>
<span data-ttu-id="86aac-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86aac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86aac-130">响应</span><span class="sxs-lookup"><span data-stu-id="86aac-130">Response</span></span>
<span data-ttu-id="86aac-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [webApp](../resources/intune-apps-webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86aac-131">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86aac-132">示例</span><span class="sxs-lookup"><span data-stu-id="86aac-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="86aac-133">请求</span><span class="sxs-lookup"><span data-stu-id="86aac-133">Request</span></span>
<span data-ttu-id="86aac-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86aac-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="86aac-135">响应</span><span class="sxs-lookup"><span data-stu-id="86aac-135">Response</span></span>
<span data-ttu-id="86aac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86aac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1024

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```






