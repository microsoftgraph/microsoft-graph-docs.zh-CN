---
title: 获取 mobileAppContentFile
description: 读取 mobileAppContentFile 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 3f72f132b8c6e1c1b08a487abd95391f639683a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350594"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="c1b9e-103">获取 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c1b9e-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="c1b9e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1b9e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1b9e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1b9e-107">读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-107">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1b9e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1b9e-108">Prerequisites</span></span>
<span data-ttu-id="c1b9e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c1b9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b9e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1b9e-111">Permission type</span></span>|<span data-ttu-id="c1b9e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1b9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b9e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1b9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b9e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1b9e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1b9e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1b9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b9e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-116">Not supported.</span></span>|
|<span data-ttu-id="c1b9e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1b9e-117">Application</span></span>|<span data-ttu-id="c1b9e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b9e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1b9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1b9e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1b9e-120">Optional query parameters</span></span>
<span data-ttu-id="c1b9e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c1b9e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1b9e-122">Request headers</span></span>
|<span data-ttu-id="c1b9e-123">标头</span><span class="sxs-lookup"><span data-stu-id="c1b9e-123">Header</span></span>|<span data-ttu-id="c1b9e-124">值</span><span class="sxs-lookup"><span data-stu-id="c1b9e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b9e-125">授权</span><span class="sxs-lookup"><span data-stu-id="c1b9e-125">Authorization</span></span>|<span data-ttu-id="c1b9e-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b9e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c1b9e-127">Accept</span></span>|<span data-ttu-id="c1b9e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b9e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b9e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1b9e-129">Request body</span></span>
<span data-ttu-id="c1b9e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1b9e-131">响应</span><span class="sxs-lookup"><span data-stu-id="c1b9e-131">Response</span></span>
<span data-ttu-id="c1b9e-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-132">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b9e-133">示例</span><span class="sxs-lookup"><span data-stu-id="c1b9e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1b9e-134">请求</span><span class="sxs-lookup"><span data-stu-id="c1b9e-134">Request</span></span>
<span data-ttu-id="c1b9e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="c1b9e-136">响应</span><span class="sxs-lookup"><span data-stu-id="c1b9e-136">Response</span></span>
<span data-ttu-id="c1b9e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContentFile",
    "azureStorageUri": "Azure Storage Uri value",
    "isCommitted": true,
    "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "name": "Name value",
    "size": 4,
    "sizeEncrypted": 13,
    "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
    "manifest": "bWFuaWZlc3Q=",
    "uploadState": "transientError",
    "isFrameworkFile": true,
    "isDependency": true
  }
}
```





