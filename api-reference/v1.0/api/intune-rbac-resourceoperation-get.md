---
title: 获取 resourceOperation
description: 读取 resourceOperation 对象的属性和关系。
ms.openlocfilehash: b5d449dc1eb113058e76fb40770f5acaeffe064b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010217"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="538ca-103">获取 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="538ca-103">Get resourceOperation</span></span>

> <span data-ttu-id="538ca-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="538ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="538ca-105">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="538ca-105">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="538ca-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="538ca-106">Prerequisites</span></span>
<span data-ttu-id="538ca-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="538ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="538ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="538ca-109">Permission type</span></span>|<span data-ttu-id="538ca-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="538ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="538ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="538ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="538ca-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="538ca-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="538ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="538ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="538ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="538ca-114">Not supported.</span></span>|
|<span data-ttu-id="538ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="538ca-115">Application</span></span>|<span data-ttu-id="538ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="538ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="538ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="538ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="538ca-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="538ca-118">Optional query parameters</span></span>
<span data-ttu-id="538ca-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="538ca-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="538ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="538ca-120">Request headers</span></span>
|<span data-ttu-id="538ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="538ca-121">Header</span></span>|<span data-ttu-id="538ca-122">值</span><span class="sxs-lookup"><span data-stu-id="538ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="538ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="538ca-123">Authorization</span></span>|<span data-ttu-id="538ca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="538ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="538ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="538ca-125">Accept</span></span>|<span data-ttu-id="538ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="538ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="538ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="538ca-127">Request body</span></span>
<span data-ttu-id="538ca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="538ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="538ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="538ca-129">Response</span></span>
<span data-ttu-id="538ca-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="538ca-130">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="538ca-131">示例</span><span class="sxs-lookup"><span data-stu-id="538ca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="538ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="538ca-132">Request</span></span>
<span data-ttu-id="538ca-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="538ca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="538ca-134">响应</span><span class="sxs-lookup"><span data-stu-id="538ca-134">Response</span></span>
<span data-ttu-id="538ca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="538ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



