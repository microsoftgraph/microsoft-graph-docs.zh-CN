---
title: 列出 microsoftStoreForBusinessApps
description: 列出 microsoftStoreForBusinessApp 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d18a519558b9ecd855b75998ea10b1a8258b2cc4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355168"
---
# <a name="list-microsoftstoreforbusinessapps"></a><span data-ttu-id="34ed1-103">列出 microsoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="34ed1-103">List microsoftStoreForBusinessApps</span></span>

> <span data-ttu-id="34ed1-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34ed1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ed1-105">列出 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34ed1-105">List properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34ed1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="34ed1-106">Prerequisites</span></span>
<span data-ttu-id="34ed1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ed1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="34ed1-109">Permission type</span></span>|<span data-ttu-id="34ed1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34ed1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34ed1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34ed1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34ed1-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ed1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="34ed1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34ed1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34ed1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="34ed1-114">Not supported.</span></span>|
|<span data-ttu-id="34ed1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="34ed1-115">Application</span></span>|<span data-ttu-id="34ed1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34ed1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34ed1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34ed1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="34ed1-118">请求头</span><span class="sxs-lookup"><span data-stu-id="34ed1-118">Request headers</span></span>
|<span data-ttu-id="34ed1-119">标头</span><span class="sxs-lookup"><span data-stu-id="34ed1-119">Header</span></span>|<span data-ttu-id="34ed1-120">值</span><span class="sxs-lookup"><span data-stu-id="34ed1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34ed1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34ed1-121">Authorization</span></span>|<span data-ttu-id="34ed1-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34ed1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34ed1-123">接受</span><span class="sxs-lookup"><span data-stu-id="34ed1-123">Accept</span></span>|<span data-ttu-id="34ed1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34ed1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ed1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="34ed1-125">Request body</span></span>
<span data-ttu-id="34ed1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34ed1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34ed1-127">响应</span><span class="sxs-lookup"><span data-stu-id="34ed1-127">Response</span></span>
<span data-ttu-id="34ed1-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="34ed1-128">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ed1-129">示例</span><span class="sxs-lookup"><span data-stu-id="34ed1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="34ed1-130">请求</span><span class="sxs-lookup"><span data-stu-id="34ed1-130">Request</span></span>
<span data-ttu-id="34ed1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34ed1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="34ed1-132">响应</span><span class="sxs-lookup"><span data-stu-id="34ed1-132">Response</span></span>
<span data-ttu-id="34ed1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34ed1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1070

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
      "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
      "publishingState": "processing",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "productKey": "Product Key value",
      "licenseType": "online",
      "packageIdentityName": "Package Identity Name value"
    }
  ]
}
```




