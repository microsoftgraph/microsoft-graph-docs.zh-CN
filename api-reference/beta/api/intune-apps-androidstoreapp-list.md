---
title: 列出 androidStoreApps
description: 列出 androidStoreApp 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0ab42416053a69795cb660db4eac3ab77fb6ca6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977259"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="f76d8-103">列出 androidStoreApps</span><span class="sxs-lookup"><span data-stu-id="f76d8-103">List androidStoreApps</span></span>

> <span data-ttu-id="f76d8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f76d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f76d8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f76d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f76d8-106">列出 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f76d8-106">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f76d8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f76d8-107">Prerequisites</span></span>
<span data-ttu-id="f76d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f76d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76d8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f76d8-110">Permission type</span></span>|<span data-ttu-id="f76d8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f76d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f76d8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f76d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f76d8-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f76d8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f76d8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f76d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f76d8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f76d8-115">Not supported.</span></span>|
|<span data-ttu-id="f76d8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f76d8-116">Application</span></span>|<span data-ttu-id="f76d8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f76d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f76d8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f76d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f76d8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f76d8-119">Request headers</span></span>
|<span data-ttu-id="f76d8-120">标头</span><span class="sxs-lookup"><span data-stu-id="f76d8-120">Header</span></span>|<span data-ttu-id="f76d8-121">值</span><span class="sxs-lookup"><span data-stu-id="f76d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f76d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f76d8-122">Authorization</span></span>|<span data-ttu-id="f76d8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f76d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f76d8-124">接受</span><span class="sxs-lookup"><span data-stu-id="f76d8-124">Accept</span></span>|<span data-ttu-id="f76d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f76d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f76d8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f76d8-126">Request body</span></span>
<span data-ttu-id="f76d8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f76d8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f76d8-128">响应</span><span class="sxs-lookup"><span data-stu-id="f76d8-128">Response</span></span>
<span data-ttu-id="f76d8-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f76d8-129">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76d8-130">示例</span><span class="sxs-lookup"><span data-stu-id="f76d8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f76d8-131">请求</span><span class="sxs-lookup"><span data-stu-id="f76d8-131">Request</span></span>
<span data-ttu-id="f76d8-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f76d8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f76d8-133">响应</span><span class="sxs-lookup"><span data-stu-id="f76d8-133">Response</span></span>
<span data-ttu-id="f76d8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f76d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1584

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
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




