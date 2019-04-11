---
title: 列出 windowsMobileMSIs
description: 列出 windowsMobileMSI 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7c66f9bf1d94e7efcb41cdd3767d068cea72908
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780733"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="921de-103">列出 windowsMobileMSIs</span><span class="sxs-lookup"><span data-stu-id="921de-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="921de-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="921de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="921de-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="921de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921de-106">列出 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="921de-106">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="921de-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="921de-107">Prerequisites</span></span>
<span data-ttu-id="921de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="921de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="921de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="921de-110">Permission type</span></span>|<span data-ttu-id="921de-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="921de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="921de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="921de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="921de-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="921de-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="921de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="921de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="921de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="921de-115">Not supported.</span></span>|
|<span data-ttu-id="921de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="921de-116">Application</span></span>|<span data-ttu-id="921de-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="921de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="921de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="921de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="921de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="921de-119">Request headers</span></span>
|<span data-ttu-id="921de-120">标头</span><span class="sxs-lookup"><span data-stu-id="921de-120">Header</span></span>|<span data-ttu-id="921de-121">值</span><span class="sxs-lookup"><span data-stu-id="921de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="921de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="921de-122">Authorization</span></span>|<span data-ttu-id="921de-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="921de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="921de-124">接受</span><span class="sxs-lookup"><span data-stu-id="921de-124">Accept</span></span>|<span data-ttu-id="921de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="921de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="921de-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="921de-126">Request body</span></span>
<span data-ttu-id="921de-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="921de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="921de-128">响应</span><span class="sxs-lookup"><span data-stu-id="921de-128">Response</span></span>
<span data-ttu-id="921de-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="921de-129">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="921de-130">示例</span><span class="sxs-lookup"><span data-stu-id="921de-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="921de-131">请求</span><span class="sxs-lookup"><span data-stu-id="921de-131">Request</span></span>
<span data-ttu-id="921de-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="921de-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="921de-133">响应</span><span class="sxs-lookup"><span data-stu-id="921de-133">Response</span></span>
<span data-ttu-id="921de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="921de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1407

{
  "value": [
    {
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
  ]
}
```





