---
title: reviewSetQuery：applyTags
description: 将标记应用于与指定查询匹配的文档。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2c3f41d1fbe9851babc582c1f21c9f9673d53541
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446025"
---
# <a name="reviewsetquery-applytags"></a><span data-ttu-id="32cc0-103">reviewSetQuery：applyTags</span><span class="sxs-lookup"><span data-stu-id="32cc0-103">reviewSetQuery: applyTags</span></span>

<span data-ttu-id="32cc0-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="32cc0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="32cc0-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="32cc0-105">Permissions</span></span>

<span data-ttu-id="32cc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32cc0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="32cc0-108">Permission type</span></span>|<span data-ttu-id="32cc0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32cc0-109">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32cc0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32cc0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="32cc0-111">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32cc0-111">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="32cc0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32cc0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32cc0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="32cc0-113">Not supported.</span></span>|
|<span data-ttu-id="32cc0-114">Application</span><span class="sxs-lookup"><span data-stu-id="32cc0-114">Application</span></span>|<span data-ttu-id="32cc0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32cc0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32cc0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32cc0-116">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewSetId}/queries/{reviewSetQueryId}/applyTags
```

## <a name="request-headers"></a><span data-ttu-id="32cc0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="32cc0-117">Request headers</span></span>

|<span data-ttu-id="32cc0-118">名称</span><span class="sxs-lookup"><span data-stu-id="32cc0-118">Name</span></span>|<span data-ttu-id="32cc0-119">说明</span><span class="sxs-lookup"><span data-stu-id="32cc0-119">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32cc0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="32cc0-120">Authorization</span></span>|<span data-ttu-id="32cc0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32cc0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32cc0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32cc0-123">Content-Type</span></span>|<span data-ttu-id="32cc0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="32cc0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32cc0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="32cc0-126">Request body</span></span>

<span data-ttu-id="32cc0-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32cc0-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32cc0-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="32cc0-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32cc0-129">参数</span><span class="sxs-lookup"><span data-stu-id="32cc0-129">Parameter</span></span>|<span data-ttu-id="32cc0-130">类型</span><span class="sxs-lookup"><span data-stu-id="32cc0-130">Type</span></span>|<span data-ttu-id="32cc0-131">说明</span><span class="sxs-lookup"><span data-stu-id="32cc0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32cc0-132">tagsToAdd</span><span class="sxs-lookup"><span data-stu-id="32cc0-132">tagsToAdd</span></span>|<span data-ttu-id="32cc0-133">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32cc0-133">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="32cc0-134">要添加到与查询匹配的文档的标记的标识。</span><span class="sxs-lookup"><span data-stu-id="32cc0-134">IDs of tags to add to the documents that match the query.</span></span>|
|<span data-ttu-id="32cc0-135">tagsToRemove</span><span class="sxs-lookup"><span data-stu-id="32cc0-135">tagsToRemove</span></span>|<span data-ttu-id="32cc0-136">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32cc0-136">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="32cc0-137">要从匹配查询的文档中删除的标记的标识。</span><span class="sxs-lookup"><span data-stu-id="32cc0-137">IDs of tags to remove from the documents that match the query.</span></span>|

## <a name="response"></a><span data-ttu-id="32cc0-138">响应</span><span class="sxs-lookup"><span data-stu-id="32cc0-138">Response</span></span>

<span data-ttu-id="32cc0-139">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32cc0-139">If successful, this action returns a `202 Accepted` response code.</span></span>

<span data-ttu-id="32cc0-140">如果标记操作成功启动，此操作将返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32cc0-140">If the tagging operation is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="32cc0-141">响应还将包含一个标头，其中包含为处理标记而创建的 `Location` [tagOperation](../resources/ediscovery-tagOperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="32cc0-141">The response will also contain a `Location` header, which contains the location of the [tagOperation](../resources/ediscovery-tagOperation.md) that was created to handle the tagging.</span></span> <span data-ttu-id="32cc0-142">通过向位置提出 GET 请求来检查标记操作的状态，成功完成后， [状态将更改为](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded` 。</span><span class="sxs-lookup"><span data-stu-id="32cc0-142">Check the status of the tagging operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="32cc0-143">示例</span><span class="sxs-lookup"><span data-stu-id="32cc0-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32cc0-144">请求</span><span class="sxs-lookup"><span data-stu-id="32cc0-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reviewsetquery_applytags"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/reviewsets/6c95c2a6-31fa-45a8-93ef-dd4531974783/queries/b4798d14-748d-468e-a1ec-96a2b1d49677/applyTags
Content-Type: application/json
Content-length: 778

{
    "tagsToAdd": [
        {
            "id": "b4798d14-748d-468e-a1ec-96a2b1d49677"
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="32cc0-145">响应</span><span class="sxs-lookup"><span data-stu-id="32cc0-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 56c9dd8b-d8f7-59ae-6733-38191862c9c9,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/operations('d77f7933e88842bab3221e280be9dc0b'),
request-id: c2397a81-e9c2-4851-b669-d87e0751e45a
```
