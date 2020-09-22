---
title: 列出 androidManagedStoreWebApps
description: 列出 androidManagedStoreWebApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 100be07e4fe275484ff848933afbeef273b86d8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006284"
---
# <a name="list-androidmanagedstorewebapps"></a><span data-ttu-id="43c3a-103">列出 androidManagedStoreWebApps</span><span class="sxs-lookup"><span data-stu-id="43c3a-103">List androidManagedStoreWebApps</span></span>

<span data-ttu-id="43c3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43c3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43c3a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43c3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43c3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43c3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c3a-107">列出 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43c3a-107">List properties and relationships of the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43c3a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="43c3a-108">Prerequisites</span></span>
<span data-ttu-id="43c3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43c3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c3a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43c3a-111">Permission type</span></span>|<span data-ttu-id="43c3a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43c3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43c3a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43c3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43c3a-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43c3a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43c3a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43c3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43c3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43c3a-116">Not supported.</span></span>|
|<span data-ttu-id="43c3a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="43c3a-117">Application</span></span>|<span data-ttu-id="43c3a-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43c3a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43c3a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43c3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="43c3a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="43c3a-120">Request headers</span></span>
|<span data-ttu-id="43c3a-121">标头</span><span class="sxs-lookup"><span data-stu-id="43c3a-121">Header</span></span>|<span data-ttu-id="43c3a-122">值</span><span class="sxs-lookup"><span data-stu-id="43c3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43c3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c3a-123">Authorization</span></span>|<span data-ttu-id="43c3a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43c3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43c3a-125">接受</span><span class="sxs-lookup"><span data-stu-id="43c3a-125">Accept</span></span>|<span data-ttu-id="43c3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43c3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43c3a-127">Request body</span></span>
<span data-ttu-id="43c3a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43c3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c3a-129">响应</span><span class="sxs-lookup"><span data-stu-id="43c3a-129">Response</span></span>
<span data-ttu-id="43c3a-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="43c3a-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43c3a-131">示例</span><span class="sxs-lookup"><span data-stu-id="43c3a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c3a-132">请求</span><span class="sxs-lookup"><span data-stu-id="43c3a-132">Request</span></span>
<span data-ttu-id="43c3a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43c3a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="43c3a-134">响应</span><span class="sxs-lookup"><span data-stu-id="43c3a-134">Response</span></span>
<span data-ttu-id="43c3a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43c3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
      "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "isPrivate": true,
      "isSystemApp": true,
      "appTracks": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
          "trackId": "Track Id value",
          "trackAlias": "Track Alias value"
        }
      ],
      "supportsOemConfig": true
    }
  ]
}
```






