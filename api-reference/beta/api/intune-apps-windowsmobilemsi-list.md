---
title: 列出 windowsMobileMSIs
description: 列出 windowsMobileMSI 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a6d8dd816ca5d36f1eb3cab48f86ec22eef42a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955301"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="121e5-103">列出 windowsMobileMSIs</span><span class="sxs-lookup"><span data-stu-id="121e5-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="121e5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="121e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="121e5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="121e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="121e5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="121e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="121e5-107">列出 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="121e5-107">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="121e5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="121e5-108">Prerequisites</span></span>
<span data-ttu-id="121e5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="121e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="121e5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="121e5-111">Permission type</span></span>|<span data-ttu-id="121e5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="121e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="121e5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="121e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="121e5-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="121e5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="121e5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="121e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="121e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="121e5-116">Not supported.</span></span>|
|<span data-ttu-id="121e5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="121e5-117">Application</span></span>|<span data-ttu-id="121e5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="121e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="121e5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="121e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="121e5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="121e5-120">Request headers</span></span>
|<span data-ttu-id="121e5-121">标头</span><span class="sxs-lookup"><span data-stu-id="121e5-121">Header</span></span>|<span data-ttu-id="121e5-122">值</span><span class="sxs-lookup"><span data-stu-id="121e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="121e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="121e5-123">Authorization</span></span>|<span data-ttu-id="121e5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="121e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="121e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="121e5-125">Accept</span></span>|<span data-ttu-id="121e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="121e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="121e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="121e5-127">Request body</span></span>
<span data-ttu-id="121e5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="121e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="121e5-129">响应</span><span class="sxs-lookup"><span data-stu-id="121e5-129">Response</span></span>
<span data-ttu-id="121e5-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="121e5-130">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="121e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="121e5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="121e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="121e5-132">Request</span></span>
<span data-ttu-id="121e5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="121e5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="121e5-134">响应</span><span class="sxs-lookup"><span data-stu-id="121e5-134">Response</span></span>
<span data-ttu-id="121e5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="121e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1275

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





