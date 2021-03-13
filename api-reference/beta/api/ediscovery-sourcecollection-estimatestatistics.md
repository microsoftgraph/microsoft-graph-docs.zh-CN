---
title: sourceCollection： estimateStatistics
description: 运行源集合的估计值。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2ae6b7363bdb1be34e38dd7f5502962fc920808d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772707"
---
# <a name="sourcecollection-estimatestatistics"></a><span data-ttu-id="4b65c-103">sourceCollection： estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="4b65c-103">sourceCollection: estimateStatistics</span></span>

<span data-ttu-id="4b65c-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4b65c-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b65c-105">运行源集合中电子邮件和文档的估计数量。</span><span class="sxs-lookup"><span data-stu-id="4b65c-105">Run an estimate of the number of emails and documents in the source collection.</span></span> <span data-ttu-id="4b65c-106">若要了解有关源集合 (电子数据展示中的搜索) ，请参阅在高级电子数据展示 中收集 [案例的数据](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="4b65c-106">To learn more about source collections (also known as searches in eDiscovery), see [Collect data for a case in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b65c-107">权限</span><span class="sxs-lookup"><span data-stu-id="4b65c-107">Permissions</span></span>

<span data-ttu-id="4b65c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b65c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b65c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b65c-110">Permission type</span></span>|<span data-ttu-id="4b65c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b65c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b65c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b65c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b65c-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b65c-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4b65c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b65c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b65c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b65c-115">Not supported.</span></span>|
|<span data-ttu-id="4b65c-116">Application</span><span class="sxs-lookup"><span data-stu-id="4b65c-116">Application</span></span>|<span data-ttu-id="4b65c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b65c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b65c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b65c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

## <a name="request-headers"></a><span data-ttu-id="4b65c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b65c-119">Request headers</span></span>

|<span data-ttu-id="4b65c-120">名称</span><span class="sxs-lookup"><span data-stu-id="4b65c-120">Name</span></span>|<span data-ttu-id="4b65c-121">说明</span><span class="sxs-lookup"><span data-stu-id="4b65c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4b65c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b65c-122">Authorization</span></span>|<span data-ttu-id="4b65c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b65c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b65c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b65c-125">Request body</span></span>

<span data-ttu-id="4b65c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b65c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b65c-127">响应</span><span class="sxs-lookup"><span data-stu-id="4b65c-127">Response</span></span>

<span data-ttu-id="4b65c-128">如果估计成功启动，此操作将返回 响应 `202 Accepted` 代码。</span><span class="sxs-lookup"><span data-stu-id="4b65c-128">If the estimate is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="4b65c-129">响应还将包含标头，其中包含为处理估计而创建的 `Location` [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="4b65c-129">The response will also contain a `Location` header, which contains the location of the [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) that was created to handle the estimate.</span></span> <span data-ttu-id="4b65c-130">通过向位置提出 GET 请求来检查估计操作的状态，成功完成后， [状态](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) 将更改为 `succeeded` 。</span><span class="sxs-lookup"><span data-stu-id="4b65c-130">Check the status of the estimate operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="4b65c-131">示例</span><span class="sxs-lookup"><span data-stu-id="4b65c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b65c-132">请求</span><span class="sxs-lookup"><span data-stu-id="4b65c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4b65c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b65c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollection_estimatestatistics"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```
# <a name="c"></a>[<span data-ttu-id="4b65c-134">C#</span><span class="sxs-lookup"><span data-stu-id="4b65c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollection-estimatestatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b65c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b65c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollection-estimatestatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b65c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b65c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollection-estimatestatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b65c-137">Java</span><span class="sxs-lookup"><span data-stu-id="4b65c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollection-estimatestatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b65c-138">响应</span><span class="sxs-lookup"><span data-stu-id="4b65c-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: private
client-request-id: af32de50-99d9-e3a8-371b-a4f366cc78e7
content-length: 0
content-type: text/plain
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/82edd40e182a464fa02c24a36fa94873
request-id: e890176f-640f-4222-9cd8-be26e71c5e5d
```
