---
title: 获取 managedAndroidStoreApp
description: 读取 managedAndroidStoreApp 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 914102e24b2c594bcd1302cbcf7579470c28ae16
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347668"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="90ab8-103">获取 managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="90ab8-103">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="90ab8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="90ab8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90ab8-105">读取 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90ab8-105">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90ab8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="90ab8-106">Prerequisites</span></span>
<span data-ttu-id="90ab8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="90ab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ab8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90ab8-109">Permission type</span></span>|<span data-ttu-id="90ab8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90ab8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ab8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90ab8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90ab8-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="90ab8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="90ab8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90ab8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ab8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90ab8-114">Not supported.</span></span>|
|<span data-ttu-id="90ab8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90ab8-115">Application</span></span>|<span data-ttu-id="90ab8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90ab8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ab8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90ab8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90ab8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90ab8-118">Optional query parameters</span></span>
<span data-ttu-id="90ab8-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="90ab8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="90ab8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="90ab8-120">Request headers</span></span>
|<span data-ttu-id="90ab8-121">标头</span><span class="sxs-lookup"><span data-stu-id="90ab8-121">Header</span></span>|<span data-ttu-id="90ab8-122">值</span><span class="sxs-lookup"><span data-stu-id="90ab8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ab8-123">授权</span><span class="sxs-lookup"><span data-stu-id="90ab8-123">Authorization</span></span>|<span data-ttu-id="90ab8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90ab8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ab8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90ab8-125">Accept</span></span>|<span data-ttu-id="90ab8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90ab8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ab8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="90ab8-127">Request body</span></span>
<span data-ttu-id="90ab8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90ab8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ab8-129">响应</span><span class="sxs-lookup"><span data-stu-id="90ab8-129">Response</span></span>
<span data-ttu-id="90ab8-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90ab8-130">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ab8-131">示例</span><span class="sxs-lookup"><span data-stu-id="90ab8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="90ab8-132">请求</span><span class="sxs-lookup"><span data-stu-id="90ab8-132">Request</span></span>
<span data-ttu-id="90ab8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90ab8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="90ab8-134">响应</span><span class="sxs-lookup"><span data-stu-id="90ab8-134">Response</span></span>
<span data-ttu-id="90ab8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90ab8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1275

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
    "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    }
  }
}
```



