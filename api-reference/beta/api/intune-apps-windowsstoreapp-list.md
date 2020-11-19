---
title: 列出 windowsStoreApps
description: 列出 windowsStoreApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b27ed0335d3522c6ebb538385fd70851a9e3266d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49246150"
---
# <a name="list-windowsstoreapps"></a><span data-ttu-id="dcf7c-103">列出 windowsStoreApps</span><span class="sxs-lookup"><span data-stu-id="dcf7c-103">List windowsStoreApps</span></span>

<span data-ttu-id="dcf7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcf7c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcf7c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcf7c-107">列出 [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-107">List properties and relationships of the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcf7c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dcf7c-108">Prerequisites</span></span>
<span data-ttu-id="dcf7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf7c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcf7c-111">Permission type</span></span>|<span data-ttu-id="dcf7c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dcf7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcf7c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcf7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcf7c-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcf7c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dcf7c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcf7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcf7c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-116">Not supported.</span></span>|
|<span data-ttu-id="dcf7c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcf7c-117">Application</span></span>|<span data-ttu-id="dcf7c-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcf7c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcf7c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcf7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dcf7c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcf7c-120">Request headers</span></span>
|<span data-ttu-id="dcf7c-121">标头</span><span class="sxs-lookup"><span data-stu-id="dcf7c-121">Header</span></span>|<span data-ttu-id="dcf7c-122">值</span><span class="sxs-lookup"><span data-stu-id="dcf7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcf7c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf7c-123">Authorization</span></span>|<span data-ttu-id="dcf7c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcf7c-125">接受</span><span class="sxs-lookup"><span data-stu-id="dcf7c-125">Accept</span></span>|<span data-ttu-id="dcf7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcf7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcf7c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcf7c-127">Request body</span></span>
<span data-ttu-id="dcf7c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf7c-129">响应</span><span class="sxs-lookup"><span data-stu-id="dcf7c-129">Response</span></span>
<span data-ttu-id="dcf7c-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-130">If successful, this method returns a `200 OK` response code and a collection of [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf7c-131">示例</span><span class="sxs-lookup"><span data-stu-id="dcf7c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcf7c-132">请求</span><span class="sxs-lookup"><span data-stu-id="dcf7c-132">Request</span></span>
<span data-ttu-id="dcf7c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="dcf7c-134">响应</span><span class="sxs-lookup"><span data-stu-id="dcf7c-134">Response</span></span>
<span data-ttu-id="dcf7c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dcf7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1142

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsStoreApp",
      "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```




