---
title: 获取 resourceOperation
description: 读取 resourceOperation 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fa01fe1c3de366c2564703d96c43fb2957526c9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933419"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="fb734-103">获取 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="fb734-103">Get resourceOperation</span></span>

> <span data-ttu-id="fb734-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb734-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb734-105">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb734-105">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb734-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb734-106">Prerequisites</span></span>
<span data-ttu-id="fb734-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fb734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb734-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb734-109">Permission type</span></span>|<span data-ttu-id="fb734-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb734-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb734-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb734-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb734-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb734-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fb734-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb734-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb734-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb734-114">Not supported.</span></span>|
|<span data-ttu-id="fb734-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb734-115">Application</span></span>|<span data-ttu-id="fb734-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb734-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb734-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb734-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb734-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb734-118">Optional query parameters</span></span>
<span data-ttu-id="fb734-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb734-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fb734-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb734-120">Request headers</span></span>
|<span data-ttu-id="fb734-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb734-121">Header</span></span>|<span data-ttu-id="fb734-122">值</span><span class="sxs-lookup"><span data-stu-id="fb734-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb734-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb734-123">Authorization</span></span>|<span data-ttu-id="fb734-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb734-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb734-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb734-125">Accept</span></span>|<span data-ttu-id="fb734-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb734-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb734-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb734-127">Request body</span></span>
<span data-ttu-id="fb734-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb734-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb734-129">响应</span><span class="sxs-lookup"><span data-stu-id="fb734-129">Response</span></span>
<span data-ttu-id="fb734-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb734-130">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb734-131">示例</span><span class="sxs-lookup"><span data-stu-id="fb734-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb734-132">请求</span><span class="sxs-lookup"><span data-stu-id="fb734-132">Request</span></span>
<span data-ttu-id="fb734-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb734-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="fb734-134">响应</span><span class="sxs-lookup"><span data-stu-id="fb734-134">Response</span></span>
<span data-ttu-id="fb734-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb734-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



