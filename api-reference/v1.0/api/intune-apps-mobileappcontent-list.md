---
title: 列出 mobileAppContents
description: 列出 mobileAppContent 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74f3d13e50c293140f1a35ab3e4ec570efb45021
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515965"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="0475d-103">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="0475d-103">List mobileAppContents</span></span>

<span data-ttu-id="0475d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0475d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0475d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0475d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0475d-106">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0475d-106">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0475d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0475d-107">Prerequisites</span></span>
<span data-ttu-id="0475d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0475d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0475d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0475d-110">Permission type</span></span>|<span data-ttu-id="0475d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0475d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0475d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0475d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0475d-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0475d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0475d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0475d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0475d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0475d-115">Not supported.</span></span>|
|<span data-ttu-id="0475d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0475d-116">Application</span></span>|<span data-ttu-id="0475d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0475d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0475d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0475d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="0475d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0475d-119">Request headers</span></span>
|<span data-ttu-id="0475d-120">标头</span><span class="sxs-lookup"><span data-stu-id="0475d-120">Header</span></span>|<span data-ttu-id="0475d-121">值</span><span class="sxs-lookup"><span data-stu-id="0475d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0475d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0475d-122">Authorization</span></span>|<span data-ttu-id="0475d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0475d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0475d-124">接受</span><span class="sxs-lookup"><span data-stu-id="0475d-124">Accept</span></span>|<span data-ttu-id="0475d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0475d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0475d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0475d-126">Request body</span></span>
<span data-ttu-id="0475d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0475d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0475d-128">响应</span><span class="sxs-lookup"><span data-stu-id="0475d-128">Response</span></span>
<span data-ttu-id="0475d-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0475d-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0475d-130">示例</span><span class="sxs-lookup"><span data-stu-id="0475d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0475d-131">请求</span><span class="sxs-lookup"><span data-stu-id="0475d-131">Request</span></span>
<span data-ttu-id="0475d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0475d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="0475d-133">响应</span><span class="sxs-lookup"><span data-stu-id="0475d-133">Response</span></span>
<span data-ttu-id="0475d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0475d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```




