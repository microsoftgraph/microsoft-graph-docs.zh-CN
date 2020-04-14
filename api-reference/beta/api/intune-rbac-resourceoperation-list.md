---
title: 列出 resourceOperations
description: 列出 resourceOperation 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd783dbe77e0f5b0b81d5871ff97740eb792cdf8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455430"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="3dbc6-103">列出 resourceOperations</span><span class="sxs-lookup"><span data-stu-id="3dbc6-103">List resourceOperations</span></span>

<span data-ttu-id="3dbc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dbc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3dbc6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dbc6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dbc6-107">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dbc6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3dbc6-108">Prerequisites</span></span>
<span data-ttu-id="3dbc6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dbc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dbc6-111">Permission type</span></span>|<span data-ttu-id="3dbc6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3dbc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dbc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dbc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3dbc6-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dbc6-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3dbc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dbc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dbc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-116">Not supported.</span></span>|
|<span data-ttu-id="3dbc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dbc6-117">Application</span></span>|<span data-ttu-id="3dbc6-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dbc6-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dbc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dbc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="3dbc6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dbc6-120">Request headers</span></span>
|<span data-ttu-id="3dbc6-121">标头</span><span class="sxs-lookup"><span data-stu-id="3dbc6-121">Header</span></span>|<span data-ttu-id="3dbc6-122">值</span><span class="sxs-lookup"><span data-stu-id="3dbc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dbc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dbc6-123">Authorization</span></span>|<span data-ttu-id="3dbc6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dbc6-125">接受</span><span class="sxs-lookup"><span data-stu-id="3dbc6-125">Accept</span></span>|<span data-ttu-id="3dbc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dbc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dbc6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dbc6-127">Request body</span></span>
<span data-ttu-id="3dbc6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dbc6-129">响应</span><span class="sxs-lookup"><span data-stu-id="3dbc6-129">Response</span></span>
<span data-ttu-id="3dbc6-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dbc6-131">示例</span><span class="sxs-lookup"><span data-stu-id="3dbc6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dbc6-132">请求</span><span class="sxs-lookup"><span data-stu-id="3dbc6-132">Request</span></span>
<span data-ttu-id="3dbc6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="3dbc6-134">响应</span><span class="sxs-lookup"><span data-stu-id="3dbc6-134">Response</span></span>
<span data-ttu-id="3dbc6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3dbc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```



