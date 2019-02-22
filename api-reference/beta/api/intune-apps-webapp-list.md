---
title: 列出 webApps
description: 列出 webApp 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46f4ea50a4f13e81e9b56ec6a4578c794a599340
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153569"
---
# <a name="list-webapps"></a><span data-ttu-id="b5222-103">列出 webApps</span><span class="sxs-lookup"><span data-stu-id="b5222-103">List webApps</span></span>

> <span data-ttu-id="b5222-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5222-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5222-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5222-106">列出 [webApp](../resources/intune-apps-webapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5222-106">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5222-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5222-107">Prerequisites</span></span>
<span data-ttu-id="b5222-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b5222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b5222-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5222-110">Permission type</span></span>|<span data-ttu-id="b5222-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5222-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5222-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5222-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5222-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b5222-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5222-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5222-115">Not supported.</span></span>|
|<span data-ttu-id="b5222-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5222-116">Application</span></span>|<span data-ttu-id="b5222-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5222-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5222-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5222-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b5222-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5222-119">Request headers</span></span>
|<span data-ttu-id="b5222-120">标头</span><span class="sxs-lookup"><span data-stu-id="b5222-120">Header</span></span>|<span data-ttu-id="b5222-121">值</span><span class="sxs-lookup"><span data-stu-id="b5222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5222-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5222-122">Authorization</span></span>|<span data-ttu-id="b5222-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5222-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5222-124">Accept</span></span>|<span data-ttu-id="b5222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5222-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5222-126">Request body</span></span>
<span data-ttu-id="b5222-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5222-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5222-128">响应</span><span class="sxs-lookup"><span data-stu-id="b5222-128">Response</span></span>
<span data-ttu-id="b5222-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [webApp](../resources/intune-apps-webapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b5222-129">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5222-130">示例</span><span class="sxs-lookup"><span data-stu-id="b5222-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5222-131">请求</span><span class="sxs-lookup"><span data-stu-id="b5222-131">Request</span></span>
<span data-ttu-id="b5222-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5222-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="b5222-133">响应</span><span class="sxs-lookup"><span data-stu-id="b5222-133">Response</span></span>
<span data-ttu-id="b5222-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5222-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1061

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
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```




