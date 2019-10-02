---
title: 列出 resourceOperations
description: 列出 resourceOperation 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34d296f8ef034b66d944b537c94dd33a6f802135
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361838"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="b56aa-103">列出 resourceOperations</span><span class="sxs-lookup"><span data-stu-id="b56aa-103">List resourceOperations</span></span>

> <span data-ttu-id="b56aa-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b56aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b56aa-105">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b56aa-105">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b56aa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b56aa-106">Prerequisites</span></span>
<span data-ttu-id="b56aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b56aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b56aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b56aa-109">Permission type</span></span>|<span data-ttu-id="b56aa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b56aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b56aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b56aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b56aa-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b56aa-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b56aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b56aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b56aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b56aa-114">Not supported.</span></span>|
|<span data-ttu-id="b56aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b56aa-115">Application</span></span>|<span data-ttu-id="b56aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b56aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b56aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b56aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="b56aa-118">请求头</span><span class="sxs-lookup"><span data-stu-id="b56aa-118">Request headers</span></span>
|<span data-ttu-id="b56aa-119">标头</span><span class="sxs-lookup"><span data-stu-id="b56aa-119">Header</span></span>|<span data-ttu-id="b56aa-120">值</span><span class="sxs-lookup"><span data-stu-id="b56aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b56aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b56aa-121">Authorization</span></span>|<span data-ttu-id="b56aa-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b56aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b56aa-123">接受</span><span class="sxs-lookup"><span data-stu-id="b56aa-123">Accept</span></span>|<span data-ttu-id="b56aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b56aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b56aa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b56aa-125">Request body</span></span>
<span data-ttu-id="b56aa-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b56aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b56aa-127">响应</span><span class="sxs-lookup"><span data-stu-id="b56aa-127">Response</span></span>
<span data-ttu-id="b56aa-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b56aa-128">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b56aa-129">示例</span><span class="sxs-lookup"><span data-stu-id="b56aa-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b56aa-130">请求</span><span class="sxs-lookup"><span data-stu-id="b56aa-130">Request</span></span>
<span data-ttu-id="b56aa-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b56aa-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="b56aa-132">响应</span><span class="sxs-lookup"><span data-stu-id="b56aa-132">Response</span></span>
<span data-ttu-id="b56aa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b56aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value"
    }
  ]
}
```




