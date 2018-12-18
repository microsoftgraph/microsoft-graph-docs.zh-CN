---
title: 列出 androidStoreApps
description: 列出 androidStoreApp 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 0f3e1b0ca33d6995cd8dbdc30207395e5f5075a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330931"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="9c74d-103">列出 androidStoreApps</span><span class="sxs-lookup"><span data-stu-id="9c74d-103">List androidStoreApps</span></span>

> <span data-ttu-id="9c74d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9c74d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c74d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9c74d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c74d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c74d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c74d-107">列出 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c74d-107">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c74d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c74d-108">Prerequisites</span></span>
<span data-ttu-id="9c74d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9c74d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c74d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c74d-111">Permission type</span></span>|<span data-ttu-id="9c74d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c74d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c74d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c74d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c74d-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c74d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9c74d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c74d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c74d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c74d-116">Not supported.</span></span>|
|<span data-ttu-id="9c74d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c74d-117">Application</span></span>|<span data-ttu-id="9c74d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c74d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c74d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c74d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9c74d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c74d-120">Request headers</span></span>
|<span data-ttu-id="9c74d-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c74d-121">Header</span></span>|<span data-ttu-id="9c74d-122">值</span><span class="sxs-lookup"><span data-stu-id="9c74d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c74d-123">授权</span><span class="sxs-lookup"><span data-stu-id="9c74d-123">Authorization</span></span>|<span data-ttu-id="9c74d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c74d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c74d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c74d-125">Accept</span></span>|<span data-ttu-id="9c74d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c74d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c74d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c74d-127">Request body</span></span>
<span data-ttu-id="9c74d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c74d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c74d-129">响应</span><span class="sxs-lookup"><span data-stu-id="9c74d-129">Response</span></span>
<span data-ttu-id="9c74d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9c74d-130">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c74d-131">示例</span><span class="sxs-lookup"><span data-stu-id="9c74d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c74d-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c74d-132">Request</span></span>
<span data-ttu-id="9c74d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c74d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="9c74d-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c74d-134">Response</span></span>
<span data-ttu-id="9c74d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c74d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1483

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidStoreApp",
      "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
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
        "v5_1": true,
        "v6_0": true,
        "v7_0": true,
        "v7_1": true,
        "v8_0": true,
        "v8_1": true,
        "v9_0": true
      }
    }
  ]
}
```





