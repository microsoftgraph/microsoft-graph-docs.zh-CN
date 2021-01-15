---
title: CloudPcOnPremisesConnection：runHealthChecks
description: 在云电脑本地连接上运行运行状况检查。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: d32dabad93edc1621bc7f634eff52284a0b8597a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872749"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="d89f1-103">CloudPcOnPremisesConnection：runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="d89f1-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="d89f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d89f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d89f1-105">对 [cloudPcOnPremisesConnection 对象运行运行状况](../resources/cloudpconpremisesconnection.md) 检查。</span><span class="sxs-lookup"><span data-stu-id="d89f1-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="d89f1-106">这将触发此 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的新运行状况检查，并完成检查后更改 healthCheckStatus 和 [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="d89f1-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="d89f1-107">权限</span><span class="sxs-lookup"><span data-stu-id="d89f1-107">Permissions</span></span>

<span data-ttu-id="d89f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d89f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d89f1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d89f1-110">Permission type</span></span>|<span data-ttu-id="d89f1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d89f1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d89f1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d89f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d89f1-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d89f1-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d89f1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d89f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d89f1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d89f1-115">Not supported.</span></span>|
|<span data-ttu-id="d89f1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d89f1-116">Application</span></span>|<span data-ttu-id="d89f1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d89f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d89f1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d89f1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="d89f1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d89f1-119">Request headers</span></span>

|<span data-ttu-id="d89f1-120">名称</span><span class="sxs-lookup"><span data-stu-id="d89f1-120">Name</span></span>|<span data-ttu-id="d89f1-121">说明</span><span class="sxs-lookup"><span data-stu-id="d89f1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d89f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d89f1-122">Authorization</span></span>|<span data-ttu-id="d89f1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d89f1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d89f1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d89f1-125">Request body</span></span>

<span data-ttu-id="d89f1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d89f1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d89f1-127">响应</span><span class="sxs-lookup"><span data-stu-id="d89f1-127">Response</span></span>

<span data-ttu-id="d89f1-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d89f1-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d89f1-129">示例</span><span class="sxs-lookup"><span data-stu-id="d89f1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d89f1-130">请求</span><span class="sxs-lookup"><span data-stu-id="d89f1-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d89f1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d89f1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="d89f1-132">C#</span><span class="sxs-lookup"><span data-stu-id="d89f1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d89f1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d89f1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d89f1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d89f1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d89f1-135">Java</span><span class="sxs-lookup"><span data-stu-id="d89f1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d89f1-136">响应</span><span class="sxs-lookup"><span data-stu-id="d89f1-136">Response</span></span>

<span data-ttu-id="d89f1-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d89f1-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
