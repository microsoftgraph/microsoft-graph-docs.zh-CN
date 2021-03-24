---
title: 获取 windowsMobileMSI
description: 读取 windowsMobileMSI 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62369bf142ac9b3831f5a49122667357faa37bd0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138896"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="bbc63-103">获取 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="bbc63-103">Get windowsMobileMSI</span></span>

<span data-ttu-id="bbc63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbc63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbc63-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bbc63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbc63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bbc63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbc63-107">读取 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bbc63-107">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbc63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbc63-108">Prerequisites</span></span>
<span data-ttu-id="bbc63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbc63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbc63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbc63-111">Permission type</span></span>|<span data-ttu-id="bbc63-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbc63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbc63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbc63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbc63-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc63-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bbc63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbc63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbc63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbc63-116">Not supported.</span></span>|
|<span data-ttu-id="bbc63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbc63-117">Application</span></span>|<span data-ttu-id="bbc63-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc63-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbc63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbc63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbc63-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bbc63-120">Optional query parameters</span></span>
<span data-ttu-id="bbc63-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bbc63-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbc63-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbc63-122">Request headers</span></span>
|<span data-ttu-id="bbc63-123">标头</span><span class="sxs-lookup"><span data-stu-id="bbc63-123">Header</span></span>|<span data-ttu-id="bbc63-124">值</span><span class="sxs-lookup"><span data-stu-id="bbc63-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbc63-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbc63-125">Authorization</span></span>|<span data-ttu-id="bbc63-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbc63-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbc63-127">接受</span><span class="sxs-lookup"><span data-stu-id="bbc63-127">Accept</span></span>|<span data-ttu-id="bbc63-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bbc63-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbc63-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbc63-129">Request body</span></span>
<span data-ttu-id="bbc63-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbc63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbc63-131">响应</span><span class="sxs-lookup"><span data-stu-id="bbc63-131">Response</span></span>
<span data-ttu-id="bbc63-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbc63-132">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc63-133">示例</span><span class="sxs-lookup"><span data-stu-id="bbc63-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbc63-134">请求</span><span class="sxs-lookup"><span data-stu-id="bbc63-134">Request</span></span>
<span data-ttu-id="bbc63-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbc63-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="bbc63-136">响应</span><span class="sxs-lookup"><span data-stu-id="bbc63-136">Response</span></span>
<span data-ttu-id="bbc63-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbc63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1386

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsMobileMSI",
    "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "commandLine": "Command Line value",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "ignoreVersionDetection": true,
    "identityVersion": "Identity Version value",
    "useDeviceContext": true
  }
}
```




