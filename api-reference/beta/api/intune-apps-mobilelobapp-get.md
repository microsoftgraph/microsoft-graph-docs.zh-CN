---
title: 获取 mobileLobApp
description: 读取 mobileLobApp 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 3dec2c91e3a2484f0b6f725cc96bb370230a1b72
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319129"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="f1cc0-103">获取 mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="f1cc0-103">Get mobileLobApp</span></span>

> <span data-ttu-id="f1cc0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1cc0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1cc0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1cc0-107">读取 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-107">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1cc0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1cc0-108">Prerequisites</span></span>
<span data-ttu-id="f1cc0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f1cc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1cc0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1cc0-111">Permission type</span></span>|<span data-ttu-id="f1cc0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1cc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1cc0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1cc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1cc0-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1cc0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1cc0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1cc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1cc0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-116">Not supported.</span></span>|
|<span data-ttu-id="f1cc0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1cc0-117">Application</span></span>|<span data-ttu-id="f1cc0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1cc0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1cc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1cc0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f1cc0-120">Optional query parameters</span></span>
<span data-ttu-id="f1cc0-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1cc0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1cc0-122">Request headers</span></span>
|<span data-ttu-id="f1cc0-123">标头</span><span class="sxs-lookup"><span data-stu-id="f1cc0-123">Header</span></span>|<span data-ttu-id="f1cc0-124">值</span><span class="sxs-lookup"><span data-stu-id="f1cc0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1cc0-125">授权</span><span class="sxs-lookup"><span data-stu-id="f1cc0-125">Authorization</span></span>|<span data-ttu-id="f1cc0-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1cc0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f1cc0-127">Accept</span></span>|<span data-ttu-id="f1cc0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f1cc0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1cc0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1cc0-129">Request body</span></span>
<span data-ttu-id="f1cc0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1cc0-131">响应</span><span class="sxs-lookup"><span data-stu-id="f1cc0-131">Response</span></span>
<span data-ttu-id="f1cc0-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-132">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1cc0-133">示例</span><span class="sxs-lookup"><span data-stu-id="f1cc0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1cc0-134">请求</span><span class="sxs-lookup"><span data-stu-id="f1cc0-134">Request</span></span>
<span data-ttu-id="f1cc0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f1cc0-136">响应</span><span class="sxs-lookup"><span data-stu-id="f1cc0-136">Response</span></span>
<span data-ttu-id="f1cc0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1cc0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 949

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
    "uploadState": 11,
    "publishingState": "processing",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```





