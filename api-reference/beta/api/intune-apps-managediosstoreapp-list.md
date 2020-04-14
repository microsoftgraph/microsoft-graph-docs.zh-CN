---
title: 列出 managedIOSStoreApps
description: 列出 managedIOSStoreApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7f3a8631d67be095431e956ac8d77ae87c0b8d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405607"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="b8183-103">列出 managedIOSStoreApps</span><span class="sxs-lookup"><span data-stu-id="b8183-103">List managedIOSStoreApps</span></span>

<span data-ttu-id="b8183-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8183-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8183-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8183-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8183-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8183-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8183-107">列出 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8183-107">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8183-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8183-108">Prerequisites</span></span>
<span data-ttu-id="b8183-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8183-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8183-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8183-111">Permission type</span></span>|<span data-ttu-id="b8183-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8183-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8183-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8183-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8183-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8183-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b8183-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8183-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8183-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8183-116">Not supported.</span></span>|
|<span data-ttu-id="b8183-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8183-117">Application</span></span>|<span data-ttu-id="b8183-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8183-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8183-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8183-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b8183-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8183-120">Request headers</span></span>
|<span data-ttu-id="b8183-121">标头</span><span class="sxs-lookup"><span data-stu-id="b8183-121">Header</span></span>|<span data-ttu-id="b8183-122">值</span><span class="sxs-lookup"><span data-stu-id="b8183-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8183-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8183-123">Authorization</span></span>|<span data-ttu-id="b8183-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8183-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8183-125">接受</span><span class="sxs-lookup"><span data-stu-id="b8183-125">Accept</span></span>|<span data-ttu-id="b8183-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8183-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8183-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8183-127">Request body</span></span>
<span data-ttu-id="b8183-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8183-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8183-129">响应</span><span class="sxs-lookup"><span data-stu-id="b8183-129">Response</span></span>
<span data-ttu-id="b8183-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b8183-130">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8183-131">示例</span><span class="sxs-lookup"><span data-stu-id="b8183-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8183-132">请求</span><span class="sxs-lookup"><span data-stu-id="b8183-132">Request</span></span>
<span data-ttu-id="b8183-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8183-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="b8183-134">响应</span><span class="sxs-lookup"><span data-stu-id="b8183-134">Response</span></span>
<span data-ttu-id="b8183-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8183-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSStoreApp",
      "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
        "v13_0": true
      }
    }
  ]
}
```



