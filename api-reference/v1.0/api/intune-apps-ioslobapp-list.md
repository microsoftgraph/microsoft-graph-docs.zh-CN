---
title: 列出 iosLobApps
description: 列出 iosLobApp 对象的属性和关系。
ms.openlocfilehash: 0abbf97189bdeaf5835da287783db447ba626993
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008553"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="cd294-103">列出 iosLobApps</span><span class="sxs-lookup"><span data-stu-id="cd294-103">List iosLobApps</span></span>

> <span data-ttu-id="cd294-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cd294-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd294-105">列出 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd294-105">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd294-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd294-106">Prerequisites</span></span>
<span data-ttu-id="cd294-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cd294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd294-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd294-109">Permission type</span></span>|<span data-ttu-id="cd294-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd294-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd294-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd294-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd294-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd294-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cd294-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd294-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd294-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd294-114">Not supported.</span></span>|
|<span data-ttu-id="cd294-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd294-115">Application</span></span>|<span data-ttu-id="cd294-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd294-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd294-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd294-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cd294-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd294-118">Request headers</span></span>
|<span data-ttu-id="cd294-119">标头</span><span class="sxs-lookup"><span data-stu-id="cd294-119">Header</span></span>|<span data-ttu-id="cd294-120">值</span><span class="sxs-lookup"><span data-stu-id="cd294-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd294-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd294-121">Authorization</span></span>|<span data-ttu-id="cd294-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd294-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd294-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cd294-123">Accept</span></span>|<span data-ttu-id="cd294-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd294-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd294-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd294-125">Request body</span></span>
<span data-ttu-id="cd294-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd294-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd294-127">响应</span><span class="sxs-lookup"><span data-stu-id="cd294-127">Response</span></span>
<span data-ttu-id="cd294-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cd294-128">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd294-129">示例</span><span class="sxs-lookup"><span data-stu-id="cd294-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd294-130">请求</span><span class="sxs-lookup"><span data-stu-id="cd294-130">Request</span></span>
<span data-ttu-id="cd294-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd294-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="cd294-132">响应</span><span class="sxs-lookup"><span data-stu-id="cd294-132">Response</span></span>
<span data-ttu-id="cd294-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd294-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobApp",
      "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
      "size": 4,
      "bundleId": "Bundle Id value",
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
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value"
    }
  ]
}
```



