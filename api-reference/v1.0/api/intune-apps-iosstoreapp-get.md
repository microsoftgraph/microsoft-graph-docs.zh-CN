---
title: 获取 iosStoreApp
description: 读取 iosStoreApp 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: dfe25e6b5f57ea8e862d9a9c86d40aa35ec0ca05
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340367"
---
# <a name="get-iosstoreapp"></a><span data-ttu-id="979ec-103">获取 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="979ec-103">Get iosStoreApp</span></span>

> <span data-ttu-id="979ec-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="979ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="979ec-105">读取 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="979ec-105">Read properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="979ec-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="979ec-106">Prerequisites</span></span>
<span data-ttu-id="979ec-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="979ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="979ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="979ec-109">Permission type</span></span>|<span data-ttu-id="979ec-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="979ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="979ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="979ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="979ec-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="979ec-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="979ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="979ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="979ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="979ec-114">Not supported.</span></span>|
|<span data-ttu-id="979ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="979ec-115">Application</span></span>|<span data-ttu-id="979ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="979ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="979ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="979ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="979ec-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="979ec-118">Optional query parameters</span></span>
<span data-ttu-id="979ec-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="979ec-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="979ec-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="979ec-120">Request headers</span></span>
|<span data-ttu-id="979ec-121">标头</span><span class="sxs-lookup"><span data-stu-id="979ec-121">Header</span></span>|<span data-ttu-id="979ec-122">值</span><span class="sxs-lookup"><span data-stu-id="979ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="979ec-123">授权</span><span class="sxs-lookup"><span data-stu-id="979ec-123">Authorization</span></span>|<span data-ttu-id="979ec-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="979ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="979ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="979ec-125">Accept</span></span>|<span data-ttu-id="979ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="979ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="979ec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="979ec-127">Request body</span></span>
<span data-ttu-id="979ec-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="979ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="979ec-129">响应</span><span class="sxs-lookup"><span data-stu-id="979ec-129">Response</span></span>
<span data-ttu-id="979ec-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="979ec-130">If successful, this method returns a `200 OK` response code and [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="979ec-131">示例</span><span class="sxs-lookup"><span data-stu-id="979ec-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="979ec-132">请求</span><span class="sxs-lookup"><span data-stu-id="979ec-132">Request</span></span>
<span data-ttu-id="979ec-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="979ec-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="979ec-134">响应</span><span class="sxs-lookup"><span data-stu-id="979ec-134">Response</span></span>
<span data-ttu-id="979ec-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="979ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1265

{
  "value": {
    "@odata.type": "#microsoft.graph.iosStoreApp",
    "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
    "bundleId": "Bundle Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true
    }
  }
}
```



