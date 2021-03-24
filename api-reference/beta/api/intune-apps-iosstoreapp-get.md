---
title: 获取 iosStoreApp
description: 读取 iosStoreApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 071cf3323c89ec5b6ac2692eb32dd0b2230cd8a0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144156"
---
# <a name="get-iosstoreapp"></a><span data-ttu-id="aeb71-103">获取 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="aeb71-103">Get iosStoreApp</span></span>

<span data-ttu-id="aeb71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeb71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aeb71-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aeb71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aeb71-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aeb71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeb71-107">读取 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aeb71-107">Read properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aeb71-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aeb71-108">Prerequisites</span></span>
<span data-ttu-id="aeb71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aeb71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeb71-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aeb71-111">Permission type</span></span>|<span data-ttu-id="aeb71-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aeb71-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeb71-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aeb71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aeb71-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeb71-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aeb71-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aeb71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeb71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aeb71-116">Not supported.</span></span>|
|<span data-ttu-id="aeb71-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aeb71-117">Application</span></span>|<span data-ttu-id="aeb71-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeb71-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeb71-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aeb71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aeb71-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aeb71-120">Optional query parameters</span></span>
<span data-ttu-id="aeb71-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aeb71-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeb71-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aeb71-122">Request headers</span></span>
|<span data-ttu-id="aeb71-123">标头</span><span class="sxs-lookup"><span data-stu-id="aeb71-123">Header</span></span>|<span data-ttu-id="aeb71-124">值</span><span class="sxs-lookup"><span data-stu-id="aeb71-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeb71-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeb71-125">Authorization</span></span>|<span data-ttu-id="aeb71-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aeb71-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aeb71-127">接受</span><span class="sxs-lookup"><span data-stu-id="aeb71-127">Accept</span></span>|<span data-ttu-id="aeb71-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aeb71-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeb71-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="aeb71-129">Request body</span></span>
<span data-ttu-id="aeb71-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aeb71-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeb71-131">响应</span><span class="sxs-lookup"><span data-stu-id="aeb71-131">Response</span></span>
<span data-ttu-id="aeb71-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aeb71-132">If successful, this method returns a `200 OK` response code and [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeb71-133">示例</span><span class="sxs-lookup"><span data-stu-id="aeb71-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="aeb71-134">请求</span><span class="sxs-lookup"><span data-stu-id="aeb71-134">Request</span></span>
<span data-ttu-id="aeb71-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aeb71-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="aeb71-136">响应</span><span class="sxs-lookup"><span data-stu-id="aeb71-136">Response</span></span>
<span data-ttu-id="aeb71-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aeb71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1516

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
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
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
      "v12_0": true,
      "v13_0": true,
      "v14_0": true
    }
  }
}
```




