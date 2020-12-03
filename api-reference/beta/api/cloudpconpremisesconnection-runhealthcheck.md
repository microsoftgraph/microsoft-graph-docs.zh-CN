---
title: CloudPcOnPremisesConnection-RunHealthChecks
description: 在云 PC 本地连接上运行运行状况检查。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 949d9d01d7706f878b19702f811b4838f4e6bfe8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563288"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="59e1b-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="59e1b-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="59e1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59e1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e1b-105">对 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象运行运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="59e1b-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="59e1b-106">这将触发对此 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的新运行状况检查，并在检查完成时更改 HealthCheckStatus 和 [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="59e1b-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="59e1b-107">权限</span><span class="sxs-lookup"><span data-stu-id="59e1b-107">Permissions</span></span>

<span data-ttu-id="59e1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59e1b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59e1b-110">Permission type</span></span>|<span data-ttu-id="59e1b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59e1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59e1b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59e1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59e1b-113">CloudPC</span><span class="sxs-lookup"><span data-stu-id="59e1b-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="59e1b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59e1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59e1b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59e1b-115">Not supported.</span></span>|
|<span data-ttu-id="59e1b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59e1b-116">Application</span></span>|<span data-ttu-id="59e1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="59e1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59e1b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59e1b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="59e1b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59e1b-119">Request headers</span></span>

|<span data-ttu-id="59e1b-120">名称</span><span class="sxs-lookup"><span data-stu-id="59e1b-120">Name</span></span>|<span data-ttu-id="59e1b-121">说明</span><span class="sxs-lookup"><span data-stu-id="59e1b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59e1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59e1b-122">Authorization</span></span>|<span data-ttu-id="59e1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59e1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59e1b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="59e1b-125">Request body</span></span>

<span data-ttu-id="59e1b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59e1b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59e1b-127">响应</span><span class="sxs-lookup"><span data-stu-id="59e1b-127">Response</span></span>

<span data-ttu-id="59e1b-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="59e1b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="59e1b-129">示例</span><span class="sxs-lookup"><span data-stu-id="59e1b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59e1b-130">请求</span><span class="sxs-lookup"><span data-stu-id="59e1b-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="59e1b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="59e1b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="59e1b-132">C#</span><span class="sxs-lookup"><span data-stu-id="59e1b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59e1b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59e1b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59e1b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59e1b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59e1b-135">Java</span><span class="sxs-lookup"><span data-stu-id="59e1b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59e1b-136">响应</span><span class="sxs-lookup"><span data-stu-id="59e1b-136">Response</span></span>

<span data-ttu-id="59e1b-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="59e1b-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
