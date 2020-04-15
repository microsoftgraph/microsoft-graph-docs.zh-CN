---
title: 列出 webApps
description: 列出 webApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6e26e2d1a4542d691d27b8764b081d8f4302b25
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464578"
---
# <a name="list-webapps"></a><span data-ttu-id="72c6c-103">列出 webApps</span><span class="sxs-lookup"><span data-stu-id="72c6c-103">List webApps</span></span>

<span data-ttu-id="72c6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72c6c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72c6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72c6c-106">列出 [webApp](../resources/intune-apps-webapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72c6c-106">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72c6c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="72c6c-107">Prerequisites</span></span>
<span data-ttu-id="72c6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72c6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72c6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72c6c-110">Permission type</span></span>|<span data-ttu-id="72c6c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="72c6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72c6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72c6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72c6c-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c6c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72c6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72c6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72c6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72c6c-115">Not supported.</span></span>|
|<span data-ttu-id="72c6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72c6c-116">Application</span></span>|<span data-ttu-id="72c6c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="72c6c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72c6c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72c6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="72c6c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72c6c-119">Request headers</span></span>
|<span data-ttu-id="72c6c-120">标头</span><span class="sxs-lookup"><span data-stu-id="72c6c-120">Header</span></span>|<span data-ttu-id="72c6c-121">值</span><span class="sxs-lookup"><span data-stu-id="72c6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72c6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72c6c-122">Authorization</span></span>|<span data-ttu-id="72c6c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="72c6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72c6c-124">接受</span><span class="sxs-lookup"><span data-stu-id="72c6c-124">Accept</span></span>|<span data-ttu-id="72c6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72c6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72c6c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="72c6c-126">Request body</span></span>
<span data-ttu-id="72c6c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72c6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c6c-128">响应</span><span class="sxs-lookup"><span data-stu-id="72c6c-128">Response</span></span>
<span data-ttu-id="72c6c-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [webApp](../resources/intune-apps-webapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72c6c-129">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72c6c-130">示例</span><span class="sxs-lookup"><span data-stu-id="72c6c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="72c6c-131">请求</span><span class="sxs-lookup"><span data-stu-id="72c6c-131">Request</span></span>
<span data-ttu-id="72c6c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72c6c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="72c6c-133">响应</span><span class="sxs-lookup"><span data-stu-id="72c6c-133">Response</span></span>
<span data-ttu-id="72c6c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72c6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 934

{
  "value": [
    {
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
      "publishingState": "processing",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```






