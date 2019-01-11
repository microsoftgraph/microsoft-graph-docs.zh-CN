---
title: 获取 mobileLobApp
description: 读取 mobileLobApp 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 54a7337fc83ed4d9cb715def2e5404c7208ac27b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855494"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="75447-103">获取 mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="75447-103">Get mobileLobApp</span></span>

> <span data-ttu-id="75447-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="75447-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75447-105">读取 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75447-105">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75447-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="75447-106">Prerequisites</span></span>
<span data-ttu-id="75447-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="75447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75447-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="75447-109">Permission type</span></span>|<span data-ttu-id="75447-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="75447-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75447-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75447-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75447-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="75447-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="75447-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75447-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75447-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="75447-114">Not supported.</span></span>|
|<span data-ttu-id="75447-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="75447-115">Application</span></span>|<span data-ttu-id="75447-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="75447-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75447-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75447-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75447-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75447-118">Optional query parameters</span></span>
<span data-ttu-id="75447-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75447-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="75447-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="75447-120">Request headers</span></span>
|<span data-ttu-id="75447-121">标头</span><span class="sxs-lookup"><span data-stu-id="75447-121">Header</span></span>|<span data-ttu-id="75447-122">值</span><span class="sxs-lookup"><span data-stu-id="75447-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75447-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75447-123">Authorization</span></span>|<span data-ttu-id="75447-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="75447-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75447-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75447-125">Accept</span></span>|<span data-ttu-id="75447-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75447-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75447-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="75447-127">Request body</span></span>
<span data-ttu-id="75447-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75447-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75447-129">响应</span><span class="sxs-lookup"><span data-stu-id="75447-129">Response</span></span>
<span data-ttu-id="75447-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75447-130">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75447-131">示例</span><span class="sxs-lookup"><span data-stu-id="75447-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="75447-132">请求</span><span class="sxs-lookup"><span data-stu-id="75447-132">Request</span></span>
<span data-ttu-id="75447-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75447-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="75447-134">响应</span><span class="sxs-lookup"><span data-stu-id="75447-134">Response</span></span>
<span data-ttu-id="75447-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75447-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```



