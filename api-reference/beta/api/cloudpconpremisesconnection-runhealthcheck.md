---
title: CloudPcOnPremisesConnection：runHealthChecks
description: 在云电脑本地连接上运行运行状况检查。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b207be1da6585adcabb76c8f51f048db1e159d77
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705840"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="195a5-103">CloudPcOnPremisesConnection：runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="195a5-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="195a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="195a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="195a5-105">对 [cloudPcOnPremisesConnection 对象运行运行状况](../resources/cloudpconpremisesconnection.md) 检查。</span><span class="sxs-lookup"><span data-stu-id="195a5-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="195a5-106">这将触发此 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的新运行状况检查，并完成检查后更改 healthCheckStatus 和 [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="195a5-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="195a5-107">权限</span><span class="sxs-lookup"><span data-stu-id="195a5-107">Permissions</span></span>

<span data-ttu-id="195a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="195a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="195a5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="195a5-110">Permission type</span></span>|<span data-ttu-id="195a5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="195a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="195a5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="195a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="195a5-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="195a5-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="195a5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="195a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="195a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="195a5-115">Not supported.</span></span>|
|<span data-ttu-id="195a5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="195a5-116">Application</span></span>|<span data-ttu-id="195a5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="195a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="195a5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="195a5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="195a5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="195a5-119">Request headers</span></span>

|<span data-ttu-id="195a5-120">名称</span><span class="sxs-lookup"><span data-stu-id="195a5-120">Name</span></span>|<span data-ttu-id="195a5-121">说明</span><span class="sxs-lookup"><span data-stu-id="195a5-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="195a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="195a5-122">Authorization</span></span>|<span data-ttu-id="195a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="195a5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="195a5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="195a5-125">Request body</span></span>

<span data-ttu-id="195a5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="195a5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="195a5-127">响应</span><span class="sxs-lookup"><span data-stu-id="195a5-127">Response</span></span>

<span data-ttu-id="195a5-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="195a5-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="195a5-129">示例</span><span class="sxs-lookup"><span data-stu-id="195a5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="195a5-130">请求</span><span class="sxs-lookup"><span data-stu-id="195a5-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="195a5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="195a5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="195a5-132">C#</span><span class="sxs-lookup"><span data-stu-id="195a5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="195a5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="195a5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="195a5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="195a5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="195a5-135">Java</span><span class="sxs-lookup"><span data-stu-id="195a5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="195a5-136">响应</span><span class="sxs-lookup"><span data-stu-id="195a5-136">Response</span></span>

<span data-ttu-id="195a5-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="195a5-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
