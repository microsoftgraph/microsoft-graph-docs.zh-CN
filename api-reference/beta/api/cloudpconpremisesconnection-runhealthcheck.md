---
title: CloudPcOnPremisesConnection-RunHealthChecks
description: 在云 PC 本地连接上运行运行状况检查。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 484d48f0400c328090d66bbcf7a930a485a9d950
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378271"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="a727d-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="a727d-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="a727d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a727d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a727d-105">对 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象运行运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="a727d-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="a727d-106">这将触发对此 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的新运行状况检查，并在检查完成时更改 HealthCheckStatus 和 [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="a727d-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

## <a name="permissions"></a><span data-ttu-id="a727d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a727d-107">Permissions</span></span>

<span data-ttu-id="a727d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a727d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a727d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a727d-110">Permission type</span></span>|<span data-ttu-id="a727d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a727d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a727d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a727d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a727d-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a727d-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a727d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a727d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a727d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a727d-115">Not supported.</span></span>|
|<span data-ttu-id="a727d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a727d-116">Application</span></span>|<span data-ttu-id="a727d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a727d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a727d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a727d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="a727d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a727d-119">Request headers</span></span>

|<span data-ttu-id="a727d-120">名称</span><span class="sxs-lookup"><span data-stu-id="a727d-120">Name</span></span>|<span data-ttu-id="a727d-121">说明</span><span class="sxs-lookup"><span data-stu-id="a727d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a727d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a727d-122">Authorization</span></span>|<span data-ttu-id="a727d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a727d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a727d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a727d-125">Request body</span></span>

<span data-ttu-id="a727d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a727d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a727d-127">响应</span><span class="sxs-lookup"><span data-stu-id="a727d-127">Response</span></span>

<span data-ttu-id="a727d-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a727d-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a727d-129">示例</span><span class="sxs-lookup"><span data-stu-id="a727d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a727d-130">请求</span><span class="sxs-lookup"><span data-stu-id="a727d-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

### <a name="response"></a><span data-ttu-id="a727d-131">响应</span><span class="sxs-lookup"><span data-stu-id="a727d-131">Response</span></span>

<span data-ttu-id="a727d-132">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a727d-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
