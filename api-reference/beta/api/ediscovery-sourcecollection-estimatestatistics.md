---
title: sourceCollection：estimateStatistics
description: 运行源集合的估计值。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7489f2900ef79afc95cdc00c47569a63b378572f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446010"
---
# <a name="sourcecollection-estimatestatistics"></a><span data-ttu-id="38439-103">sourceCollection：estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="38439-103">sourceCollection: estimateStatistics</span></span>

<span data-ttu-id="38439-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="38439-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38439-105">运行源集合中电子邮件和文档的估计数量。</span><span class="sxs-lookup"><span data-stu-id="38439-105">Run an estimate of the number of emails and documents in the source collection.</span></span> <span data-ttu-id="38439-106">若要了解有关电子数据展示 (搜索的源集合) ，请参阅"在高级电子数据展示"中收集 [案例的数据](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="38439-106">To learn more about source collections (also known as searches in eDiscovery), see [Collect data for a case in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

## <a name="permissions"></a><span data-ttu-id="38439-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="38439-107">Permissions</span></span>

<span data-ttu-id="38439-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38439-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38439-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38439-110">Permission type</span></span>|<span data-ttu-id="38439-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38439-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38439-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38439-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38439-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38439-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="38439-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38439-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38439-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38439-115">Not supported.</span></span>|
|<span data-ttu-id="38439-116">Application</span><span class="sxs-lookup"><span data-stu-id="38439-116">Application</span></span>|<span data-ttu-id="38439-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38439-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38439-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38439-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

## <a name="request-headers"></a><span data-ttu-id="38439-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38439-119">Request headers</span></span>

|<span data-ttu-id="38439-120">名称</span><span class="sxs-lookup"><span data-stu-id="38439-120">Name</span></span>|<span data-ttu-id="38439-121">说明</span><span class="sxs-lookup"><span data-stu-id="38439-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="38439-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38439-122">Authorization</span></span>|<span data-ttu-id="38439-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38439-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38439-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="38439-125">Request body</span></span>

<span data-ttu-id="38439-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38439-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38439-127">响应</span><span class="sxs-lookup"><span data-stu-id="38439-127">Response</span></span>

<span data-ttu-id="38439-128">如果估计成功启动，此操作将返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="38439-128">If the estimate is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="38439-129">响应还将包含一个标头，其中包含为处理估计而创建的 `Location` [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="38439-129">The response will also contain a `Location` header, which contains the location of the [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) that was created to handle the estimate.</span></span> <span data-ttu-id="38439-130">通过向位置提出 GET 请求来检查估计操作的状态，成功完成后， [状态将更改为](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded` 。</span><span class="sxs-lookup"><span data-stu-id="38439-130">Check the status of the estimate operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="38439-131">示例</span><span class="sxs-lookup"><span data-stu-id="38439-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38439-132">请求</span><span class="sxs-lookup"><span data-stu-id="38439-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "sourcecollection_estimatestatistics"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

### <a name="response"></a><span data-ttu-id="38439-133">响应</span><span class="sxs-lookup"><span data-stu-id="38439-133">Response</span></span>

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
