---
title: 获取 resourceOperation
description: 读取 resourceOperation 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80345f5ed9f6675f63882104fc983c0dc6586191
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461327"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="3b795-103">获取 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="3b795-103">Get resourceOperation</span></span>

<span data-ttu-id="3b795-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b795-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b795-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b795-106">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b795-106">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b795-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b795-107">Prerequisites</span></span>
<span data-ttu-id="3b795-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b795-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b795-110">Permission type</span></span>|<span data-ttu-id="3b795-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b795-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b795-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b795-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b795-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b795-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3b795-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b795-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b795-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b795-115">Not supported.</span></span>|
|<span data-ttu-id="3b795-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b795-116">Application</span></span>|<span data-ttu-id="3b795-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b795-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b795-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b795-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b795-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3b795-119">Optional query parameters</span></span>
<span data-ttu-id="3b795-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3b795-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b795-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b795-121">Request headers</span></span>
|<span data-ttu-id="3b795-122">标头</span><span class="sxs-lookup"><span data-stu-id="3b795-122">Header</span></span>|<span data-ttu-id="3b795-123">值</span><span class="sxs-lookup"><span data-stu-id="3b795-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b795-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b795-124">Authorization</span></span>|<span data-ttu-id="3b795-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b795-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b795-126">接受</span><span class="sxs-lookup"><span data-stu-id="3b795-126">Accept</span></span>|<span data-ttu-id="3b795-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3b795-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b795-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b795-128">Request body</span></span>
<span data-ttu-id="3b795-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b795-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b795-130">响应</span><span class="sxs-lookup"><span data-stu-id="3b795-130">Response</span></span>
<span data-ttu-id="3b795-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b795-131">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b795-132">示例</span><span class="sxs-lookup"><span data-stu-id="3b795-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b795-133">请求</span><span class="sxs-lookup"><span data-stu-id="3b795-133">Request</span></span>
<span data-ttu-id="3b795-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b795-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="3b795-135">响应</span><span class="sxs-lookup"><span data-stu-id="3b795-135">Response</span></span>
<span data-ttu-id="3b795-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b795-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value"
  }
}
```






