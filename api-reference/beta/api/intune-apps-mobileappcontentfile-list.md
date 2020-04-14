---
title: 列出 mobileAppContentFiles
description: 列出 mobileAppContentFile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38b4cbbe0d32f701cbc83af1343748a6aed31718
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43415541"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="ea8eb-103">列出 mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="ea8eb-103">List mobileAppContentFiles</span></span>

<span data-ttu-id="ea8eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea8eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea8eb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea8eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea8eb-107">列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-107">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea8eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea8eb-108">Prerequisites</span></span>
<span data-ttu-id="ea8eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea8eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea8eb-111">Permission type</span></span>|<span data-ttu-id="ea8eb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea8eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea8eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea8eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea8eb-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea8eb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ea8eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea8eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea8eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-116">Not supported.</span></span>|
|<span data-ttu-id="ea8eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea8eb-117">Application</span></span>|<span data-ttu-id="ea8eb-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea8eb-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea8eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea8eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="ea8eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea8eb-120">Request headers</span></span>
|<span data-ttu-id="ea8eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea8eb-121">Header</span></span>|<span data-ttu-id="ea8eb-122">值</span><span class="sxs-lookup"><span data-stu-id="ea8eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea8eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea8eb-123">Authorization</span></span>|<span data-ttu-id="ea8eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea8eb-125">接受</span><span class="sxs-lookup"><span data-stu-id="ea8eb-125">Accept</span></span>|<span data-ttu-id="ea8eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea8eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea8eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea8eb-127">Request body</span></span>
<span data-ttu-id="ea8eb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea8eb-129">响应</span><span class="sxs-lookup"><span data-stu-id="ea8eb-129">Response</span></span>
<span data-ttu-id="ea8eb-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea8eb-131">示例</span><span class="sxs-lookup"><span data-stu-id="ea8eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea8eb-132">请求</span><span class="sxs-lookup"><span data-stu-id="ea8eb-132">Request</span></span>
<span data-ttu-id="ea8eb-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="ea8eb-134">响应</span><span class="sxs-lookup"><span data-stu-id="ea8eb-134">Response</span></span>
<span data-ttu-id="ea8eb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea8eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContentFile",
      "azureStorageUri": "Azure Storage Uri value",
      "isCommitted": true,
      "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "name": "Name value",
      "size": 4,
      "sizeEncrypted": 13,
      "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
      "manifest": "bWFuaWZlc3Q=",
      "uploadState": "transientError",
      "isFrameworkFile": true,
      "isDependency": true
    }
  ]
}
```



