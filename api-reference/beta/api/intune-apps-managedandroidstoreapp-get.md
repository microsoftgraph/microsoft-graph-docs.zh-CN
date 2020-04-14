---
title: 获取 managedAndroidStoreApp
description: 读取 managedAndroidStoreApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 292fbf26b3612c51d96f77178265727791e57051
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406272"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="aa21b-103">获取 managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="aa21b-103">Get managedAndroidStoreApp</span></span>

<span data-ttu-id="aa21b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa21b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa21b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa21b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa21b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa21b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa21b-107">读取 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa21b-107">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa21b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa21b-108">Prerequisites</span></span>
<span data-ttu-id="aa21b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa21b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa21b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa21b-111">Permission type</span></span>|<span data-ttu-id="aa21b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa21b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa21b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa21b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa21b-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa21b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aa21b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa21b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa21b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa21b-116">Not supported.</span></span>|
|<span data-ttu-id="aa21b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa21b-117">Application</span></span>|<span data-ttu-id="aa21b-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa21b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa21b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa21b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa21b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aa21b-120">Optional query parameters</span></span>
<span data-ttu-id="aa21b-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aa21b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa21b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa21b-122">Request headers</span></span>
|<span data-ttu-id="aa21b-123">标头</span><span class="sxs-lookup"><span data-stu-id="aa21b-123">Header</span></span>|<span data-ttu-id="aa21b-124">值</span><span class="sxs-lookup"><span data-stu-id="aa21b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa21b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa21b-125">Authorization</span></span>|<span data-ttu-id="aa21b-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa21b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa21b-127">接受</span><span class="sxs-lookup"><span data-stu-id="aa21b-127">Accept</span></span>|<span data-ttu-id="aa21b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aa21b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa21b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa21b-129">Request body</span></span>
<span data-ttu-id="aa21b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa21b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa21b-131">响应</span><span class="sxs-lookup"><span data-stu-id="aa21b-131">Response</span></span>
<span data-ttu-id="aa21b-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa21b-132">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa21b-133">示例</span><span class="sxs-lookup"><span data-stu-id="aa21b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa21b-134">请求</span><span class="sxs-lookup"><span data-stu-id="aa21b-134">Request</span></span>
<span data-ttu-id="aa21b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa21b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="aa21b-136">响应</span><span class="sxs-lookup"><span data-stu-id="aa21b-136">Response</span></span>
<span data-ttu-id="aa21b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa21b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1547

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
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
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
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    }
  }
}
```



