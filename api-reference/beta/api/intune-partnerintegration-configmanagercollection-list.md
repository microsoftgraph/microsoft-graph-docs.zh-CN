---
title: 列出 configManagerCollections
description: 列出 configManagerCollection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 165ed79f911fb0ef8505d75029e28cdf1003eb93
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337017"
---
# <a name="list-configmanagercollections"></a><span data-ttu-id="958a1-103">列出 configManagerCollections</span><span class="sxs-lookup"><span data-stu-id="958a1-103">List configManagerCollections</span></span>

<span data-ttu-id="958a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="958a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="958a1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="958a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="958a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="958a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="958a1-107">列出 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="958a1-107">List properties and relationships of the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="958a1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="958a1-108">Prerequisites</span></span>
<span data-ttu-id="958a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="958a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="958a1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="958a1-111">Permission type</span></span>|<span data-ttu-id="958a1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="958a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="958a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="958a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="958a1-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="958a1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="958a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="958a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="958a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="958a1-116">Not supported.</span></span>|
|<span data-ttu-id="958a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="958a1-117">Application</span></span>|<span data-ttu-id="958a1-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="958a1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="958a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="958a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="958a1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="958a1-120">Request headers</span></span>
|<span data-ttu-id="958a1-121">标头</span><span class="sxs-lookup"><span data-stu-id="958a1-121">Header</span></span>|<span data-ttu-id="958a1-122">值</span><span class="sxs-lookup"><span data-stu-id="958a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="958a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="958a1-123">Authorization</span></span>|<span data-ttu-id="958a1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="958a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="958a1-125">接受</span><span class="sxs-lookup"><span data-stu-id="958a1-125">Accept</span></span>|<span data-ttu-id="958a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="958a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="958a1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="958a1-127">Request body</span></span>
<span data-ttu-id="958a1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="958a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="958a1-129">响应</span><span class="sxs-lookup"><span data-stu-id="958a1-129">Response</span></span>
<span data-ttu-id="958a1-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="958a1-130">If successful, this method returns a `200 OK` response code and a collection of [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="958a1-131">示例</span><span class="sxs-lookup"><span data-stu-id="958a1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="958a1-132">请求</span><span class="sxs-lookup"><span data-stu-id="958a1-132">Request</span></span>
<span data-ttu-id="958a1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="958a1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
```

### <a name="response"></a><span data-ttu-id="958a1-134">响应</span><span class="sxs-lookup"><span data-stu-id="958a1-134">Response</span></span>
<span data-ttu-id="958a1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="958a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.configManagerCollection",
      "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
      "displayName": "Display Name value",
      "collectionIdentifier": "Collection Identifier value",
      "hierarchyName": "Hierarchy Name value",
      "hierarchyIdentifier": "Hierarchy Identifier value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




