---
title: 获取 resourceOperation
description: 读取 resourceOperation 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1730852f59f33eaf976d75a1595efddc17ee9592
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899513"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="e66ca-103">获取 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="e66ca-103">Get resourceOperation</span></span>

> <span data-ttu-id="e66ca-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e66ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e66ca-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e66ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e66ca-106">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e66ca-106">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e66ca-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e66ca-107">Prerequisites</span></span>
<span data-ttu-id="e66ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e66ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e66ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e66ca-110">Permission type</span></span>|<span data-ttu-id="e66ca-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e66ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e66ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e66ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e66ca-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e66ca-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e66ca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e66ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e66ca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e66ca-115">Not supported.</span></span>|
|<span data-ttu-id="e66ca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e66ca-116">Application</span></span>|<span data-ttu-id="e66ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e66ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e66ca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e66ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e66ca-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e66ca-119">Optional query parameters</span></span>
<span data-ttu-id="e66ca-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e66ca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e66ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e66ca-121">Request headers</span></span>
|<span data-ttu-id="e66ca-122">标头</span><span class="sxs-lookup"><span data-stu-id="e66ca-122">Header</span></span>|<span data-ttu-id="e66ca-123">值</span><span class="sxs-lookup"><span data-stu-id="e66ca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e66ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e66ca-124">Authorization</span></span>|<span data-ttu-id="e66ca-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e66ca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e66ca-126">接受</span><span class="sxs-lookup"><span data-stu-id="e66ca-126">Accept</span></span>|<span data-ttu-id="e66ca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e66ca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e66ca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e66ca-128">Request body</span></span>
<span data-ttu-id="e66ca-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e66ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e66ca-130">响应</span><span class="sxs-lookup"><span data-stu-id="e66ca-130">Response</span></span>
<span data-ttu-id="e66ca-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e66ca-131">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e66ca-132">示例</span><span class="sxs-lookup"><span data-stu-id="e66ca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e66ca-133">请求</span><span class="sxs-lookup"><span data-stu-id="e66ca-133">Request</span></span>
<span data-ttu-id="e66ca-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e66ca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="e66ca-135">响应</span><span class="sxs-lookup"><span data-stu-id="e66ca-135">Response</span></span>
<span data-ttu-id="e66ca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e66ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resource": "Resource value",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value",
    "enabledForScopeValidation": true
  }
}
```




